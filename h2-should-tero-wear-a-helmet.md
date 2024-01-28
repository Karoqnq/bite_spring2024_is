# H2 Should Tero wear a helmet?

## a) Read and summarise
- Braiterman et al 2020: Threat modeling manifesto
- Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course (12 parts, about 15 min total, audio is enough for all except video 7 "Data flow diagrams")
- Shostack 2014: Chapter 1 - Dive In and Threat Model!
- OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet
  
  
  ### [Summary of Braiterman et al 2020: Threat modeling manifesto](https://www.threatmodelingmanifesto.org/)

-	Threat Modeling is the analysis of a system / company with the purpose of highlighting any possible risks concerning security and privacy

-	Four key questions: What are we working on? What can go wrong? What are we going to do about it? Did we do a good enough job?

-	Why? Pinpoint possible problems that need solving which in return will affect the decisions you’ll make moving forward

-	Threat Modeling Manifesto > a guide to develop your own threat model

-	Follows a 2 guideline format > Values, Principle

-	Value > relative importance, there’s value in all things but one can have more than the other

-	Principles >  3 types = general truths, patterns that are recommended, patterns (anti-patterns) that should be avoided


  ### [Summary of Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course](https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf)

-	Why? To predict problems which are likely to occur before they would cause the company any loss ex. security wise, expenses etc.

-	What are we working on?
  
Collaboration is important and valuable.

Sketching makes it easier to put your thoughts on paper and communicate them especially in the starting stages 

Make records about what you’re doing, what have you done etc. With them you can learn new things about the systems and get details which will help with with finding out what can go wrong

Data flow diagrams are important > threats tend to follow data

5 symbols >
Sharp corners = anything outside of your control
Soft corners = anything under your control
Data flows = element to connect the first two
Drums = data storage
Trust boundary = show that different elements are operated by different entities

-	What can go wrong?
  
Use different structures like STRIDE or a kill chain to help find concerns. Structures help keep consistency.

STRIDE = Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privileges


-	What are we going to do about it?
  
You need to do something about each and every threat, however, it is different for any field so the best constant is to track your work and go from there.
Apply risk management to a subset of the threats you discover. Some threats you can fix immediately, some take more time and some can never be fixed.


  ### [Summary of Shostack 2014: Chapter 1 - Dive In and Threat Model!](https://www.oreilly.com/library/view/threat-modeling-designing/9781118810057/9781118810057c01.xhtml#c1)

  -	Enables you to find issues before everything is set in stone
    
  -	Using a model helps abstract away a portion of the details and see a bigger picture
    
  -	When playing an instrument, you need to develop muscles and awareness by actually playing the instrument.Through practice it gets easier and you’ll become better. It’s the same for threat modelling while following the four-step breakdown.


  ### [Summary of OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html)

  -	Structured repeatable process meant for gaining insight into security characteristics, modelling a system from the perspective of security, identifying threats based on the model, and determining the responses to those threats.

-	Ideally performed as early as possible.

-	Maintain, update and refine alongside the system.

-	Advantages > Improved Visibility of Target of Evaluation, Increased Security Awareness, Identify Risks Early-On 

-	Many different threat modelling techniques (PASTA, STRIDE, OCTAVE etc.), no right or wrong but most follow the same four key questions.

-	Broken down into basic steps: Application decomposition, threat identification and ranking, mitigations, and review and validation.


## b) Security hygiene. What basic security practices should everyone follow? Are there some security hygiene practicies that you consider useful, but might be above an average Joe?

-	Back up your data 

-	Use Two-Factor Authentication

-	Strong passwords + password manager (I think this was one of the things I was surprised about in class as I was the only one to have a password manager)

-	Use Antivirus software/ existing antivirus turned on (ex. Windows)

-	Educate yourself on security threats (I fell for a phising scam and lost an account and everything related to all my personal info + uni work for the entirety of first year so I try to stay on board with the newer methods)

-	Keep your software updated (updates can be regarding updating the systems / software from possible threats)

## c) Make-belief boogie-man - a threat model for imaginary company.

A long, extensive answer with narrative, analysis and a diagram is expected.
Create an imaginary company and create threat model.
Business requirements come from business, technical specialist help with tech. Inlude this in your narrative.
Your analysis should cover all parts of the four question model (four key questions in Threat modeling manifesto)

(1) What are we working on?
Our assets
Priorization, key assets
E.g. customer health data is a crown jevel, personel gaming server is probably not
Security supports business
Draw a diagram of the company systems
Write a description.

(2) What can go wrong?
Apply one or more named models: Attack trees, STRIDE, ATT&CK...
Give some examples of identified risks - you don't need to find all risks or likely vulnerabilites, as there would be too many for this homework.
Priorize biggest risks
High expected value (or other very high risk)
Expected value = probability * monetary value
Expected value is a tool for discussion, it's not exact science as we have to guestimate the input numbers
Are you targetted by specific threat actors?
Known TTPs? (tactics, techniques, procedures)
COI - Capability, Opportunity, Intent

(3) What are we going to do about it?
Can you: reduce attack surface, limit entry points...
Reduce, transfer, avoid, accept

(4) Did we do a good enough job?
Security audits, pentests, assesments, continous threat modeling and evaluation


## My company: 

### What are we working on? <br />

StudyFurn is a student focused online platform where students can connect to others by selling and buying affordable furniture, books, and other household appliances.

For our assets we have divided them up into 4 prioritised categories:

Authentication and Security -> StudyInfo for authentication, review system, buyer protection policies <br />
Affordability -> Students selling to students, market known for less income <br />
Diversity of Payments -> MobilePay, Card, Klarna etc.<br />
Connectivity -> Get to know students from all over, build relationships <br />

![image](https://cdn.discordapp.com/attachments/476838378227236867/1201018750481223720/image.png?ex=65c84adf&is=65b5d5df&hm=428c3831040b22eb0298752aafa4cc865ed68ff3488a24200187a49fb400bde2&)

Description: <br />
Our flow diagram represents a simplified version of how the company systems work. <br />
<br />
First of all the user interacts with our application for which they need to make an account. To make an account they have to authenticate themselves through our partner StudyInfo and will be taken to their website to confirm that they are a student. StudyInfo most commonly uses bank credentials to authenticate the legitemasy of the person as it's connected to their government id. As the authentication is necessary to be able to use our app, we've added both StudyInfo and the Banking API into our trust boundary even though they are external entities. Our payments are done through third party applications such as MobilePay, PayPal and Klarna. Due to this we can't promise that nothing will happen to their systems so they've been left out of the trust boundary.


### What can go wrong?

For risks we've decided to use the STRIDE model. We've divided our risks into 4 seperate categories taking into count the potential probability and impact. <br />

### Trust and Safety <br />
Probability = low/moderate 
Monetary impact = high <br />
- Spoofing > Fake accounts, identity theft
- Tampering > Unauthorized modification / access to user data
- Information Disclosure > unauthorized disclosure of sensitive information <br />

### Technical Difficulties <br />
Probability = moderate 
Monetary impact = high <br />
- Denial of Service > System overload, service disruption, servers down

### Market Competition
Probability = moderate
Monetary impact = high/moderate
- Information Disclosure > Unauthorized disclosure of sensitive information <br />

### Brand Management
Probability = moderate
Monetary impact = moderate/low
- Tampering > False accusations in public-facing content
  

### What are we going to do about it?

###Mitigation for the possible risks:

Spoofing: <br />
We've implemented a multi-factor authentication with our partner StudyInfo. StudyInfo uses bank credentials for authentication which are tied to government IDs, adding an extra layer of verification to prevent fake accounts and identity theft.

#### Tampering (Unauthorized access to user data):<br />
Encryption of all sensitive data. Sensitive user data, such as personal information and transaction details is encrypted, ensuring the integrity and confidentiality of user information.

#### Information Disclosure:<br />
Control and monitor data access. Regular check ups are conducted to track access to sensitive information. Access controls are implemented to restrict data access only to authorized personel, reducing the risk of unauthorized information disclosure.

#### Denial Of Service: <br />
Scalable Infrastructure and server traffic monitoring. The platform would use scalable infrastructure, which allows it to dynamically scale resources based on demand. Automated tools can continuously monitor server traffic and incase of potential disruptions staff can manually intervene to take care of the potential threats.

#### Tampering(False accusations in public-facing content):<br />
Review system. The review system involves both automated and manual content checks. Additionally, customer support actively monitors and addresses reports of false accusations, providing a smooth content management process.

###For continuity:

#### Security Training: Regular training sessions for the development and support teams so they stay updated on the best pratices.
#### Continuous Monitoring: Implement monitoring tools which can detect and respond to potential security threats. 
#### User Education: Emphasize the importance of account security and online practices. Possibly, by in app notifications etc.









  



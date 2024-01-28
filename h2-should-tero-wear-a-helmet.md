# H2 Should Tero wear a helmet?

### a) Read and summarise
- Braiterman et al 2020: Threat modeling manifesto
- Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course (12 parts, about 15 min total, audio is enough for all except video 7 "Data flow diagrams")
- Shostack 2014: Chapter 1 - Dive In and Threat Model!
- OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet
  
  ## [Summary of Braiterman et al 2020: Threat modeling manifesto](https://www.threatmodelingmanifesto.org/)

-	Threat Modeling is the analysis of a system / company with the purpose of highlighting any possible risks concerning security and privacy

-	Four key questions: What are we working on? What can go wrong? What are we going to do about it? Did we do a good enough job?

-	Why? Pinpoint possible problems that need solving which in return will affect the decisions you’ll make moving forward

-	Threat Modeling Manifesto > a guide to develop your own threat model

-	Follows a 2 guideline format > Values, Principle

-	Value > relative importance, there’s value in all things but one can have more than the other

-	Principles >  3 types = general truths, patterns that are recommended, patterns (anti-patterns) that should be avoided


  ## [Summary of Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course](https://www.youtube.com/playlist?list=PLCVhBqLDKoOOZqKt74QI4pbDUnXSQo0nf)

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


  ## [Summary of Shostack 2014: Chapter 1 - Dive In and Threat Model!](https://www.oreilly.com/library/view/threat-modeling-designing/9781118810057/9781118810057c01.xhtml#c1)

  -	Enables you to find issues before everything is set in stone
    
  -	Using a model helps abstract away a portion of the details and see a bigger picture
    
  -	When playing an instrument, you need to develop muscles and awareness by actually playing the instrument.Through practice it gets easier and you’ll become better. It’s the same for threat modelling while following the four-step breakdown.


  ## [Summary of OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html)

  -	Structured repeatable process meant for gaining insight into security characteristics, modelling a system from the perspective of security, identifying threats based on the model, and determining the responses to those threats.

-	Ideally performed as early as possible.

-	Maintain, update and refine alongside the system.

-	Advantages > Improved Visibility of Target of Evaluation, Increased Security Awareness, Identify Risks Early-On 

-	Many different threat modelling techniques (PASTA, STRIDE, OCTAVE etc.), no right or wrong but most follow the same four key questions.

-	Broken down into basic steps: Application decomposition, threat identification and ranking, mitigations, and review and validation.

### b) Security hygiene. What basic security practices should everyone follow? Are there some security hygiene practicies that you consider useful, but might be above an average Joe?




  



# Assignment H3 - Web

## x) Read and summarize (This subtask x does not require tests with a computer. Some bullets per article is enough for your summary, feel free to write more if you like)
###OWASP (Open Worldwide Application Security Project) 10 2021:


### A05:2021-Security Misconfiguration URL: https://owasp.org/Top10/A05_2021-Security_Misconfiguration/
- 90% applications tested for some form of misconfiguration, with an average incidence rate of 4%
#### Vulnerabilites (if application is...)  >
- Missing appropriate security hardening across any part of the application stack or improperly configured permissions on cloud services,
- unnecessary features are enabled or installed,
- default accounts and their passwords are still enabled and unchanged,
- error handling reveals stack traces or other overly informative error messages to users
- the latest security features are disabled or not configured securely,
- the security settings in the application servers, application frameworks, libraries, databases, etc. are not set to secure values,
- the server does not send security headers or directives,
- the software is out of date

  
#### Prevention >
- Repeadable hardening process, development, QA and production environments configured identically, with different credentials in each
- Minimal platform, no unnecessary components, documentation, features, and samples
- A task to continuesly review and update the configurations appropriate to all security notes, updates, and patches
- A segmented application architecture
- Send security directives to clients
- An automated process to verify the effectiveness of the configurations and settings in all environments

  
#### Example of an attack >
- The application server comes with sample applications not removed from the production server. These sample applications have known security flaws attackers use to compromise the server. Suppose one of these applications is the admin console, and default accounts weren't changed. In that case, the attacker logs in with default passwords and takes over.



### A06:2021-Vulnerable and Outdated Components URL: https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/
#### Vulnerabilities >
- Not knowledgeable of the versions of all components in use
- Software is vulnerable, unsupported, or out of date
- Not scanning for vulnerabilities on a regular basis
- Not fixing or upgrading underlying platforms, frameworks, and dependencies in a risk-based timely fashion
- Not testing the compatibility of updates, upgraded, or patches libraries
- Not securing the components' configurations

#### Prevention >
- Remove unused dependencies, unnecessary features, components, files, and documentation
- Continuously inventory the versions of both client-side and server-side components using secure tools
- Obtain components from official sources over secure links
- Monitor for libraries and components that are unmaintained or do not create security patches for older versions

#### Example of an attack >
- Components typically run with the same privileges as the application itself, so flaws in any component can result in serious impact. Such flaws can be accidental (e.g., coding error) or intentional (e.g., a backdoor in a component). Some example exploitable component vulnerabilities discovered are:

CVE-2017-5638, a Struts 2 remote code execution vulnerability that enables the execution of arbitrary code on the server, has been blamed for significant breaches.


### A03:2021-Injection URL: https://owasp.org/Top10/A03_2021-Injection/
- 94% of applications were tested for some form of injection with the max incidence rate of 19%, and an average incidence rate of 3%
#### Vulnerabilities >
- User-supplied data is not validated, filtered, or sanitized by the application
- Dynamic queries or non-parameterized calls without context-aware escaping are used directly in the interpreter.
- Hostile data is used within object-relational mapping (ORM) search parameters to extract additional, sensitive records
- Hostile data is directly used or concatenated
  
#### Common injections > 
- SQL, NoSQL, OS command, Object Relational Mapping (ORM), Expression Language (EL), Object Graph Navigation Library (OGNL)

#### Prevention >
- Use a safe API, which avoids using the interpreter entirely, provides a parameterized interface, or migrates to Object Relational Mapping Tools
- Use positive server-side input validation (Not complete defense)
- For any residual dynamic queries, escape special characters using the specific escape syntax for that interpreter
- Use LIMIT and other SQL controls within queries to prevent mass disclosure of records in case of SQL injection

#### Example of an attack >
- An application uses untrusted data in the construction of the following vulnerable SQL call: String query = "SELECT \* FROM accounts WHERE custID='" + request.getParameter("id") + "'";

## a) Goat. Install WebGoat 2023.4. This subtask does not need to be reported, unless there are technical problems.
- Done
  
## b) F12. Solve Webgoat 2023.4: General: Developer tools.
Did this in class, not sure if I have to redo it for this assignment.
  
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/b7293e13-b0b4-4e81-8155-f25aee1176ae)

  
## c) Not outdated. Update all operating system and all applications in your Linux.
Ran the following code ($ sudo apt-get -y dist-upgrade) to make sure everything was up to date
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/1668da20-5c4b-4d1b-9a59-27611130dac7)

## d) Sequel. Solve SQLZoo:
-  0 SELECT basics and 2 SELECT from World, from first two subtasks.
  
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/c4c9a1cc-c86c-441e-8060-530ce14cef5f)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/9414bb55-7667-456f-80ff-00bb13fcb5bd)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/ab8dd78f-576b-42a9-8c50-7ee2aa58d68c)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/99b972c8-d6b0-4256-85f7-b2929436cd9e)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/81011b0f-252d-41f0-9af3-9235848ced3e)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/212a8190-43e3-48c9-a870-96da90e5121a)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/5abee2c9-472e-43f1-a964-02a17e462b01)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/477f53e1-bbb0-474e-a8f7-c8ba23818efb)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/db5cc09d-ba33-496c-85c2-c1b1a054c7da)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/a58b49f5-66e3-4f2f-b390-7bbba36b3893)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/cf3bb0c4-ef0f-410a-9a3c-ae6550515334)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/5665c9a8-03e5-4d90-a06b-d4d575d2a40a)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/d72cf6dc-bd8b-4349-ba82-4ab63b81388c)
    ![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/e9babd43-3dda-4bc1-8f16-fcaa2a54d14f)
    
## e) Johnny tables. Solve Portswigger Labs: Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data
- This is the website we were forwarded to
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/c135d8e6-8bde-4cff-a8a8-1b87859fcb71)
- When we check the refined search we can see that the category is defined by different topics depending on which one you're looking at. 
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/41eb7d54-072b-43c3-987c-a4e09494f3a4)
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/eaab5d80-9029-404b-afb5-10d287897950)
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/0b2ce47c-3cdd-4960-b1cf-7a6afe0e3c3b)
- In our case we were supposed to find something similar to this > SELECT * FROM products WHERE category = 'Gifts' AND released = 1
- The URL matching closest to our select statement would be the one for corporate gifts
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/067984b7-5979-4082-a33e-ef9c7ac081d6)
- We can try to close that statement with quotes in which case it shows an internal server error
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/836fc43b-ddd9-41cd-a266-7e5fa2b8ac71)
- As we have now succesfully closed the old statement we can try to see if there is a vulnerability in the website by adding a simple statement of OR 1 = 1 -- after it and if there is a vulnerability it will show us all the info regarding the website database
- Why we use ' OR 1 = 1 -- is because 1 always equals to 1 and -- comments out the rest of the code
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/d19bfe53-b02e-4b05-94d9-cb3658cf8096)
- This ended up working and gave us access to all the items on the website
![image](https://github.com/Karoqnq/bite_spring2024_is/assets/112175331/708a2321-5a0e-438b-8f83-9be382472363)









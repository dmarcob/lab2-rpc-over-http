## Lab2 solution

To build, check and execute the server i've used these commands
respectively:  
```bash
    ./gradlew :server:build 
    ./gradlew :server:check
    ./gradlew :server:bootRun
```
I've used similar commands for the client:
```bash
    ./gradlew :client:build 
    ./gradlew :client:check
    ./gradlew :client:bootRun
```
To execute the system correctly we need to know these facts:  
  * Client only build succesfully if we've executed server previusly.  
  * We need to set java 11 as default version in our S.O. 
    In other case, the server wont be able to execute.
  
To configure github actions for tracking 'work' branch i've modified cy.yml file. I've added 'work' in 'branches' section.

Finally, in 'Server.kt' I've completed the endpoint returning a TranslationResponse object with translation atribute setted to "hola". 
 


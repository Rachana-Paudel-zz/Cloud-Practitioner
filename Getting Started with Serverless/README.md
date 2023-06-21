### Introduction to Serverless

+       Microservices
    +   Architectural and organizational approach to software development
    +   Software is composed of small independent services.
    +   Communicate over well-defined APIs.
    +   Owned by small, self-contained teams.

<img src="assets/microservice.PNG" alt="microservices" style="height:100%; width:100%">    

#####   Tightly versus loosely coupled
1.      Monolithic
    +   Tightly coupled
    +   In this application, if one piece were to fail, the entire application would crash, as this example illustrates. If there is a spike in demand, the entire architecture must be scaled. Adding features to a monolithic application becomes more complex as time goes on. Pieces of the code base must work with each other to sync properly.

<img src="assets/monolithic.PNG" alt="monolithic" style="height:100%; width:100%">    

2.      Microservices
<img src="assets/microservices2.PNG" alt="microservices" style="height:100%; width:100%"> 

<img src="assets/microservice architecture.PNG" alt="microservices" style="height:100%; width:100%">

#####   Benefits of microservices
+   use public APIs
<img src="assets/public api.PNG" alt="api" style="height:100%; width:100%">

+   use the right tool for the job
<img src="assets/right tool.PNG" alt="right tool" style="height:100%; width:100%">

+   secure your services
<img src="assets/secure services.PNG" alt="services" style="height:100%; width:100%">

+   be a good citizen
<img src="assets/good citizen.PNG" alt="good citizen" style="height:100%; width:100%">

+   company transformation
<img src="assets/company transformation.PNG" alt="transformation" style="height:100%; width:100%">

+   automate everything
<img src="assets/automate.PNG" alt="automate" style="height:100%; width:100%">

#####   Downside of monoliths
All processes are tightly coupled and run as a single service.
Adding or improving a monilithic application's features becomes more complex as the code base grows.
Dependent and tightly coupled processes increase the impact of a single process failure.

+       Serverless  
Build and run applications and services without thinking about servers.
<img src="assets/serverless.PNG" alt="serverless" style="height:100%; width:100%">

We can build them for nearly any type of application or backend service, and everything required to run and scale your application with high availability is handled for you.

+       Event driven architectures
+       Hybrid methods
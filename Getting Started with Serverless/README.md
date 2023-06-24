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
Developers can focus on their core product. 
Not worrying about managing and operating servers or runtimes.
<img src="assets/micro and serverless.PNG" alt="microservice" style="height:100%; width:100%">

#####   Benefits
1.   No server management
AWS founded the concept of serverless on the following principles:
When adapting a serverless service for building a serverless architecture, these ideals are fundamental to serverless strategy.

2.   Pay-for-value services
<img src="assets/pay.PNG" alt="pay-for-value" style="height:100%; width:100%">

3.   Continuous scaling
<img src="assets/scaling.PNG" alt="scaling" style="height:100%; width:100%">

4.   High availability
<img src="assets/availability.PNG" alt="scaling" style="height:100%; width:100%">

5.       Event driven architectures

<img src="assets/event.PNG" alt="event-driven" style="height:100%; width:100%">
<img src="assets/event driven.PNG" alt="event-driven" style="height:100%; width:100%">

##### Benefits
+       Scale and fail independently
    By decoupling your services, they are only aware of the event router, not each other. This means that your services are interoperable, but if one service has a failure, the rest will keep running. The event router acts as an elastic buffer that accommodates surges in workloads.
+       Audit with ease
    An event router acts as a centralized location to audit your application and define policies. These policies can restrict who can publish and subscribe to a router and control which users and resources have permission to access your data. You can also encrypt your events.
+       Develop with agility
<img src="assets/develop agility.PNG" alt="agility" style="height:100%; width:100%">    

+       Cut costs
<img src="assets/cut cost.PNG" alt="cut cost" style="height:100%; width:100%"> 

##### Serverless and non-serverless services work together
<img src="assets/serverless and nonserverless.PNG" alt="cut cost" style="height:100%; width:100%"> 

6.       Hybrid methods

### Introduction to Lambda
<img src="assets/intro to lambda.PNG" alt="lambda" style="height:100%; width:100%"> 

#####   Function configuration elements
+   Name
+   Description
+   Memory
+   Ephemeral Storage

#####   Some Lambda function triggers
+   S3 events
+   Amazon EventBridge
+   Amazon CloudWatch alarms
+   Other lambda functions

#####   AWS lambda function
<img src="assets/aws lambda function.PNG" alt="lambda" style="height:100%; width:100%">

#####   AWS lambda core components
<img src="assets/lambda core components.PNG" alt="lambda" style="height:100%; width:100%">

#####   Lambda function invoking
<img src="assets/lambda function invoking.PNG" alt="lambda" style="height:100%; width:100%">

#####   Types of invocation
+   Synchronous
<img src="assets/synchronous invoking.PNG" alt="lambda" style="height:100%; width:100%">

+   Asynchronous
<img src="assets/asynchronous invoking.PNG" alt="lambda" style="height:100%; width:100%">

+   Polling
<img src="assets/polling.PNG" alt="lambda" style="height:100%; width:100%">

### Execution environment lifecycle
<img src="assets/execution lifecycle.PNG" alt="lambda" style="height:100%; width:100%">

<img src="assets/execution1.PNG" alt="lambda" style="height:100%; width:100%">

<img src="assets/execution2.PNG" alt="lambda" style="height:100%; width:100%">

<img src="assets/execution3.PNG" alt="lambda" style="height:100%; width:100%">

### Cold and warm starts
<img src="assets/cold and warm starts.PNG" alt="lambda" style="height:100%; width:100%">

#####   Event source

<img src="assets/event source.PNG" alt="lambda" style="height:100%; width:100%">
<img src="assets/event source2.PNG" alt="lambda" style="height:100%; width:100%">
<img src="assets/event source eg.PNG" alt="lambda" style="height:100%; width:100%">

#####   AWS lambda permission
<img src="assets/aws lambda permission.PNG" alt="lambda" style="height:100%; width:100%">

### Identifying limits
<img src="assets/identify limits.PNG" alt="lambda" style="height:100%; width:100%">

+   memory
<img src="assets/limit1.PNG" alt="lambda" style="height:100%; width:100%">

+   timeout
<img src="assets/limit2.PNG" alt="lambda" style="height:100%; width:100%">

+   Concurrency
<img src="assets/limit3.PNG" alt="lambda" style="height:100%; width:100%">

#####   AWS lambda use cases
+   Web applications
    It includes
    +   static websites
    +   Complex web applications
    +   packages for flask and express
    +   built-in-https endpoints for single-function microservices

+   Backends: includes applications and services, mobile, IOT

+   Data processing: includes real-time processing, MapReduce

+   Chatbots: An example of chatbot use case would be powering chatbot logic.

+   Amazon Alexa: includes powering voice-activated application, alexa skills kit

+   IT automation: Policy engines, extending AWS services, Infrastructure management

#####   Pricing
<img src="assets/pricing.PNG" alt="lambda" style="height:100%; width:100%">


### Preparing to work with Lambda
Coding experience and expertise in the following domains.
+   Linux OS and commands
+   Security services and concepts
+   Cloud concepts and IP networking
+   Distributed computing concepts.

<img src="assets/preparing to work with lambda.PNG" alt="lambda" style="height:100%; width:100%">

#####   Three ways to build an AWS Lambda function
<img src="assets/way to build lambda function.PNG" alt="lambda" style="height:100%; width:100%">

#####   Function basic information
<img src="assets/function basic.PNG" alt="lambda" style="height:100%; width:100%">

#####   Handler method
<img src="assets/handler method.PNG" alt="lambda" style="height:100%; width:100%">

1.      Event handler
<img src="assets/event handler.PNG" alt="lambda" style="height:100%; width:100%">

<img src="assets/context object.PNG" alt="lambda" style="height:100%; width:100%">

#####   Design best practices
+   Separate bussiness logic
Separate your core bussiness logic from the handler event.
This makes your code more portable, and you can target unit tests on your code without worrying about the configuration of the function.

+   Modular functions
It will reduce the amount of time that it takes for your deployment package to download and unpack before invocation. Instead of having one function tha does compression, thumbnailing, and indexing, consider having three different functions that each serve a single purpose. 
Follow same principles you would apply to developing microservies.

+   Treat function as stateless
<img src="assets/treat function.PNG" alt="lambda" style="height:100%; width:100%">

+   Only include wha you 
<img src="assets/include needed.PNG" alt="lambda" style="height:100%; width:100%">

#####   Best practices of writing code
+   Include logging statements
<img src="assets/log statement.PNG" alt="lambda" style="height:100%; width:100%">

+   Use return coding
<img src="assets/return coding.PNG" alt="lambda" style="height:100%; width:100%">

+   Provide environment variables
<img src="assets/provide variable.PNG" alt="lambda" style="height:100%; width:100%">

+   Add secrets and reference data
<img src="assets/add secrets.PNG" alt="lambda" style="height:100%; width:100%">

+   Avoid reccursive code
<img src="assets/avoid recursive.PNG" alt="lambda" style="height:100%; width:100%">

+   Gather metrics with Amazon CloudWatch
<img src="assets/gather metrics.PNG" alt="lambda" style="height:100%; width:100%">

+   Reuse execution context
<img src="assets/reuse execution.PNG" alt="lambda" style="height:100%; width:100%">

#####   Configuration memory and timeout
<img src="assets/configuration memory.PNG" alt="lambda" style="height:100%; width:100%">
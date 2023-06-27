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

2. Context object
<img src="assets/context object.PNG" alt="lambda" style="height:100%; width:100%">

#####   Design best practices
+   Separate business logic
Separate your core business logic from the handler event.
This makes your code more portable, and you can target unit tests on your code without worrying about the configuration of the function.

+   Modular functions
It will reduce the amount of time that it takes for your deployment package to download and unpack before invocation. Instead of having one function tha does compression, thumbnailing, and indexing, consider having three different functions that each serve a single purpose. 
Follow same principles you would apply to developing microservies.

+   Treat function as stateless
<img src="assets/treat function.PNG" alt="lambda" style="height:100%; width:100%">

+   Only include what you 
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

+   Avoid recursive code
<img src="assets/avoid recursive.PNG" alt="lambda" style="height:100%; width:100%">

+   Gather metrics with Amazon CloudWatch
<img src="assets/gather metrics.PNG" alt="lambda" style="height:100%; width:100%">

+   Reuse execution context
<img src="assets/reuse execution.PNG" alt="lambda" style="height:100%; width:100%">

#####   Configuration memory and timeout
<img src="assets/configuration memory.PNG" alt="lambda" style="height:100%; width:100%">

#####   Configuring timeout
<img src="assets/configuring timeout.PNG" alt="lambda" style="height:100%; width:100%">

#####   Configuring concurrency and scaling
<img src="assets/configure concurrency.PNG" alt="lambda" style="height:100%; width:100%">

1.  Reserved concurrency
It guarantees the maximum number of concurrent instances for the function. When a function has reserved concurrency, no other function can use that concurrency. There is no charge for configuring reserved concurrency for a function.

2.  Provisioned
It initializes a requested number of execution environments so that they are prepared to respond immediately to your function's invocations. Note that configuring provisioned concurrency incurs charges to your AWS account.

#####   Destination and types
+   A destination can send records of asynchronous invocations to other services.
+   Configure separate destinations for events that fail processing and for events that process successfully.
+   Configure destinations on a function, a version, or an alias.
+   Address errors and successes without needing to write more code.

<img src="assets/destination and types.PNG" alt="lambda" style="height:100%; width:100%">

1.  Success
<img src="assets/success.PNG" alt="lambda" style="height:100%; width:100%">

2.  Failure
<img src="assets/failure.PNG" alt="lambda" style="height:100%; width:100%">

### Types of monitoring graphs
1.  Invocations
This graph includes the number of times that your function code is run, including successful runs and runs that result in a function error. If the invocation request is throttled or otherwise resulted in an invocation error, invocations aren't recorded.

2.  Duration
This shows the amount of time that your function code spends processing an event. The billed duration for an invocation is the value of duration rounded up to the nearest millisecond.

3.  Errors
This includes number of invocations that result in a function error. Function errors include exceptions thrown by your code and exceptions thrown by the Lambda runtime. The runtime returns errors for issues such as timeouts and configuration errors.

4.  Throttles
This shows number of times that a process failed because of concurrency limits. When all function instances are processing requests and no concurrency is available to scale up, Lambda rejects additional requests.

5.  IteratorAge
This pertains to event source mappings that read from streams. This shows the age of the last record in the event. The age is the amount of time between when the stream receives the record and when the event source mapping sends the events to the function.

6.  DeadLetterErrors
For asynchronous invocation, this is the number of times Lambda attempts to send an event to a dead-letter queue but fails.

7.  Concurrent Executions
<img src="assets/concurrent execution.PNG" alt="lambda" style="height:100%; width:100%">

### Amazon CloudWatch Lambda Insights
<img src="assets/lambda insight.PNG" alt="lambda" style="height:100%; width:100%">

### Lambda Insights Dashboard
<img src="assets/insight dashboard.PNG" alt="lambda" style="height:100%; width:100%">

### Monitoring using AWS X-Ray
<img src="assets/AWS X-ray.PNG" alt="lambda" style="height:100%; width:100%">

### AWS Serverless Service
<img src="assets/SQS.PNG" alt="lambda" style="height:100%; width:100%">

#####   Amazon SQS benefits
+   Fully managed messaging queue
+   Loosely coupled
+   High volume capabilities
+   Fault tolerance

#####   Achieving loose coupling with Amazon SQS
+   Use asynchronous processing to get your responses from each step quickly.
+   Handle performance and service requirements by increasing the number of job instance.
+   Exception or transaction failure, the order processing can be retried.

#####   Amazon SQS queue types
+   Standard
<img src="assets/standard queue.PNG" alt="lambda" style="height:100%; width:100%">

+   FIFO
<img src="assets/fifo queue.PNG" alt="lambda" style="height:100%; width:100%">

#####   Amazon SQS use cases
<img src="assets/sqs usecase.PNG" alt="lambda" style="height:100%; width:100%">

#####   Amazon Simple Notification Service (Amazon SNS)
<img src="assets/sns.PNG" alt="lambda" style="height:100%; width:100%">

#####   Amazon SNS subscription types
1.  Email
Messages are sent to registered addresses as email.
Email-JSON sends notifications as a JSON objects, while email sends text-based email.

2.  Mobile text messaging(SMS)
Messages are sent to registered phone number as SMS text messages.

3.  HTTP/HTTPS
Subscribers specify a URL as part of the subscription registration. Notifications will be delivered through an HTTPS POST to the specified URL.

4.  Amazon SQS
Users can specify an SQS standard queue as the endpoint. Amazon SNS will enqueue a notification message to the specified queue.
Note that FIFO queues are not currently supported.

5.  AWS Lambda
Messages can also be delivered to AWS Lambda functions for handling message customizations, enabling message persistence or communicating with other AWS service.

### Amazon SNS characteristics
<img src="assets/sns character.PNG" alt="lambda" style="height:100%; width:100%">

+   Single published message
All notification message contain a single published message. Amazon SNS attempts to deliver messages from the publisher in the order they were published into the topic. However, network issues could potentially result in out-of-order messages at the subscriber end.

+   No recall options
When a message is delivered successfully, there is no way to recall it.

+   HTTP or HTTPS retry
<img src="assets/http retry.PNG" alt="lambda" style="height:100%; width:100%">

+   Order and delivery not guaranteed
<img src="assets/order.PNG" alt="lambda" style="height:100%; width:100%">

### Amazon SNS use cases
<img src="assets/sns usecase.PNG" alt="lambda" style="height:100%; width:100%">

### Amazon SNS and Amazon SQS differences
<img src="assets/sns and sqs.PNG" alt="lambda" style="height:100%; width:100%">

### Serverless characteristics of S3
1.  Pay for value
<img src="assets/pay for value.PNG" alt="lambda" style="height:100%; width:100%">

2.  Elastic storage
<img src="assets/elastic storage.PNG" alt="lambda" style="height:100%; width:100%">

3.  Continuous scaling
<img src="assets/continous scaling.PNG" alt="lambda" style="height:100%; width:100%">

4.  Fault tolerance
<img src="assets/fault tolerance.PNG" alt="lambda" style="height:100%; width:100%">

5.  No server management
<img src="assets/never management.PNG" alt="lambda" style="height:100%; width:100%">

### Lambda@Edge
<img src="assets/lambda@edge.PNG" alt="lambda" style="height:100%; width:100%">

### Amazon API Gateway
<img src="assets/api.PNG" alt="lambda" style="height:100%; width:100%">

### API Gateway use case
<img src="assets/api usecase.PNG" alt="lambda" style="height:100%; width:100%">

### AWS Fargate
<img src="assets/fargate.PNG" alt="lambda" style="height:100%; width:100%">

### Container
<img src="assets/container.PNG" alt="lambda" style="height:100%; width:100%">
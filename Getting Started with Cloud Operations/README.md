# Getting Started with Cloud Operations
### This is the begining of cloud practitioner journey.
We begin our journey from AWS educate course. Click [Getting Started with Cloud Operations](https://awseducate.instructure.com/courses/889) to start learning.

## Objectives
By the end of this course you will be able to do the following:

+      Describe cloud operation fundamental concepts.

+      Explain the Amazon Well-Architected Framework.

+      Describe AWS cost and free tier structures.

+      Describe the AWS cost management tools that are available.

+      Identify support plans and explain the differences between them.

+      Discuss AWS cloud operations services that are available to you, including AWS Trusted Advisor, AWS Health  Dashboard, Amazon CloudWatch, AWS CloudTrail, AWS Organizations, AWS Systems Manager, and AWS Config.

## Getting Started learning pathway
This is a course that’s a part of a series of courses designed to give you foundational knowledge about cloud computing.  
Each of the courses are focused on a specific domain of cloud computing.

Although you can take any of the courses at any time, we suggest that you take the courses in the following order:

1. Getting Started with Storage
2. Getting Started with Compute
3. Getting Started with Networking 
4. Getting Started with Databases 
5. Getting Started with Cloud Operations 
6. Getting Started with Security 
7. Getting Started with Serverless   

## Learning
<img src="assets/Learning_Module1.png" alt="Guide Video" style="height: 100%; width:100%;"/>

## Getting Started with Cloud Operations Lab  
This hands-on lab guides you through the steps to estimate Amazon Web Services (AWS) costs for a sample workload. The workload that you evaluate is for a three-tier web application that consists of :  
+       An Application Load Balancer  
+       An Amazon Elastic Compute Cloud (Amazon EC2) instance  
+       An Amazon Relational Database Service (Amazon RDS) instance 

The skills will help you to use AWS Pricing Calculator to estimate costs for your workloads.

###     Introduction to the Well-Architected Framework
<b>Cloud Environment</b>

+   Security
+   Operation
+   Performance
+   Scalability
+   Cost


### What is cloud operations?
+   Innovation
+   Cost
+   Compliance
+   Security


### Benefits of Cloud Operations
+       Innovation
    AWS helps you use the cloud to turn ideas into opportunities, creating new ways to grow, increase efficiency, and serve customers better. AWS has industry leading cloud services to help customers solve problems and explore possibilities.

+       Scale
    AWS management and governance services are built to manage highly dynamic cloud resources at massive scale.

+       Simplicity
    AWS reduces complexity, offering a single control plane for customers to manage and govern their resources on AWS and on-premises.

+       Cost savings
    Customers can use AWS management and governance services to assess their resource utilization and identify ways to reduce costs.

### AWS WA Framework Introduction
Foundation should be strong    
<img src="assets/WA intro.PNG" alt="WA" style="height:100%; width:100%">

### WA Framework pillars
<img src="assets/pillar.PNG" alt="pillar" style="height:100%; width:100%">

### AWS WA Framework: six pillars
+       Operational excellence
    The operational excellence pillar focuses on running and monitoring systems and continually improving processes and procedures. Key topics include automating changes, responding to events, and defining standards to manage daily operations.
    
+       Security
    The security pillar focuses on protecting information and systems. Key topics include confidentiality and integrity of data, managing user permissions, and establishing controls to detect security events.

+       Reliability
    The relaibility pillar focuses on workloads performing their intended function and how to recover quickly from failure to meet demands. Key topics include distributed system design, recovery planning, and adapting to changing requirements.

+       Performance efficiency
    This pillar focuses on structured and streamlined allocation of IT and computing resources. Key topics include selecting resource types and sizes optimized for workload requirements, monitoring performance, and maintaining efficiency as business need evolve.

+       Cost optimization
    The cost optimization pillar focuses on avoiding unnecessary costs. Key topics include understanding spending over time and controlling fund allocation, selecting resources of the right type and quantity, and scaling to meet business needs without overspending.
+       Sustainability












## LAB:
### Getting Started with Cost Estimation
#### 1. AWS Pricing Calculator
+ Launch [AWS Pricing Calculator](https://calculator.aws/#/) and begin to <strong>Create an estimate.</strong>  
<img src="assets/aws_calculator.png" alt="AWS Pricing Calculator" style="height: 100%; width:100%;"/>

#### 2. Add and configure services in AWS Pricing Calculator 
+   <b><u>Add the load balancer to the estimate</u></b>  
    a.  On the Select service page, in the Find Service search box, enter `Elastic Load Balancing` and configure it. <small><u><i>[Learn to configure](https://awseducate.instructure.com/courses/889/modules/items/15053)</i></u></small>.

<img src="assets/Configure_ELB.PNG" alt="Configure ELB" style="height: 100%; width:100%;"/>

+   <b><u>Add the EC2 instance to the estimate</u></b>  
    a.  On the Select service page, in the Find Service search box, enter `EC2` and configure it. <small><u><i>[Learn to configure](https://awseducate.instructure.com/courses/889/modules/items/15053)</i></u></small>.

<img src="assets/Configure_EC2.PNG" alt="Configure EC2" style="height: 100%; width:100%;"/>

+   <b><u>Add the RDS instance to the estimate</u></b>  
    a.  On the Select service page, in the Find Service search box, enter `RDS` and configure it. <small><u><i>[Learn to configure](https://awseducate.instructure.com/courses/889/modules/items/15053)</i></u></small>.

<img src="assets/Configure_RDS.PNG" alt="Configure RDS" style="height: 50%; width:45%; padding-right:10px"/>

<img src="assets/Configure_RDS2.PNG" alt="Configure RDS" style="height: 50%; width:45% ;"/>

#### 3. Review and download the estimate

+   <b><u>Choose View summary.</u></b>  
    a.  Review the overall costs that AWS Pricing Calculator generated for the services from the My Estimate page. enter `Review Summary` and configure it. <small><u><i>[Learn to configure](https://awseducate.instructure.com/courses/889/modules/items/15053)</i></u></small>.

    <img src="assets/View_Summary.PNG" alt="Summary" style="height: 100%; width:100%;"/>

  
    ##### Note: The prices found in your estimate may vary as prices occasionally change. 

    + Choose Export, and then choose CSV.
    + In the Export My Estimate to csv dialog box, choose OK.
    + Use your local file explorer to save the file.  

#### 4. Save and share the estimate
+ Choose Share.

+ In the Save estimate dialog box, choose Agree and continue.

+ To copy the link for your estimate, choose Copy public link.

+ To share the estimate, send the link to others using a communication tool such as email.

Note: When you share an estimate, AWS Pricing Calculator automatically saves it and generates a URL to access it. AWS Pricing Calculator saves your estimate for 3 years.

<i>[Learn more ...](https://awseducate.instructure.com/courses/889/modules/items/15053)</i>

##### `LAB COMPLETE and Quiz starts`
#### End of Cloud Operations


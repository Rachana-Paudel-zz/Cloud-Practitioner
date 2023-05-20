### Getting started with Security

####    In this module
+   Introduction to security
+   Introduction to AWS IAM
+   Using IAM
+   Additional AWS Security Services

####    IT security

<img src="assets/IT security1.PNG" alt="security" style="height:100%; width:100%;">

<img src="assets/IT security2.PNG" alt="security" style="height:100%; width:100%;">

####    Principle of least privilege

<img src="assets/privilege1.PNG" alt="privilege" style="height:100%; width:100%;">

<img src="assets/privilege2.PNG" alt="privilege" style="height:100%; width:100%;">

<img src="assets/privilege3.PNG" alt="privilege" style="height:100%; width:100%;">
 
####    Identity and access management
   working sessions can have thousands of users that will need different level of permissions, therefore this need to be carefully managed.

   To do this organization should use IAM.
   <img src="assets/IAM.PNG" alt="IAM" style="height:100%; width:100%;">

####    Authentication and authorization
1.      Authentication
    It is a basic computer security concept: a user or system must first prove their identity. Consider how you authenticate yourself when you go to the airport and you want to get through airport security so that you can catch your flight. In this situation, you must present some form of identification to the security official to prove who you are before you can enter a restricted area. A similar concept applies for gaining access to IT resources.

2.      Authorization
    It is the process of determining what permissions a user should be granted. After a user has been authenticated, they must be authorized to access the IT resource or data that they are requesting.    

<b> Authentication and authorization together</b>

    First, user enter username and password. The username and password are verified by database. If the entered password or username does not match then user return to login again. If entered information matches authentication is completed. After this the authorization process determine permission the user has to the applications.

<img src="assets/aa.PNG" alt="security" style="height:100%; width:100%;">

### Layers of security
IT security starts with protecting physical data center then actual data files. The forming layer of IT security are:
+   Perimeter layer
    +   Building:  
    Aws data centers are housed in nondescript, undisclosed facilities. They are protected by a number of security features such as security guards, fencing, security feeds, and other security measures.

    +   Surveillance:
    Professional security staff use video surveillance, intrusion detection, access log monitoring systems and other electronic means. Entrances are secured with devices that sound alarms if a door is forced or held open.

    +   Employee scrutinization:
    Only AWS employees who routinely need access are given permissions to relevant areas of the facility based on job function. If an employee doesn't have an ongoing bussiness need to be at a data center, they have to go through the visitor process and have an escort assigned throughout the duration of their visit.

    +   Principle of least privilege:
    AWS limits access to  pre-approved areas and only provides data center access to employees and contractors who have a legitimate business need for such privileges.


+       Environment layer
    +   Mitigate environmental risks:
    AWS carefully chooses their data center locations to mitigate environmenal risks like flooding, extreme weather, and seismic activity.

    +   High availability and performance:
    Customers requiring high availability and performance can deploy their applications across multiple Availability Zones in the same region. This provides lower latency, reduced costs and data compliance, while opening up the potential to engineer for fault tolerance.

    +   AWS bussiness continuity testing
    To mitigate and prepare for the unexpected, AWS tests their business Continuity Plan regularly with drills that simulate different scenarios.

    +   Energy saving:
    Companies generally use 77% fewer servers, 84% less power, and tap into a 28% cleaner mix of solar and wind power in the AWS Cloud versus their own traditional data centers.

+       Infrastructure layer
    +   Fire detection:
    Automatic fire detection and suppression equipment reduces the risk of fire-related accidents. Smoke detection sensors are in all data center environments, mechanical and electrical spaces, chiller rooms and generator equipment rooms.

    +   Monitoring:
    AWS monitors electrical, mechanical and life support systems. Preventive maintenance is regularly performed.

    +   Climate control:
    It is uded to maintain a constant operating temperature for servers and other hardware. This prevents overheating and reduces the possibility of service outages.

    +   Power:
    Electrical systems are fully redundant and maintainable without impact power for critical and essential loads and generators provide backup power for the entire facility.

+   Data layer
<img src="assets/data layer.PNG" alt="security" style="height:100%; width:100%;">
    
####    AWS Shared Responsibility
<img src="assets/shared responsibility1.PNG" alt="security" style="height:100%; width:100%;">
<img src="assets/shared responsibility2.PNG" alt="security" style="height:100%; width:100%;">
<img src="assets/shared responsibility3.PNG" alt="security" style="height:100%; width:100%;">
Examples
<img src="assets/shared responsibility4.PNG" alt="security" style="height:100%; width:100%;">


####    Intoduction to Amazon S3

#####   Getting started with AWS Identity and Access Management(IAM)

#####   IAM credentials types
User is given access to <b>AWS Management Console<b> and <b>Programmatic access</b>
For AWS Managemen Console user is given username and password and for programmatic access user is given access key.

1.      AWS Management Console:
<img src="assets/aws management console.PNG" alt="security" style="height:100%; width:100%;">

2.      Programmatic access:
<img src="assets/programmatic console.PNG" alt="security" style="height:100%; width:100%;">

####    Multi-factor authentication(MFA)
<img src="assets/mfa.PNG" alt="security" style="height:100%; width:100%;">

<img src="assets/mfa2.PNG" alt="security" style="height:100%; width:100%;">
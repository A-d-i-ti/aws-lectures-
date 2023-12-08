# aws-lectures-
everything to know about aws -beginners 

## what is cloud computing ?!
- cloud computing is the delivery of computing services -
- including servers ,storage,databases,networking, software ,analytics and intelligence - over the internet ('the cloud ')
- offer faster innovation ,flexible resources and economies of scale .
  
### Benefits of cloud computing :
- faster time to market 
- scalable and flexible
- cost saving
- better collaborations
- advanced security
- data loss prevention

### Disadvantages of using cloud 
 - risk of vendor lock in
 - less control over underlying cloud infrastructure
 - intergration complexity with existing system
 - concerns about security risks like data privacy
 - unforeseen costs and unexpected expenses

- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/09c65ee7-6035-4c3f-bf7b-490bf41c2520)
- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/efad10f0-ba59-4e69-8594-ee7d2cff1952)

- cloud service models :
- Iaas : Infrastructure as a service
- Paas : Platform as a service 
- Saas : Software as a service
- 
- 

## **Amazon Web Services (AWS)**
- is the world's most comprehensive and broadly adopted cloud platform, offering over 200 fully featured services from data centers globally.
-  Millions of customers - including the fastest-growing startups, largest enterprises, and leading government agencies are using AWS to lower costs, become more agile, and innovate faster

-  ### Compute services
-  Elastic compute cloud -EC2
-  ECS/EKS - containerized servies (for linux)
-  Lambda - Serverless
  ### Storage services 
 - Simple storage services -S3
 - Elastic Block Store -EBS
 - Elastic File System - EFS
 - Archival Services - Glacier

 - creating S3 bucket :
 - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/cae38cad-03ab-4775-93c9-7bba4b72bab6)

  
## Diff btw block storage and object storage 
#### Block storage - storage that can be formatted at a later point of time , associated/ attached with os ,so os formats this storage acc to its convinence .
- Eg -- EBS (elastic block storage)provides volume that can be attached with our EC2 instances .
- Some formatting technique - ext3,ext4  NTFS , stfs, Fat32 
#### Object storage - cannot be formatted , keep our file ,stores movie file , multimedia content,
- Eg- S3 (simple storage services )- we can make bucket and store , authentication, authorisation - roles can be controlled and assign bucket uses.
- **San - storage area network (hardware )**, provide logical unit numbers (luns )  integrated with the os , can be formatted and kevilished as the hard disk 
- Network attached storage.(NAS) 
- RAID - Redandent array of independant disk , it started with raid 0 - mirroring - same data into two disc ,slow 
+ Raid-1 : slicing - half data in one other half in another 
+ Raid- 01 : mirroring then slicing 
+ Raid -10 : SLICING THEN mirroring. 
+ Raid 10/01 - req 4 disc 
+ Raid 5 : best ,used 3 disc ,1 dic perity (ie .if any one dic is killed , data can still be accessed with other 2 disc ) 
- Ios - input output per sec 
- **Elastic file system (EFS)**: only works with Linux , 
- Archival services  Glaciers - cheapest  storage, stores data that is not required at urgent need ime real time , takes time to reload data probably one day .
### Network Services 
- Virtual private cloud -(vpc) provided on a hyperscaler  ,uses private ip
- Domain Name Services - Route 53
- Direct connect 
###
- sqs- quequing service
- bracket-
- code build -is a build tool ,used for those languages which needs compilation
- rds
- cloud trail- auditing of your aws account 
- sns- notification service
- code commit - managed service of git taken over by aws
- aws comprehend - tells which kind of text it is,the sentiments of the text ..whether optimistic eg: customer care
- amazon polly -converts text to spoken language
- amazon lex - converts spoken words to text
- text track - optical character recorginisation (ocr),

### load balancer : implementation of horizontal scaling , required for high availability 
- type of load balancer :
- 1. classical load balancer - layer 4&7
  2. application load balancer - layer 7
  3. network load balancer - layer 4

  layer 7 - load balancer
  tls= transport layer security 
 - amazon linux - red hat
 - ubuntu - debian

 - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/8883a73f-a64f-4709-bd1a-2295842e33f9)

 - connection -SSH  using putty : 
 - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/ca6a11ed-f933-4a80-b4da-d613fc32e6bb)

 -####  installing nginx
 - sudo su;
 - sudo update ;
 - apt install nginx ;
 - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/0148a789-31d2-4d7b-81d9-6e8c5eaaf4a1)

### creating load balancer 
##### creating target group :
-![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/3d8a5f86-8587-4688-8a1e-3abad9184d0e)
-![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/f1894d00-a6a0-41c7-8a58-b6e08067de8f)


- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/d7c285ba-eec5-453e-9315-26b775498301)


  ### autoscaling :
  - self-healing implementation for dynamic load
  - can create and terminate instances automaticallu
  - manual scaling :
  - auto scaling grp
  - launch template- what kind of instance to be generated 
  - alarm : information after a certain threshold 
 
- Cloud watch : monitoring service ,provides system level monitoring by default ;hardware basically not application

- creating a launch template :
- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/f38d43e9-ba27-4b25-86b5-dfd7aa5828a0)

- creating auto scaling :
- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/cccdc48f-8362-4421-8697-ce8a6cb6d519)

- creating an alarm :
- autoscaling--- monitoring --ec2-- cpu ---bell icon 
-![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/08dc811f-2ea9-43a8-94e2-f2720d7bd64d)

- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/d71525b6-3be6-46f2-9a49-60a826af438c)

- a dynamic scaling policies created: 
- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/575a66a9-9b13-46a8-b493-74c702b98912)


### vpc: virtual private cloud 
- private isolated network to deploy your resources
- SUBNETs allow to partition your netwok within VPC - encrypted tunnel
- type of subnet :
   + private - cannot recieve traffic from outer world [internet]
   + public - accessible from the internet
- route table -
- **Internet gateway : IGW ** helps our vpc instance connect with internet
- **NAT GATEWAY : self managed **

- ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/dc1996f0-5aba-47b6-8c99-2fc63b552ec8)

- Cidr - classless interdomain routing 
Way of representation,we don't use net mass ,just represent using number based

-![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/cf026c4a-8117-4859-a3de-ea585dfa908f)

+ **Blue green deployment** -we can make zero down time deployment eg: any new update in the application is to be deployed. 
+ **Canery deployment**- create new architecture, already have old architecture..phase wise deployment..eg: what'sapp polling feature.
+ ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/ef81c83a-1a49-4d16-8207-e5de3684f9c1)

+ Failure over startegy -
1 . active -passive failover startegy
  -![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/6d034926-416f-4892-a408-66109b0ff94e)
  #### Creating cloudformation:
  --- creating role for cloud formation :
  - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/8052cdfe-fafc-4da8-9ebf-335d8bc02ad0)
  - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/9051df29-0780-428e-bb5f-6bb0805aab52)
 
  - ![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/6ced931d-7c3d-43a6-9bee-e2e3b9aac9c3)



  -![image](https://github.com/A-d-i-ti/aws-lectures-/assets/142913419/5eb10c11-2b68-4fa6-8f62-e0200050b3e1)

- **Containers**,- just like vm but don't have their own kernal ,they use kernal of the host 
- They are light weight 
- **Containerisation -** development to production directly without deployment.
- C group - give ability to control the resources.
Eg . giving 2 GB ram ..so only 2 GB is deployed is checked by c group .
- Namespace -

- - **Cloud 9 :**
- cloud based -ide ,integrated development environment , that lets us - write ,run ,debug our code with juat a browser
- code editor,debugger, terminal 
- - **Pod Limit :**
  - maximum number of pod allowed in an EC2 instance 
###   EKS MANAGEMENT Nodegroup :
- create and manages EC2
- automated 





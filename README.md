# aws-lectures-
everything to know about aws -beginners 

## what is cloud computing ?!
- cloud computing is the delivery of computing services -including servers ,storage,databases,networking, software ,analytics and intelligence - over the internet ('the cloud ')
to offer faster innovation ,flexible resources and economies of scale .
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
-  Elastic compute services -EC2
-  ECS/EKS - containerized servies (for linux)
-  Lambda - Serverless
  ### Storage services 
 - Simple storage services -S3
 - Elastic Block Store -EBS
 - Elastic File System - EFS
 - Archival Services - Glacier
  
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

# aws-lectures-
everything to know about aws -beginners 

## what is cloud computing ?!
- cloud computing is the delivery of computing services -including servers ,storage,databases,networking, software ,analytics and intelligence - over the internet ('the cloud ')
to offer faster innovation ,flexible resources and economies of scale .
### Benefits of cloud computing :
- faster time to market 
-scalable and flexible
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
- Virtual private cloud -(vpc) provided on a hyperscaler  ,uses private ip
- 

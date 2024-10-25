# AWS S3 important points:



## S3 use cases:

    Backup purposes

    Disaster recovery 

    Archiving files

    hybrid cloud storage

    Application hosting

    Media hosting

    Data Lakes and big data analytics

    Software deliviry 

    Static websites

### Bucket features:

    It can be created for a specific region

    The Data are stored in Key and value pairs , to be remember it is not working in the concepts of directories

    Key - path to the file in s3

    value - data stored in that file

    Max-size - (5TB) if size > TB => do multi-part upload

### Security:

    User-Based : Via Iam Policies

    Resoure-Based: 

        Bucket-policies : applicable to cross accounts

        Object Access control List : Fine Grain
 
        Bucket Access Control list : Less common  

### Versioning:

    Before enabling Versioning:

    In current Bucket : file 1

    after modification of the file 1 : It gets overwritten

    after deletion operation of the file 1 : It gets permanently deleted

    After Enabling Versioning:

    In current bucket : file1

    after modification of the file 1 : New file with the Particular version Id got added

    after deletion operation of the file 1 :same file will be stored as type of delete mark - version id

### S3 replication:

    -->CRR = Cross region replication -- asynchronous repliaction -- Lower latency

    -->SRR = same region replication -- live replication

    Replicates only when the replication is on

    if you want to replicate the older files you want to use s3 batch replications

    

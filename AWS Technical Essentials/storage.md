Storage Types
--------------

Block storage - While file storage treats files as a singular unit, block storage splits files into fixed-size chunks of data called blocks that have their own addresses. 


Object storage - Objects, much like files, are treated as a single unit of data when stored. However, unlike file storage, these objects are stored in a flat structure instead of a hierarchy. Each object is a file with a unique identifier. This identifier, along with any additional metadata, is bundled with the data and stored.

Amazon Elastic Block Storage (Amazon EBS)
-------------------------------------------

Volume Types : 
 * EBS Provisioned IOPS SSD, 4 GB – 16 TB, 64 000
 * EBS General Purpose SSD, 1 GB – 16 TB, 16000 IOPS
 * Throughput Optimized HDD, 500 GB – 16 TB, 500 IOPS
 * Cold HDD, 500 GB – 16 TB, 250 IOPS


S3 bucket policies
--------------------

Like IAM policies, Amazon S3 bucket policies are defined in a JSON format. The difference is IAM policies are attached to users, groups, and roles, whereas S3 bucket policies are only attached to S3 buckets. S3 bucket policies specify what actions are allowed or denied on the bucket.

S3 bucket policies can only be placed on buckets, and cannot be used for folders or objects. However, the policy that is placed on the bucket applies to every object in that bucket.

S3 Versioning states
---------------------

Buckets can be in one of the following three states:

Unversioned (default): No new and existing objects in the bucket have a version.
Versioning-enabled: Versioning is enabled for all objects in the bucket.
Versioning-suspended: Versioning is suspended for new objects. All new objects in the bucket will not have a version. However, all existing objects keep their object versions


Six Amazon S3 storage classes
------------------------------

    * S3 Standard - S3 Standard offers high durability, availability, and performance object storage for frequently accessed data
    * S3 Intelligent-Tiering -  first cloud storage that automatically reduces your storage costs on a granular object level by automatically moving data to the most cost-effective access tier based on access frequency
    * S3 Standard-Infrequent Access - data that is accessed less frequently, but requires rapid access when needed.
    * S3 One Zone-Infrequent Access - for data that is accessed less frequently, but requires rapid access when needed. Unlike other S3 Storage Classes which store data in a minimum of three Availability Zones (AZs), S3 One Zone-IA stores data in a single AZ and costs 20% less than S3 Standard-IA
    * S3 Glacier Instant Retrieval - archive storage class that delivers the lowest-cost storage for long-lived data that is rarely accessed and requires retrieval in milliseconds 
    * S3 Glacier Deep Archive - is Amazon S3’s lowest-cost storage class and supports long-term retention and digital preservation for data that may be accessed once or twice in a year

S3 bucket encryption 
---------------------

    * Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3) 
    * Server-Side Encryption with Customer Master Keys (CMKs) Stored in AWS Key Management Service (SSE-KMS)
    * Server-Side Encryption with Customer-Provided Keys (SSE-C) 
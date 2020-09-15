
# AWS

---

# ToC

- [AWS](#aws)
- [ToC](#toc)
- [Products](#products)
  - [Region & AZ](#region--az)
  - [Create Instance](#create-instance)
  - [Products 1: Compute](#products-1-compute)
  - [AWS: EC2 vs Lightsail](#aws-ec2-vs-lightsail)
  - [Compute: Why use Elastic Beanstalk?](#compute-why-use-elastic-beanstalk)
  - [Compute: Notes on Elastic Beanstalk](#compute-notes-on-elastic-beanstalk)
  - [Products 2: Containers](#products-2-containers)
  - [AWS: Why use Fargate?](#aws-why-use-fargate)
  - [Products 3: Storage](#products-3-storage)
  - [S3 vs EFS vs EBS](#s3-vs-efs-vs-ebs)
    - [EFS](#efs)
    - [EBS](#ebs)
    - [S3](#s3)
  - [Products 4: Database](#products-4-database)
  - [ElastiCache](#elasticache)
    - [Engine](#engine)
    - [Purpose](#purpose)
  - [Products 5: Security, Identity & Compliance](#products-5-security-identity--compliance)
  - [Products 6: Cryptography & PKI](#products-6-cryptography--pki)
  - [Products 7: Machine Learning](#products-7-machine-learning)
  - [Products 8: Management & Governance](#products-8-management--governance)
  - [Why need ELB?](#why-need-elb)
  - [Types of ELB](#types-of-elb)
  - [Products 9: Developer Tools](#products-9-developer-tools)
  - [Products 10: Migration & Transfer](#products-10-migration--transfer)
  - [Products 11: Networking & Contents Delivery](#products-11-networking--contents-delivery)
  - [Products 12: Media Services](#products-12-media-services)
- [VPC](#vpc)
  - [AWS VPC: Features](#aws-vpc-features)
  - [AWS VPC: Keywords](#aws-vpc-keywords)
  - [AWS VPC Gateways](#aws-vpc-gateways)
  - [AWS Products: MISC](#aws-products-misc)
  - [AWS: Account](#aws-account)
- [EC2](#ec2)
  - [EC2: Setup](#ec2-setup)
    - [Ref](#ref)
  - [EC2: Amazon Linux](#ec2-amazon-linux)
    - [Types](#types)
  - [EC2: AMI](#ec2-ami)
    - [Create](#create)
  - [EC2 Instance Types: Category](#ec2-instance-types-category)
  - [EC2: Instance Types](#ec2-instance-types)
  - [EC2: Connect to instance](#ec2-connect-to-instance)
  - [AWS VPC: Config Example 1](#aws-vpc-config-example-1)
  - [AWS VPC: Config Example 2](#aws-vpc-config-example-2)
- [Deploy to EC2](#deploy-to-ec2)
  - [AWS + Laravel](#aws--laravel)
  - [AWS + Laravel (Elastic Beanstalk)](#aws--laravel-elastic-beanstalk)
    - [Ref](#ref-1)
  - [AWS + Laravel: Overview](#aws--laravel-overview)
  - [AWS + Laravel: References](#aws--laravel-references)
  - [AWS + Laravel: Set up PHP](#aws--laravel-set-up-php)
  - [AWS + Laravel: Set up Apache](#aws--laravel-set-up-apache)
  - [AWS + Laravel: Set up Postgres](#aws--laravel-set-up-postgres)
  - [AWS + Laravel](#aws--laravel-1)
- [RDS](#rds)
  - [RDS](#rds-1)
- [AWS + Gaming](#aws--gaming)
  - [w/o CloudFront](#wo-cloudfront)
  - [w/ CloudFront (then)](#w-cloudfront-then)
  - [w/ CloudFront (modern)](#w-cloudfront-modern)
  - [System Config](#system-config)

---

# Products

>>>

## Region & AZ

- Region:
  - __ap-northeast-1__ is for Tokyo
- AZ: Availability Zone
  - A region has multiple AZ, that is, data centers
  - A service can ber deployed to multiple AZs for redundancy
  - Comm between multiple regions: High latency
  - COmm between AZs inside the same region: Low latency
- For high availability:
  - Multi-AZs with Active-Passive / Active-Active

>>>

## Create Instance

1. Choose AMI
2. Choose an instance type
3. Configure the instance details
4. Add tags
5. Set up Security group
6. Start

>>>

## Products 1: Compute

- **EC2**: Elastic Compute Cloud
- Lightsail
  - Servers + Storage + DB + Networking. Cheap
- **Lambda**
  - Run the code triggered by the events
- Elastic Beanstalk
  - PaaS for PHP, Node, Python, Docker... etc.
- CodeStar
  - CD (Continuous Delivery) tool: quick build & deployment

>>>

## AWS: EC2 vs Lightsail

Lightsail is a good option for small websites, test / dev env, WordPress blog

- Lightsail is cheaper
  - Lightsail has monthly fixed cost, while EC2 cost is calc by usage
- Lightsail is all-in-one while EC2 is computing only
  - Storage, snapshot, LB, firewall, DNS, networking
  - With server snapshot functionality, you can duplicate the server easily
  - LAMP / MEAN/ Node.js env is pre-configured
  - Easy to host the website (incl. WordPress)
- EC2 is more customizable
  - Lightsail is highly pre-configured, and it can't be changed
  - Lightsail service can't be linked to other AWS services with ease
  - Lightsail can't be scaled according to the requests

>>>

## Compute: Why use Elastic Beanstalk?

- Automatically configure the programming language-specific env
  - e.g. PHP, Laravel, etc.
- Automatically configure the necessary AWS services:
  - EC2 Instance
  - Auto Scaling Group
  - Load Balancer
  - CloudWatch

>>>

## Compute: Notes on Elastic Beanstalk

- EC2 instance which is related to EB can't be stopped, seemingly
- EB service can't be halted; it must be terminated not to consume AWS resources.

>>>

## Products 2: Containers

- ECS: Elastic Container Service
- EKS: Elastic Kubernetes Service
- Fargate
  - Compute Engine for ECS / EKS
- ECR: Elastic Container Registry
  - Store of the Docker images

>>>

## AWS: Why use Fargate?

1. Build the container image 
2. Deploy EC2 instances (Fargate does this instead of you!)
3. Define memory resources
4. Isolate apps with VMs (Fargate does this instead of you!)
5. Run app

>>>

## Products 3: Storage

- **S3**: Simple Store Service
  - Cheap
- **EBS**: Elastic Block Store
  - Virtual hard disks
- EFS: Elastic File System


>>>

## S3 vs EFS vs EBS

### EFS

- EFS is NFS (Network File System)
- OSからマウントできる。S3はHTTPS経由でアクセス
- EC2にマウントできる（EBSと同じ）
- **複数のAZにまたがる大量のEC2 Instance**から同時にアクセス可
- **expensive**

### EBS

- EBS is Block Storage
- Mountable to EC2 (Same as EFS)
- **single AZ, single EC2 instance**
  - A EC2 instance can mount multiple EBSs, tho

### S3

- Object Storage
- Multi-AZ
- **cheap**

>>>

## Products 4: Database

- **RDS**: Relational Database Service
- DynamoDB
- ElastiCache
- RedShift
- AWS Aurora: RDB compatible with MySQL / PostgreSQL

>>>

## ElastiCache

### Engine
- Redis
- Memcached

### Purpose

- Data which will be accessed frequently
- Data which won't be updated frequently
- **session**, **DB cache**, etc.

>>>

## Products 5: Security, Identity & Compliance

- IAM: Identy & Access Management

>>>

## Products 6: Cryptography & PKI

>>>

## Products 7: Machine Learning

- SageMaker

>>>

## Products 8: Management & Governance

- **ELB**: Elastic Load Balancing
  - Application LB
  - Network LB
  - Classic LB
- **Auto Scaling**
- **CloudFormation**
  - Describe the AWS system config in JSON; sort of IaC?
- Systems Manager
  - incl. Parameters Store
- **CloudWatch**
- CloudTrail
  - Monitor the AWS Account activity
- (DataDog)
  - DataDog is provided by DataDog corp, not by AWS
  - Offer the console for the AWS monitoring services

>>>

## Why need ELB?

- ELB distributes the load to multiple servers
  - Smaller load to each server, higher usability
- ELB puts the server into a maintenance mode without stopping the entire service
  - Fault tolerent
- ELB monitors the health of the servers
- ELB manages the security group
  - You can get SSL certificate
- ELB scales according to traffic amount

>>>

## Types of ELB

- Application Load Balancer
  - High-spec
  - Layer 7: distribute HTTP / HTTPS
  - Can deal with container / micro-services
- Network Load Balancer
  - Millions of requests per sec
  - Layer 4: distribute TCP / UDP / TLS traffics
- Classic Load Balancer
  - Layer 7 & Layer 4


>>>

## Products 9: Developer Tools

>>>

## Products 10: Migration & Transfer

>>>

## Products 11: Networking & Contents Delivery

- CloudFront
  - CDN service: Static / dynamic contents will be delivered from the nearest server to the user
  - high speed delivery with cache: streaming is possible
- App Mesh
- Amazon Route 53
  - DNS service

>>>

## Products 12: Media Services

---

# VPC

>>>

## AWS VPC: Features

- VPC: Virtual Private Cloud
  - selection of your own IP address range
  - creation of subnets
  - configuration of route tables and network gateways
- Major combination
  - EBS (for permanet storage)
  - EC2 (for server software)
  - VPC (for network)
- A VPC can have multiple AZs

>>>

## AWS VPC: Keywords

- Subnet
  - Public Subnet
  - Private Subnet
- Route table
  - Define possible connections among internet / subnets
- Router
- VPC Peering
- Endpoints for S3
- Elastic IP
  - Reachable IPv4 address from the internet
  - After you get the Elastic IP, you must assign it to your EC2 instance
- Security Group
  - Firewall for each instance

>>>

## AWS VPC Gateways

- Virtual Private Gateway
  - GW between the private network (such as on-premise server) & VPC
- IGW: Internet Gateway
  - GW between the internet & VPC
  - Without this, instances can't have the global IP
- NGW: NAT gateway: Network Address Translation
  - GW between the internet & private subnet
  - Enable instances in the private subnet connect to internet / other AWS services
  - Disable the internet establish the connection to the instances
- API Gateway
- AWS Direct Connect

>>>

## AWS Products: MISC

- AWS Athena
- Search S3 storage with queries
- AWS Glue
- Amazon SNS: Simple Notification Service
- Amazon SQS: Simple Query Service
- AWS Snowball

>>>

## AWS: Account

- IAM: Identity and Access Management
- Root Acount
- IAM User

---

# EC2

>>>

## EC2: Setup

1. Generate key pair (if not set yet)
   - You can't connect to EC2 without local private key
   - On Ubuntu, you should put the `.pem` file to `~/.ssh` dir
2. Choose AMI
3. Choose instance type
4. Choose security group
   - In the inbound rules, allow access from `anywhere` with `HTTP` & `HTTPS`
5. Choose key pair
6. Launch
7. Connect with SSH
   - `ssh -i /path/my-key-pair.pem ec2-user@my-instance-IPv6-address`


### Ref

- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html
- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/get-set-up-for-amazon-ec2.html#create-a-base-security-group

>>>

## EC2: Amazon Linux

- Linux server OS of AWS
- Amazon Linux uses `yum` like Cent OS instead of `apt`

### Types

- Amazon Linux
- Amazon Linux 2
  - available as AMI

>>>

## EC2: AMI

- Amazon Machine Image provides the info required to launch an instance:
  - EBS snapshot(s)
  - Link to AWS account
  - Block device mapping which specifies the volumes to attach to the instance on launch

### Create

1. Create AMI
2. Register AMI
3. Launch AMI

>>>

## EC2 Instance Types: Category

- General Purpose: A, T, M
- Compute Optimized: C
- Memory Optimized: R, X, High Memory, z1d
- Accelerated Computing: P, Inf, G, F
- Storage Optimized: I, D, H

>>>

## EC2: Instance Types

- **t2.micro** is available for free tier
- Every instance can be Linux or Windows
- nano < micro < small < medium < large < xlarge < 2xlarge

>>>

## EC2: Connect to instance

- **SSH Client**
- EC2 Instance Connect
- AWS Systems Manager Session Manager
- PuTTY (Windows)

>>>

## AWS VPC: Config Example 1

- Internet -(IGW)- VPC > AZ (has Subnets)
  - IGW > Public Subnet > t2.micro Instance
  - IGW > Public Subnet > NGW > Private Subnet > DB

>>>

## AWS VPC: Config Example 2

- Internet - (ELB)
  - EC2 1 in AZ 1 -> RDS 1 -> RDS 2 (replicate of RDS 1)
  - EC2 2 in AZ 2 -> RDS 1 -> RDS 2 (replicate of RDS 1)

---

# Deploy to EC2

>>>

## AWS + Laravel

- A. Use AWS Beanstalk
  - Beanstalk -> My Code
- B. Deploy the Laravel on the  EC2 directly
  - Install LAMP, Composer manually with SSH
  - Host Infra -> OS -> Application Server -> HTTP Server -> My Code


>>>

## AWS + Laravel (Elastic Beanstalk)

1. Launch Elastic Beanstalk env
1. Bundle Laravel app into .zip
1. Upload & deploy .zip on EB console
1. Configure doc root path
1. Add DB Instance
1. Configure `/database.php`
1. Bundle & Deploy again

### Ref

- https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/php-laravel-tutorial.html
- https://dev.classmethod.jp/articles/elastic-beanstalk-laravel-deploy/

>>>

## AWS + Laravel: Overview

1. Create EC2 instance
2. Connect to EC2 with SSH
3. Install Apache, PHP, Postgres with `yum`
4. Start Apache, then configure file privileges
    - `sudo service httpd`
5. Install Composer
6. Git clone the Laravel project, and install dependencies
7. Configure MySQL & `.env`
8. Run file seeding

>>>

## AWS + Laravel: References

- https://qiita.com/masataka715/items/6e46f1f5e53bdff6cd3d
- https://qiita.com/nakm/items/0bcc6564538a0604b2ce
- https://qiita.com/atto/items/e1effd28c212c3829cb0
- https://varunver.wordpress.com/2016/06/03/centos-7-install-php-and-postgres/
  - install PHP, Postgres

>>>

## AWS + Laravel: Set up PHP

- `sudo yum install php -y`


>>>

## AWS + Laravel: Set up Apache

```sh
# install
sudo yum install -y httpd24

# start httpd
# http daemon runs in the backgroud of web server,
# and waits for incoming server requests
sudo service httpd start

# Add "apache" supplemental group to the user "ec2-user"
# -a "appends" anyone to a supplemental groups
# -G add supplemental groups
sudo usermod -a -G apache ec2-user

#
sudo chown -R ec2-user:apache /var/www

# 
sudo chmod 2775 /var/www

find /var/www -type d -exec sudo chmod 2775 {} \;

find /var/www -type f -exec sudo chmod 0664 {} \;
```

>>>

## AWS + Laravel: Set up Postgres

- `sudo yum install postgresql-server postgresql-contrib`
- `sudo yum install php-pgsql`: Connector of PHP & Postgres


>>>

## AWS + Laravel

- 

---

# RDS

>>>

## RDS

- a

---

# AWS + Gaming

## w/o CloudFront

- Internet -> ELB -> EC2 -> RDS

## w/ CloudFront (then)

- Route 1: Internet -> ELB -> EC2 -> RDS
- Route 2: Internet -> CF -> S3

## w/ CloudFront (modern)

- `CF -> ELB (ALB) -> EC2 (Apache) -> RDS (MySQL)`
- For static contents: CF returns the contents from the cache
- For dynamic contents: CF do nothing, EC2 & RDS returns the contents

---


>>>

## System Config

- App
  - CloudFront -> S3 -> ALB -> Apache PHP Servers
- Storage
  - RDS MySQL
  - ElastiCache (Redis): セッション保存用
  - EFS (NFS: Network File Systemの一種)
- Management
  - CloudWatch
  - Lambda
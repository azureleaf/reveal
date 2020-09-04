
# AWS

---

# Overview

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

## AWS Products 1/6: Computing

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

## AWS Products 2/6: Container

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

## AWS Products 3/6: Storage

- **S3**: Simple Store Service
  - Cheap
- **EBS**: Elastic Block Store
  - Virtual hard disks
- **RDS**: Relational Database Service
  - MySQL, Oracle, Postgres, SQL Server...
- EFS: Elastic File System
- DynamoDB
- ElastiCache
- RedShift
- AWS Aurora: RDB compatible with MySQL / PostgreSQL

>>>

## AWS Storage: S3 vs EFS vs EBS

- S3 は Object Storage
- EFSはNFS(Network File SYstem)
  - OSからマウントできる。S3はHTTPS経由でアクセス
  - EC2にマウントできる（EBSと同じ）
  - **複数のAZにまたがる大量のEC2 Instance**から同時にアクセス可
- EBSはBlock Storage
  - EC2にマウントできる（EFSと同じ）
  - **単一AZの単一のEC2からアクセス** (一つのEC２インスタンスは複数のEBSにマウントできるが)

>>>

## AWS Products 4/6: Management

- **ELB**: Elastic Load Balancing
  - Application LB
  - Network LB
  - Classic LB
- **Auto Scaling**
- **CloudFormation**
- IAM: Identity and Access Management
  - Control the access to the AWS accounts
- App Mesh
- ParameterStore

>>>

## AWS Products 5/6: Monitoring

- **CloudWatch**
- DataDog
  - DataDog is provided by DataDog corp, not by AWS
  - Offer the console for the AWS monitoring services
- CloudTrail
  - Monitor the AWS Account activity

>>>

## AWS Products 6/6: Networking

- CloudFront
  - CDN service: Static / dynamic contents will be delivered from the nearest server to the user
  - high speed delivery with cache: streaming is possible too
- Amazon Route 53
  - DNS service

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

## AWS: MISC

- AWS cli
- Amazon Linux

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
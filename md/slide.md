## Study Notes for Coding

---

## Todos

1. TCP/IP
2. SSH & Encryption
3. Cookie & Session
4. PHP: array, control syntax
5. PHP: interface, trait, class
6. PHP: Class, constructor, destructor, inheritance, final
7. Tech blog
8. PHP: File IO
9.  PHP PDO, 
10. SQL
11. DB: Indexing, Regularization of the
12. AWS

---

## ToC

>>>

- [Knowing the Corps.](#knowing-the-corps)
  - [il](#il)
  - [il: gaming](#il-gaming)
  - [il: non-gaming](#il-non-gaming)
  - [il: vr/ar](#il-vrar)
  - [il: people whom they want to hire](#il-people-whom-they-want-to-hire)
- [MISC](#misc)
  - [CS Books](#cs-books)
- [AWS](#aws)
  - [Region & AZ](#region--az)
  - [Create Instance](#create-instance)
  - [AWS Products 1/6: Computing](#aws-products-16-computing)
  - [AWS: EC2 vs Lightsail](#aws-ec2-vs-lightsail)
  - [AWS Products 2/6: Container](#aws-products-26-container)
  - [AWS: Why use Fargate?](#aws-why-use-fargate)
  - [AWS Products 3/6: Storage](#aws-products-36-storage)
  - [AWS Storage: S3 vs EFS vs EBS](#aws-storage-s3-vs-efs-vs-ebs)
  - [AWS Products 4/6: Management](#aws-products-46-management)
  - [AWS Products 5/6: Monitoring](#aws-products-56-monitoring)
  - [AWS Products 6/6: Networking](#aws-products-66-networking)
  - [AWS VPC: Features](#aws-vpc-features)
  - [AWS VPC: Keywords](#aws-vpc-keywords)
  - [AWS VPC Gateways](#aws-vpc-gateways)
  - [AWS Products: MISC](#aws-products-misc)
  - [AWS: MISC](#aws-misc)
  - [AWS: Account](#aws-account)
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
  - [AWS + Laravel](#aws--laravel)
  - [AWS + Laravel (Elastic Beanstalk)](#aws--laravel-elastic-beanstalk)
    - [Ref](#ref-1)
  - [AWS + Laravel: Overview](#aws--laravel-overview)
  - [AWS + Laravel: References](#aws--laravel-references)
  - [AWS + Laravel: Set up PHP](#aws--laravel-set-up-php)
  - [AWS + Laravel: Set up Apache](#aws--laravel-set-up-apache)
  - [AWS + Laravel: Set up Postgres](#aws--laravel-set-up-postgres)
  - [AWS + Laravel](#aws--laravel-1)
- [Frontend](#frontend)
  - [MISC](#misc-1)
  - [Framework](#framework)
  - [Frontend Libs](#frontend-libs)
  - [Design Libs](#design-libs)
  - [SSR vs SSG](#ssr-vs-ssg)
  - [Cookie & Session](#cookie--session)
- [Backend](#backend)
  - [IaC: What’s this?](#iac-whats-this)
  - [IaC: Products](#iac-products)
  - [Ansible](#ansible)
  - [Search](#search)
  - [Big Data](#big-data)
  - [Connection](#connection)
  - [Web Stack](#web-stack)
  - [Server Types](#server-types)
  - [Monitoring: Services](#monitoring-services)
  - [Monitoring: CloudWatch](#monitoring-cloudwatch)
  - [Monitoring](#monitoring)
  - [Monitoring Servers](#monitoring-servers)
  - [Monitoring: MISC](#monitoring-misc)
  - [Monitoring: Visualization](#monitoring-visualization)
  - [Server Product](#server-product)
  - [Deployment Env.](#deployment-env)
- [Quality Control](#quality-control)
  - [Testing Types](#testing-types)
  - [Tools](#tools)
  - [Frontend Performance: TTFB](#frontend-performance-ttfb)
- [DB](#db)
  - [DB MISC](#db-misc)
  - [3層スキーマ](#3層スキーマ)
  - [DB Model](#db-model)
  - [ER Diagram](#er-diagram)
  - [DB types](#db-types)
  - [正規形](#正規形)
  - [従属](#従属)
  - [演算](#演算)
    - [関係演算](#関係演算)
    - [集合演算](#集合演算)
  - [SQL: Lang Types](#sql-lang-types)
  - [SQL: SELECT](#sql-select)
  - [DBMS](#dbms)
  - [SQL: GRANT](#sql-grant)
  - [Mutex for DB](#mutex-for-db)
  - [Mutex for DB: Lock](#mutex-for-db-lock)
  - [障害回復](#障害回復)
  - [DB Performance](#db-performance)
  - [Strategy to increase the DB server performance](#strategy-to-increase-the-db-server-performance)
  - [Distributed DB: MISC](#distributed-db-misc)
  - [分散DBでの表の結合方法](#分散dbでの表の結合方法)
  - [Distributed DB: Basics](#distributed-db-basics)
  - [Distributed DB: Advantage](#distributed-db-advantage)
  - [Distributed DB: Keywords](#distributed-db-keywords)
  - [Transaction: ACID](#transaction-acid)
  - [Transaction: Isolation Level](#transaction-isolation-level)
  - [Transaction: Isolation MISC](#transaction-isolation-misc)
  - [RDB](#rdb)
  - [DB Partitioning: Overview](#db-partitioning-overview)
  - [DB partitioning: Category](#db-partitioning-category)
  - [DB partitioning:](#db-partitioning)
- [Operating System](#operating-system)
  - [Mutual Exclusion](#mutual-exclusion)
  - [Automaton](#automaton)
  - [`service` command](#service-command)
  - [File permission](#file-permission)
  - [User Group](#user-group)
    - [Primary Group vs Secondary Group](#primary-group-vs-secondary-group)
    - [bash](#bash)
    - [UID vs GID](#uid-vs-gid)
    - [ref.](#ref-2)
  - [chmod: ls -l](#chmod-ls--l)
    - [rwx](#rwx)
    - [`drwxr-xr-x`](#drwxr-xr-x)
  - [chmod: permission](#chmod-permission)
    - [Specify all the actions](#specify-all-the-actions)
    - [Specify one action](#specify-one-action)
  - [chmod: Use with find command](#chmod-use-with-find-command)
  - [chown](#chown)
  - [Apache](#apache)
- [Computer Architecture](#computer-architecture)
  - [Memory](#memory)
  - [CPU](#cpu)
  - [Instruction Cycle](#instruction-cycle)
  - [GPU](#gpu)
  - [Primary Storage](#primary-storage)
  - [Secondary Storage](#secondary-storage)
- [Software Engineering](#software-engineering)
  - [Dev.](#dev)
  - [Agile Dev. vs Waterfall Dev.](#agile-dev-vs-waterfall-dev)
  - [SCRUM](#scrum)
    - [DDD](#ddd)
  - [Design Pattern: Web](#design-pattern-web)
  - [Design Pattern](#design-pattern)
  - [CI/CD Tools: Products](#cicd-tools-products)
  - [CI/CD Tools: Why necessary?](#cicd-tools-why-necessary)
  - [Modular Programming](#modular-programming)
  - [Cohesion](#cohesion)
  - [Coupling](#coupling)
  - [Redundancy Tips](#redundancy-tips)
  - [Redundancy: Number of entities](#redundancy-number-of-entities)
  - [Redundancy: Roles](#redundancy-roles)
- [Gaming](#gaming)
  - [Data format used for server-client comm.](#data-format-used-for-server-client-comm)
  - [MISC](#misc-2)
  - [Maintenance](#maintenance)
  - [Gaming + AWSの例](#gaming--awsの例)
- [VR](#vr)
  - [Virtual Cast](#virtual-cast)
  - [VR](#vr-1)
- [Network](#network)
  - [Network: MISC](#network-misc)
  - [Xaas](#xaas)
  - [XaaS Comparison](#xaas-comparison)
  - [VPN: What's this?](#vpn-whats-this)
    - [Types](#types-1)
  - [VPN: VPN vs Leased Line](#vpn-vpn-vs-leased-line)
  - [VPN: Internet VPN technologies](#vpn-internet-vpn-technologies)
  - [VPN: Protocols](#vpn-protocols)
  - [Latency vs Bandwidth](#latency-vs-bandwidth)
  - [DNS](#dns)
  - [IPv4:](#ipv4)
  - [IPv6:](#ipv6)
  - [TCP / IP Model](#tcp--ip-model)
  - [OSI Model](#osi-model)
  - [Tools](#tools-1)
  - [Network Devices](#network-devices)
  - [Network Devices](#network-devices-1)
  - [LAN Topology](#lan-topology)
  - [LAN Access Control Methods](#lan-access-control-methods)
  - [WLAN](#wlan)
  - [Network Cables](#network-cables)
  - [TCP / IP](#tcp--ip)
- [Security](#security)
  - [Attacks](#attacks)
  - [Encrytion Keywords](#encrytion-keywords)
  - [Public-key Cryptography](#public-key-cryptography)
  - [How login works with SSH](#how-login-works-with-ssh)
    - [On registration](#on-registration)
    - [On login](#on-login)
  - [SSH: Secure SHell](#ssh-secure-shell)
    - [SSH vs SSL](#ssh-vs-ssl)
  - [CORS](#cors)
  - [CSRF](#csrf)
- [Authentication & Authorization](#authentication--authorization)
  - [JWT](#jwt)
  - [Social Login](#social-login)
  - [Passport](#passport)
  - [Cookie & Session](#cookie--session-1)
- [Virtualization](#virtualization)
  - [Tools](#tools-2)
- [Computer Architecture](#computer-architecture-1)
- [Algorithm](#algorithm)
  - [Data Structure](#data-structure)
  - [shell](#shell)
- [PHP](#php)
  - [PHP Tools](#php-tools)
  - [Laravel Topics ***](#laravel-topics-)
  - [Laravel Topics **](#laravel-topics--1)
  - [Laravel Topics *](#laravel-topics--2)
  - [PHP: Class Inheritance](#php-class-inheritance)
  - [PHP Frameworks](#php-frameworks)
  - [PHP vs JS: Array](#php-vs-js-array)
  - [PHP vs JS: Class](#php-vs-js-class)
  - [PHP Modifier](#php-modifier)
  - [PHP const](#php-const)
  - [PHP vs JS: Control Statement](#php-vs-js-control-statement)
  - [Scope Resolution Operator ::](#scope-resolution-operator-)
  - [PHP: Abstract class vs Trait vs Interface](#php-abstract-class-vs-trait-vs-interface)
  - [PHP Logging](#php-logging)
  - [PHP Interesting Syntax](#php-interesting-syntax)
  - [PHP Files](#php-files)
  - [PHP Constants](#php-constants)
- [Tips](#tips)
  - [Using fish](#using-fish)

---

# Knowing the Corps.

>>>

## il

- 「最先端の最後尾を独走する」: ゆるさ + 技術
- staff: 160
- Sendai + Sapporo
- President: Matsui, Vice-president: Ono
- 97% employees take paid vacation / "reversi vacation", after-release vacation
- Being forced to work on weekends is rare; overtime work is 1 hr a day?
- Special budget for a coronavirus: 50000 jpy
- in-compnay

>>>

## il: gaming

- Main: "Strategy" game for smartphones

>>>

## il: non-gaming

- AI Haiku
- Cyrstal Signal Pi
  - Started as IL club activity
- Shukiin
- cartoru
  - Car seller + VR

>>>

## il: vr/ar

- `Virtual Cast`
  - Started as IL club activity
- `The Seed Online`
- Shifting focus onto XR / Unity from Gaming / PHP
- Wanna increase in-house dev instead of contracted dev

>>>

## il: people whom they want to hire

- Has a specific strong interest / achievements 
- Understands the policy / culture of our corp
- Can work as a team member over a long time period
- Wanna recruit local people
- Has output
  - Without portfolio programs, you can't judge anybody.
  - Portfolio is precious source of info to know the applicants even when it's not so sophisticated
- Interested in the programming edu for children (sample for the people)
- Has future vision

---

# MISC

>>>

## CS Books

- Readable Code
- Refactoring
- Algorithm
- Network
- Computer Architecture

---

# AWS


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

---

# Frontend

>>>

## MISC

- Service Worker
- PWA
- SSG: Static Site Generation
- SSR: Server Side Rendering

>>>

## Framework

- Vue
- React
- Angular

>>>

## Frontend Libs

- Storybook
- Nuxt.js

## Design Libs

- Vuetify
- Elm
- Semantic UI

>>>

## SSR vs SSG

- Nuxt.js
  - Universal Mode: 
  - SPA Mode 

>>>

## Cookie & Session

>>>

---

# Backend

>>>

## IaC: What’s this?
- Infrastructure As Code
- AD
  - Less Human Error
- DA

>>>

## IaC: Products

- Ansible
- Chef
- Puppet
- Terraform

>>>

## Ansible

- Define the env by YAML

>>>

## Search

- SQL
- GraphQL
- BigQuery
- Elastic Search

>>>

## Big Data

- Hadoop
- Spark

>>>

## Connection

- Web Socket

>>>

## Web Stack

- LAMP: Linux + Apache + MySQL + PHP/Python/Perl
- LEMP: Nginx
- MEAN: Mongo + Express + Angular + Node
- JAMstack: JS + API + Markup

>>>

## Server Types

- DB Server: Master / Slave
- API Server
- Proxy Server

>>>

## Monitoring: Services

- AWS CloudWatch

>>>

## Monitoring: CloudWatch

- CloudWatch Logs
- Simple search with text or JSON
- CloudWatch Logs Insights
- Complicated queries to search logs (<1000 lines)
- Send logs to S3 & Search with AWS Athena

>>>

## Monitoring

- Fluentd

>>>

## Monitoring Servers

- Cacti

>>>

## Monitoring: MISC

- KPI: Key Performance Indicators
- DataDog
- Sentry

>>>

## Monitoring: Visualization

- Kibana
- Tableau
- MS Power BI

>>>

## Server Product

- Apache
- Nginx
- Tomcat (Java)

>>>

## Deployment Env.

- Production Env. 本番環境
- Staging Env.
- Testing Env.

---

# Quality Control

>>>

## Testing Types

- Unit Test
- Integration Test

>>>

## Tools

- JEST
- Mocha
- Jasmine
- Cypress
- Puppeteer
  - E2E
- Chai
- PHPUnit (for PHP)
- Enzyme (for React)
- Postman
  - API
- Storybook
  - UI test
- Lighthouse
  - Website Performance

>>>

## Frontend Performance: TTFB

- DNS
- Connect
- SSL
- Send
- Wait
- Receive


---

# DB

>>>

## DB MISC

- KVS: Key Value Store
- memcached
- DWH (Dataware House) vs DB

>>>

## 3層スキーマ

- Conceptual Schema
- External Schema
  - User / Application
- Internal Schema
  - Hardware

>>>

## DB Model

- Conceptual Model
  - ER diagram
- Logical Model
- Physical Model

>>>

## ER Diagram

>>>

## DB types

- 階層型
  - one root
- ネットワーク型
- RDB

>>>

## 正規形

- 第一正規形
- 第二正規形
- 第三正規形


>>>

## 従属

- 関数従属
- 完全関数従属
- 推移関数従属

>>>

## 演算

### 関係演算

- 選択
  - 行方向の取り出し
- 射影
  - 列方向の取り出し
- 結合
  - JOIN
- 商

### 集合演算

- 和
  - ２表から単純に全ての行を取り出す
- 差
  - １つの表にあり、もう一方にない行を取り出す
- 積
  - ２表に共通する行のみ取り出す
- 直積
  - ２表から全てを組み合わせる
  - 列は２倍になり、行の数は`m * n`になる
  - 
>>>

## SQL: Lang Types

- DML: Data Manipulation Language
- DDL: Data Definition Language
  - e.g. CREATE, ALTER, DROP
- DCL: Data Control Language
  - Define DB Authorization

>>>

## SQL: SELECT

- WHERE: AND / OR / NOT / AS
- DISTINCT：　重複したものは省く
- ORDER BY: ASC / DESC
- LIKE: 正規表現みたいな
- IN / BETWEEN
- EXISTS
- 集合演算: UNION / EXCEPT / INTERSECT

>>> 

## DBMS


>>>

## SQL: GRANT

- GRANT ALL PRIVILEGES
- GRANT SELECT, UPDATE, INSERT, UPDATE, DELETE
- GRANT SELECT ON products TO PUBLIC
  - 全てのユーザーに対して与える
- REVOKE SELECT ON products FROM user

>>>

## Mutex for DB

- Lock
  - 占有ロック
  - 共有ロック
- Timestamp
- 楽観的制御

>>>

## Mutex for DB: Lock

- ロックの粒度
- ２相ロック
  
>>>

## 障害回復

- Log (aka Journal)
  - WALでないと駄目
  - Roll forward
  - Roll back
- CHeck point

## DB Performance

- Index
- Hash
- B-tree

>>>

## Strategy to increase the DB server performance

- Distribute the DB: Master & Slaves
- Store the DB data in the memory rather than disk
  - With **tmpfs** of the Linux you can use certain memory space as the file system
  - This strategy is available for the slave server, because the data in the memory isn't persistent and can be lost in the server crash
- MySQL Cluster
- DB partitioning

>>>

## Distributed DB: MISC

- 2相コミット
- ３相コミット
- セミジョイン

>>>

## 分散DBでの表の結合方法

- Nested Loop
- Sort Merge
- Hash Join

>>>


## Distributed DB: Basics

- Master Server
  - Mostly single; to populate the master, you need complicated clustering
  - Referred for CUD of CRUD
- Slave Servers
  - Multiple; populating the slaves is easy
  - A slave can has single master only
  - Updates in the master always propagate to servers; this is one-way.
  - Referred for R of CRUD
    - Therefore Master-Slave architecture is powerful when reference is more frequent than updating

>>>

## Distributed DB: Advantage

- Higher performance on DB references
- Higher availability
  - When the master DB is down, the slave can be the master instead
- Higher geo-redundancy (地理的冗長性)
  - You can put the master / slaves in the geographically distant places; this increase the tolerance to the disaster
- Easier to get the backup
  - Creating the backup data from the slave won't affect the performance of the master

>>>

## Distributed DB: Keywords

- Database Polling (ポーリング)
- Synchrnous Replication / Asynchronous Replication

>>>

## Transaction: ACID

- Atomicity
- Consistency
- Isolation
- Durability
  
>>>

## Transaction: Isolation Level

- READ UNCOMMITTED
- READ COMMITTED
- REPEATABLE READ
- SERIALIZABLE

>>>

## Transaction: Isolation MISC

- Dirty Read
- Non-repeatable Read
- Phantom

>>>

## RDB

>>>


>>>

## DB Partitioning: Overview

- Dividing a large database with many tables into small databases
- Advantage

- MySQL supports partitioning by default


>>>


## DB partitioning: Category

- Vertical Partitioning
- Horizontal Partitioning

>>>

## DB partitioning: 

- 

---

# Operating System

>>>

## Mutual Exclusion

>>>


## Automaton

>>>

## `service` command

- Used to start / stop / check services
- Then: wrapper for `/etc/init.d`, `initctl`
- Now:  wrapper for `/etc/init.d`, `initctl`, `systemctl`

>>>

## File permission

- chmod: Change mode (about permission)
- chown: Change owner
- chgrp: Change group

https://qiita.com/t-a-run/items/239ed690ece7a011804a


>>>

## User Group

### Primary Group vs Secondary Group

- Primary group (aka Login group)
  - Each user can belong to single primary group only
- Secondary Group (aka Supplementary Group)

### bash

- `$ groups`
- `$ groups john`

### UID vs GID

### ref.

- https://www.networkworld.com/article/3409781/mastering-user-groups-on-linux.html

>>>

## chmod: ls -l

### rwx

- `r` or `4`: readable
- `w` or `2`: writable
- `x` or `1`: executable
- Therefore `drwxr-xr-x` is equivalent to `755`

### `drwxr-xr-x`

1. `d`: this is a dir
2. `rwx`: **owner** can read, write, execute
3. `r-x`: **group** can read, execute
4. `r-x`: **others** can read, execute

>>>

## chmod: permission

### Specify all the actions

- `chmod 775 /var/www`
- `chmod -R 775 /var`
  - Change for all the files in the dir recursively 
- `chmod 2775 /var/www`
  - Here "2" digit is for `setgid` (set group ID)

### Specify one action

- `u` User (owner)
- `g` Group
- `o` Other
- `a` All (user, group, other)
- `chmod g+x /var/www` Add permission
- `chmod ugo-wx /var/www` Revoke permission

>>>

## chmod: Use with find command

- Find command takes "action" to execute the commands
- `$ find . -type f -exec chmod 600 {} +`
- `find . -type f | xargs chmod 600`



>>>

## chown

- `chown john /var/www`
- `chown john -R var`: All the files in the dir
- `chown john:staff /var/www`: Owner is john, group is staff


>>>

## Apache



---

# Computer Architecture

>>>

## Memory

- ROM
- RAM
  - DRAM: Dynamic RAM
    - SDRAM: Synchronous DRAM
    - RDRAM: Rambus DRAM
    - DDR SDRAM: Double Data Rate SDRAM
      - DDR1
      - DDR2
      - DDR3
      - DDR4
      - 
  - SRAM: 

>>>

## CPU

- ALU
- Instruction Register: 命令レジスタ
  - Holds the address of the current instruction fetched
- General-purpose Register: 汎用レジスタ
- Program Counter
  - Address of the next instruction
- Index Register
- Base Register
- Accumulator
- 命令デコーダ

>>>

## Instruction Cycle

1. Fetch Stage
   1. Fetch the next instruction addr from the program counter
   2. Store the next instruction in the instruction register
2. Decode Stage
3. Execute Stage

>>>

## GPU


>>>

## Primary Storage

- Processor Registers
- Processor Cache

>>>


## Secondary Storage

- HDD
- SSD
- 


---

# Software Engineering

>>>

## Dev.

- TDD: Test-Driven Dev.
- DDD: Domain-Driven Dev.
- Agile Software Dev.
- SCRUM
- Waterfall Model
- Spiral Model
- Prototype Dev

>>>

## Agile Dev. vs Waterfall Dev.

- 企画 -> 要件定義 -> 設計 -> 実装 -> テスト
- Short Iteration (2 weeks), therefore flexible

>>>

## SCRUM

- Daily Scrum
- Sprint Planning
- Sprint
- Sprint Review

>>>

### DDD

- Domain: ソフトウェアの問題解決の領域に基づいて開発する


>>>

## Design Pattern: Web

- MVC
- ADR

>>>

## Design Pattern

- Singleton
- Decorator
- Facade
- Observer

>>>

## CI/CD Tools: Products

- On-premise
- Jenkins
- Cloud based
- Travis
- Circle CI
- TeamCity (by JetBrains)
- Bamboo
- Codeship
- GitLab CI
- AWS Code Build
- GCP Cloud Build

>>>

## CI/CD Tools: Why necessary?

- Source Control Version Management
- Automated Testing
- Build Automation
- Automated Deployment

>>>

## Modular Programming

>>>

## Cohesion

- Co-incidental Cohesion

>>>

## Coupling

- 

>>>

## Redundancy Tips

- RAID
- 

>>>

## Redundancy: Number of entities

- DMR: Dual Modular Redundancy
- TMR: Triple Modular Redundancy

## Redundancy: Roles

- Active-Active Clustering
  - Mainly used for the load balancing
- Active-Passive Clustering
  - Main usage: Primary HTTP Server + Failover HTTP Server

---

# Gaming

>>>

## Data format used for server-client comm.

- Returns HTML
- Returns JSON

>>>

## MISC

- DAU: Daily Active Users
- Communication Protocol
- HTTP
- Concurrent Access (同時アクセス数) is like 10k - 100k, for example

>>>

## Maintenance

- 定期メンテナンス
- 緊急メンテナンス
- 無停止メンテナンス

>>>

## Gaming + AWSの例

- APP
  - CloudFront -> S3 -> ALB -> Apache PHP Servers
- Storage
  - RDS MySQL
  - ElastiCache (Redis): セッション保存用
  - EFS (NFS: Network File Systemの一種)
- 運用系
  - CloudWatch
  - Lambda
  - EC2

---

# VR

>>>

## Virtual Cast

- Dwango + Infinite Loop
- Streaming: Raw voice + Virtual avatar animation

>>>

## VR

- HMD: Head Mount Display
  - PlayStation VR
  - Gear VR
  - Google Cardboard
  - HTC Vive
- Dev Engine
  - Unity

---

# Network

>>>

## Network: MISC

- NFS: Network File System


>>>

## Xaas

- IaaS: Infrastructure
  - Similar to conventional hosting services, however you can customize hardwares flexibly
- PaaS: Platform
- SaaS: Software
- BaaS / mBaaS: Backend 

>>>

## XaaS Comparison

|                | On-Premises |          IaaS          |                      PaaS                       |                  SaaS                   |
| -------------- | :---------: | :--------------------: | :---------------------------------------------: | :-------------------------------------: |
| Application    |    user     |          user          |                      user                       |                provider                 |
| Data           |    user     |          user          |                      user                       |                provider                 |
| Runtime        |    user     |          user          |                    provider                     |                provider                 |
| Middleware     |    user     |          user          |                    provider                     |                provider                 |
| OS             |    user     |          user          |                    provider                     |                provider                 |
| Virtualization |    user     |        provider        |                    provider                     |                provider                 |
| Servers        |    user     |        provider        |                    provider                     |                provider                 |
| Storage        |    user     |        provider        |                    provider                     |                provider                 |
| Networking     |    user     |        provider        |                    provider                     |                provider                 |
| Examples:      |    user     | EC2, GCE, DigitalOcean | GAE, Beanstalk, Heroku, Azure, RedHat OpenShift | Google Apps, Salesforce, Dropbox, Slack |

>>>

## VPN: What's this?

- Safe

### Types
- Internet VPN
  - Cheap but not so safe as others
- IP-VPN
  - Closed network for the ISP and its users
  - No need for encryption, however expensive
- Entry VPN
- WAE: Wide Area Ethernet
  - Highly customizable, but expensive and narrow

>>>

## VPN: VPN vs Leased Line

- Leased Line (専用線) is physical

>>>

## VPN: Internet VPN technologies

- Tunneling
- 

## VPN: Protocols

- IPsec-VPN
- L2TP
- PPTP
- SSL-VPN

>>>

## Latency vs Bandwidth

>>>

## DNS

- 

>>>

## IPv4:

>>>

## IPv6:




>>>

## TCP / IP Model

>>>

## OSI Model

>>>

## Tools

- Wireshark
- Firebug (dead?)

>>>

## Network Devices

- DTE: Data Terminal Equipment
- DCE: Data Circuit Terminating Equipment

## Network Devices

- Hub
- Repeater
- Bridge
- Router
- Switch

## LAN Topology

- Bass
- Star
- Ring

## LAN Access Control Methods

- CSMA/CD
- Token Passing

## WLAN

- 


## Network Cables

- 


>>>

## TCP / IP



---

# Security

>>>

## Attacks

- DDoS


>>>


## Encrytion Keywords

- Public-key Cryptography
- Symmetric key algorithms
- SSH is for secure connection to the server
- SSL is for secure display of the web page
  - HTTPS website uses SSL
  - Uses both public-key crypt & symmetric key crypt
- Digital Signature
- PKI: Public Key Infrastructure

>>>

## Public-key Cryptography

1. Recipient: Create the pair of **public key** & **private key**
2. Recipient: Send the **public key** to the sender
3. Sender: Get the public key of the recipient
4. Sender: Encrypt the contents with **public key**
5. Sender: Send the encrypted contents
6. Recipient: Decrypt the encrypted contents with **private key**

>>>

## How login works with SSH

### On registration

1. Client generates the key pair
2. Client sends the public key to the server

### On login

1. Client tells the server that he wants to login
2. Server creates encrypted content with the **public key**
3. Client decrypts the content with **private key, then give it to the server
4. Now the server can know that the client is authentic

>>>

## SSH: Secure SHell



### SSH vs SSL


>>>

## CORS

>>>

## CSRF

---

# Authentication & Authorization

>>>

## JWT

## Social Login

## Passport

>>>

## Cookie & Session

---

# Virtualization

>>>

## Tools

- Vagrant
- Virtual Box
- VMWare
- Docker
- Hyper-v
- WSL: Windows Subsystem for Linux

---

# Computer Architecture

---

# Algorithm

>>>


## Data Structure

>>>


>>>

## shell

>>>

- ls
- rm


>>>

- sed
- awk
- grep

>>>

- jq
- rsync

---

# PHP

>>>

## PHP Tools
- artisan
- composer
- php.ini
- php -a
- php -f hello.php
- phpinfo

>>>

## Laravel Topics ***

- MW
- Migration / Seeder / Factory
- Controller / Action / Blade
- Eloquent ( Collection / Mutator / Serialization)
- CSRF / Session

>>>

## Laravel Topics **

- Facade / Contract
- Service Provider / Service Container / Dependency Injection
- Accessor
- Auth / Bcrypt
- Dockerize Laravel App / Homestead

>>>

## Laravel Topics *

- Broadcasting / Job / Queue / Work / Mocking

>>>

## PHP: Class Inheritance

- Interface
- Trait
- Abstract Class

>>>

## PHP Frameworks
- Laravel
- Symfony
- CakePHP
- FuelPHP

>>>

## PHP vs JS: Array

>>>

## PHP vs JS: Class

- public function __construct()
- public function __destruct()
- new ReflectionClass()
- final
- self::
- $this->

>>>

## PHP Modifier

- public
- protected
- private

>>>

## PHP const

- const

>>>

## PHP vs JS: Control Statement

- foreach()

>>>

## Scope Resolution Operator ::

- parent
- static
- self

>>>

## PHP: Abstract class vs Trait vs Interface

>>>


## PHP Logging

- dd()
- for Laravel only
- var_export()
- var_dump()
- print_r()

>>>

## PHP Interesting Syntax

- “??”
- Coalescing Operator, shorthand for Ternary Operator, maybe
- “static”
- “namespace”

>>>

## PHP Files

- `fopen()`
- `fclose()`

>>>

## PHP Constants

```php
__DIR__
__FILE__
__FUNCTION__
__CLASS__
__METHOD__
__LINE__
line number
__NAMESPACE__
```

>>>

# Tips

>>>

## Using fish

```sh
sudo apt install fish

# using fish
fish

# change default (require re-login to apply change)
chsh -s /usr/bin/fish # to fish
chsh -s /bin/bash # to bash

# config
mkdir -p ~/.config/fish
vim ~/.config/fish/config.fish

# config
fish_config

# config file: remove greeting message on launch
set -g -x fish_greeting ''

# oh-my-fish
curl -L https://get.oh-my.fish | fish
omf install agnoster
omf theme agnoster


```

## Study Notes for Coding

---

## ToC

>>>

- [MISC](#misc)
  - [CS Books](#cs-books)
- [AWS](#aws)
  - [AWS Basics:](#aws-basics)
  - [Creating Instance](#creating-instance)
  - [AWS Products: Computing](#aws-products-computing)
  - [AWS Products: Container](#aws-products-container)
  - [AWS: Why use Fargate?](#aws-why-use-fargate)
  - [AWS Products: Storage](#aws-products-storage)
  - [AWS Products: Management](#aws-products-management)
  - [AWS Services for Networking](#aws-services-for-networking)
  - [AWS Products: MISC](#aws-products-misc)
  - [AWS: MISC](#aws-misc)
  - [AWS EC2](#aws-ec2)
  - [AWS VPC: Features](#aws-vpc-features)
  - [AWS VPC: Keywords](#aws-vpc-keywords)
  - [AWS VPC: Config Example 1](#aws-vpc-config-example-1)
  - [AWS VPC: Config Example 2](#aws-vpc-config-example-2)
  - [AWS + Laravel](#aws--laravel)
  - [AWS + Laravel: Refs](#aws--laravel-refs)
  - [AWS + Laravel:](#aws--laravel-1)
  - [AWS + Laravel: References](#aws--laravel-references)
- [Frontend](#frontend)
  - [MISC](#misc-1)
  - [Framework](#framework)
  - [Frontend Libs](#frontend-libs)
  - [Design Libs](#design-libs)
  - [SSR vs SSG](#ssr-vs-ssg)
- [Backend](#backend)
  - [IaC: What’s this?](#iac-whats-this)
  - [IaC: Products](#iac-products)
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
  - [SQL](#sql)
  - [Distributed DB](#distributed-db)
  - [Transaction](#transaction)
  - [RDB](#rdb)
  - [ER](#er)
- [Operating System](#operating-system)
  - [Mutual Exclusion](#mutual-exclusion)
  - [Automaton](#automaton)
- [Computer Architecture](#computer-architecture)
  - [Memory](#memory)
  - [CPU](#cpu)
  - [GPU](#gpu)
  - [Primary Storage](#primary-storage)
  - [Secondary Storage](#secondary-storage)
- [Software Engineering](#software-engineering)
  - [Dev.](#dev)
  - [Agile Dev. vs Waterfall Dev.](#agile-dev-vs-waterfall-dev)
  - [SCRUM](#scrum)
  - [Design Pattern: Web](#design-pattern-web)
  - [Design Pattern](#design-pattern)
  - [CI/CD Tools: Products](#cicd-tools-products)
  - [CI/CD Tools: Why necessary?](#cicd-tools-why-necessary)
  - [Modular Programming](#modular-programming)
  - [Cohesion](#cohesion)
  - [Coupling](#coupling)
  - [Redundancy Tips](#redundancy-tips)
  - [Redundancy: Number of](#redundancy-number-of)
- [Gaming](#gaming)
  - [Data format used for server-client comm.](#data-format-used-for-server-client-comm)
  - [MISC](#misc-2)
  - [Maintenance](#maintenance)
- [Network](#network)
  - [Network: MISC](#network-misc)
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
  - [Encrytion](#encrytion)
  - [CORS](#cors)
  - [CSRF](#csrf)
- [Authentication & Authorization](#authentication--authorization)
  - [JWT](#jwt)
  - [Social Login](#social-login)
  - [Passport](#passport)
  - [Cookie & Session](#cookie--session)
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

## AWS Basics:

- AMI: Amazon Machine Image
- VPC: Virtual Private Cloud
  - EC2 (server) + VPC (network) is the major combination
- Region:
  - "ap-northeast-1" is for Tokyo
- AZ: Availability Zone
  - A region has multiple data centers
  - A service can ber deployed to multiple AZs for redundancy
- Instance
- EBS: Elastic Block Store
  - Virtual hard disks
- IAM: Identity and Access Management
- Security Group

>>>

## Creating Instance

1. Choose AMI
2. Choose an instance type
3. Configure the instance details
4. Add tags
5. Set up Security group
6. Start

>>>

## AWS Products: Computing

- * EC2: Elastic Compute Cloud
- Lightsail
- *Lambda
  - Run the code triggered by the events
- Elastic Beanstalk
  - PaaS for PHP, Node, Python, Docker... etc.

>>>

## AWS Products: Container

- ECS: Elastic Container Service
- EKS: Elastic Kubernetes Service
- Fargate
  - Compute Engine for ECS / EKS

>>>

## AWS: Why use Fargate?

1. Build the container image 
2. Deploy EC2 instances (Fargate does this instead of you!)
3. Define memory resources
4. Isolate apps with VMs (Fargate does this instead of you!)
5. Run app

>>>

## AWS Products: Storage

- *S3: Simple Store Service
  - Cheap
- *RDS: Relational Database Service
  - MySQL, Oracle, Postgres, SQL Server...
- EFS: Elastic File System
- DynamoDB
- ElasiCache
- RedShift
- AWS Aurora: RDB compatible with MySQL / PostgreSQL

>>>

## AWS Products: Management

- *CloudWatch
- *ELB: Elastic Load Balancing
  - Application LB
  - Network LB
  - Classic LB
- *Auto Scaling
  - 
- App Mesh

>>>

## AWS Services for Networking

- CloudFront
- VPC: Virtual Private Cloud
- selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways
- API Gateway

>>>

## AWS Products: MISC

- AWS Athena
- Search S3 storage with queries
- AWS Glue
- AWS Lightsail
- AWS Elastic Beanstalk
- Amazon SNS: Simple Notification Service
- Amazon SQS: Simple Query Service
- AWS Snowball

>>>

## AWS: MISC

- AWS cli
- Amazon Linux

>>>


## AWS EC2

- t2.micro
  - Instance type (free tier)

>>>

## AWS VPC: Features

- EC2 (server) + VPC (network) is a major combination
- A VPC can have multiple AZs


## AWS VPC: Keywords

- IGW: Internet gateway
  - Let the VPC connect to the internet
- NGW: NAT gateway
- Subnet
  - Public Subnet
  - Private Subnet
- Route table
- Router
- VPC Peering
- Endpoints for S3
- Elastic IP
  - Reachable IPv4 address from the internet
  - After you get the Elastic IP, you must assign it to your EC2 instance

>>>

## AWS VPC: Config Example 1

- Internet -(IGW)- VPC > AZ (has Subnets)
  - IGW > Public Subnet > t2.micro Instance
  - IGW > Public Subnet > NGW > Private Subnet > DB

## AWS VPC: Config Example 2

- Internet - (ELB)
  - EC2 1 in AZ 1 -> RDS 1 -> RDS 2 (replicate of RDS 1)
  - EC2 2 in AZ 2 -> RDS 1 -> RDS 2 (replicate of RDS 1)



>>>

## AWS + Laravel

- Launch Elastic Beanstalk env
- Bundle Laravel app into .zip
- Upload & deploy .zip on EB console
- Configure doc root path
- Add DB Instance
- Configure /database.php
- Bundle & Deploy again

>>>

## AWS + Laravel: Refs

- https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/php-laravel-tutorial.html

>>>

## AWS + Laravel:

- A. Use AWS Beanstalk
  - Beanstalk -> My Code
- B. Deploy the Laravel on the  EC2 directly
  - Install LAMP, Composer manually with SSH
  - Host Infra -> OS -> Application Server -> HTTP Server -> My Code

>>>


## AWS + Laravel: References
- Official
  - https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/php-laravel-tutorial.html
- dev.io
  - https://dev.classmethod.jp/articles/elastic-beanstalk-laravel-deploy/
- Qiita EC2 + RDS
  - https://qiita.com/nakm/items/0bcc6564538a0604b2ce
- Qiita
  - https://qiita.com/masataka715/items/6e46f1f5e53bdff6cd3d
- Qiita
  - https://qiita.com/atto/items/e1effd28c212c3829cb0

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
- Terraform

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

>>>

## SQL

- DML: Data Manipulation Language
- DDL: Data Definition Language
  - e.g. CREATE, ALTER, DROP
- DCL: Data Control Language
  - Define DB Authorization

>>>

## Distributed DB

- 

>>>

## Transaction

>>>

## RDB

>>>

## ER

---

# Operating System

>>>

## Mutual Exclusion

>>>


## Automaton

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
- Spring
- Spring Review

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

## Redundancy: Number of 

- DMR: Dual Modular Redundancy
- TMR: Triple Modular Redundancy

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

>>>

## Maintenance

- 定期メンテナンス
- 緊急メンテナンス
- 無停止メンテナンス

---

# Network

>>>

## Network: MISC

- NFS: Network File System

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


## Encrytion

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

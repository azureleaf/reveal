# Study Notes for Coding

---

# ToC

>>>

- [Study Notes for Coding](#study-notes-for-coding)
- [ToC](#toc)
- [AWS](#aws)
  - [Products: Computing](#products-computing)
  - [Products: Storage](#products-storage)
  - [Products: Management](#products-management)
  - [Products: Management](#products-management-1)
  - [CS Books](#cs-books)
  - [AWS: Networking](#aws-networking)
  - [AWS: MISC](#aws-misc)
  - [AWS: MISC](#aws-misc-1)
  - [AWS + Laravel](#aws--laravel)
  - [AWS + Laravel: Refs](#aws--laravel-refs)
  - [AWS + Laravel:](#aws--laravel-1)
  - [AWS + Laravel: References](#aws--laravel-references)
- [Backends](#backends)
  - [IaC: What’s this?](#iac-whats-this)
  - [IaC: Products](#iac-products)
  - [Search](#search)
  - [Big Data](#big-data)
  - [Connection](#connection)
  - [Server](#server)
  - [Server Types](#server-types)
  - [Monitoring: Services](#monitoring-services)
  - [Monitoring: CloudWatch](#monitoring-cloudwatch)
  - [Monitoring](#monitoring)
  - [Monitoring Servers](#monitoring-servers)
  - [Monitoring: MISC](#monitoring-misc)
  - [Monitoring: Visualization](#monitoring-visualization)
  - [TTFB](#ttfb)
  - [Server Product](#server-product)
  - [Deployment Env.](#deployment-env)
- [DB](#db)
  - [DB MISC](#db-misc)
  - [SQL](#sql)
- [Software Engineering](#software-engineering)
  - [Dev.](#dev)
  - [Agile Dev. vs Waterfall Dev.](#agile-dev-vs-waterfall-dev)
  - [SCRUM](#scrum)
  - [Design Pattern: Web](#design-pattern-web)
  - [Design Pattern](#design-pattern)
  - [CI/CD Tools: Products](#cicd-tools-products)
  - [CI/CD Tools: Why necessary?](#cicd-tools-why-necessary)
- [Testing](#testing)
- [Gaming](#gaming)
  - [Data format used for server-client comm.](#data-format-used-for-server-client-comm)
  - [MISC](#misc)
  - [Maintenance](#maintenance)
- [Network](#network)
  - [Network: MISC](#network-misc)
  - [TCP / IP Model](#tcp--ip-model)
  - [OSI Model](#osi-model)
  - [Tools](#tools)
  - [TCP / IP](#tcp--ip)
- [Virtualization](#virtualization)
- [Tools](#tools-1)
- [Computer Architecture](#computer-architecture)
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

# AWS

>>>

## Products: Computing

- EC2
  - EC2 / ELB
- Lightsail
- Lambda
- ECS
- EKS
- Elastic Beanstalk
- Fargate

>>>

## Products: Storage

- S3
- EFS: Elastic File System
- RDS
- DynamoDB
- ElasiCache
- RedShift

>>>

## Products: Management

- CloudWatch
- LB: LoadBalancing

>>>

## Products: Management
- CloudWatch
- Load Balancing
- Application LB
- Network LB
- Classic LB


>>>


## CS Books

- Readable Code
- Refactoring
- Algorithm
- Network
- Computer Architecture

---

## AWS: Networking
- CloudFront
- VPC: Virtual Private Cloud
- selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways
- AWS > VPC > Public Subnet + Private Subnet
- API Gateway

>>>

## AWS: MISC
- AWS Athena
- Search S3 storage with queries
- AWS Glue
- AWS Lightsail
- AWS Elastic Beanstalk
- Amazon SNS: Simple Notification Service
- Amazon SQS: Simple Query Service
- Aurora

>>>

## AWS: MISC

- AWS cli

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

# Backends

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

## Server

- LAMP: Linux Apache MySQL PHP/Python/Perl
- LEMP
- MEAN

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

## TTFB

- DNS
- Connect
- SSL
- Send
- Wait
- Receive

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

---

# Testing

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

## TCP / IP Model

>>>

## OSI Model

>>>

## Tools

- Wireshark
- Firebug (dead?)

>>>

## TCP / IP

---

# Virtualization

>>>

# Tools

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


# Data Structure

>>>


>>>

# shell

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

## PHP

>>>

## PHP Tools
- artisan
- composer
- php.ini
- php -a
- php -f hello.php

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

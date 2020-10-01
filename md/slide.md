## Study Notes for Coding

---

## ToC

>>>

- [MISC](#misc)
  - [CS Books](#cs-books)
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
- [Operating System](#operating-system)
  - [Mutual Exclusion](#mutual-exclusion)
  - [Automaton](#automaton)
  - [`service` command](#service-command)
  - [File permission](#file-permission)
  - [User Group](#user-group)
    - [Primary Group vs Secondary Group](#primary-group-vs-secondary-group)
    - [bash](#bash)
    - [UID vs GID](#uid-vs-gid)
    - [ref.](#ref)
  - [chmod: ls -l](#chmod-ls--l)
    - [rwx](#rwx)
    - [`drwxr-xr-x`](#drwxr-xr-x)
  - [chmod: permission](#chmod-permission)
    - [Specify all the actions](#specify-all-the-actions)
    - [Specify one action](#specify-one-action)
  - [chmod: Use with find command](#chmod-use-with-find-command)
    - [Syntax](#syntax)
    - [Samples](#samples)
  - [chown](#chown)
  - [`xargs`](#xargs)
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
  - [Frequent Fault: Data Inconsistency](#frequent-fault-data-inconsistency)
    - [Solution](#solution)
  - [Frequent Fault: High Load to the server](#frequent-fault-high-load-to-the-server)
    - [Solution](#solution-1)
  - [Frequent Fault: DB size gets enormous](#frequent-fault-db-size-gets-enormous)
    - [Solution](#solution-2)
- [VR](#vr)
  - [Virtual Cast](#virtual-cast)
  - [VR](#vr-1)
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
  - [Tools](#tools-1)
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
- [GAS](#gas)
  - [What can GAS do?](#what-can-gas-do)
  - [GAS Limitations for the free-tier users](#gas-limitations-for-the-free-tier-users)

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
  - rwx (owner), rwx (group), rx (others)
- `chmod 664 /var/www`
  - rw (owner), rw (group), r (others)
- `chmod -R 775 /var`
  - Change for all the files in the dir **Recursively **
- `chmod 2775 /var/www`
  - Here "2" digit is for `setgid` (set group ID)


### Specify one action

- `u` User (owner)
- `g` Group
- `o` Other
- `a` All (user, group, other)
- `chmod g+x /var/www`
  - Add permission
- `chmod ugo-wx /var/www`
  - Revoke permission

>>>

## chmod: Use with find command

Find command takes "action" to execute the commands

### Syntax

- `{} +`

### Samples

- `find . -type f -exec chmod 600 {} +`
- `find . -type f | xargs chmod 600`
- `find /var/www -type d -exec sudo chmod 2775 {} \;`
- `find /var/www -type f -exec sudo chmod 0664 {} \;`



>>>

## chown

- `chown john /var/www`
- `chown john -R var`: All the files in the dir
- `chown john:staff /var/www`: Owner is john, group is staff

>>>

## `xargs`

- 

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
- Concurrent Access (同時アクセス数)
  - like 10k - 100k, for example

>>>

## Maintenance

- 定期メンテナンス
- 緊急メンテナンス
- 無停止メンテナンス

>>>

## Frequent Fault: Data Inconsistency

- Happens due to the many concurrent accesses to the DB

### Solution

- Lock the DB
  - However, the range of lock must be minimum, or other users will suffer from slow performance

>>>

## Frequent Fault: High Load to the server

### Solution

- Don't forget to use INDEX on the DB
- Integrate multiple SELECT queries into one

>>>

## Frequent Fault: DB size gets enormous

### Solution

- Don't save the unnecessary logs




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

---

# GAS

>>>

## What can GAS do?

- [【保存版】初心者向け実務で使えるGoogle Apps Script完全マニュアル](https://tonari-it.com/google-apps-script-manual/)

- Web Scraping
- [**Publish the website**](https://developers.google.com/apps-script/guides/web)
- Sum up the time duration of the Calendar events in the Spread Sheet
- Generate the chart automatically from the Spreadsheet
- **Connect to DB via JDBC**

>>>

## GAS Limitations for the free-tier users

[Quotas for Google Services](https://developers.google.com/apps-script/guides/services/quotas)

- Max of the running time: 6min
  - lengthy code is impossible to exec
- Daily quotas
  - 250 doc creation
  - 250 spreadsheet created
  - 100 mail recipients
  - 20000 R/W of the emails
  - 10000 JDBC connections
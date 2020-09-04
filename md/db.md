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

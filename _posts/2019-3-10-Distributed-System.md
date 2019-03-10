---
layout: post
title: Distributed System In One Lesson
date: 2019-03-09
category: Distributed System
---

Distributed System is a collection of independent computers that appear to the users as one computer.

**1. Three Characteristics**
* Operate concurrently
* Fail independently
* Do not share a global clock

**2. What will be covered**
* Storage : HDFS
* Computation: Hadoop, Spark
* Synchronization
* Consensus
* Messaging

**3. Distributed Storage**
* Read replication : Consistency (high read workload)
* Sharding : Split workload based on the key (deal with write workload)
* Consistent Hashing (Dynamo Paper)
    There are configuration parameters typically used to set the **consistency levels of distributed system**. Generally speaking, if the system has configuration R + W > N, we get strong consistency. 
* CAP theorem
    consistency 
    availability
    partition tolerance
    The CAP theorem is a tool used to make system designers aware of the trade-offs while designing networked shared-data system.
    
**4. Distributed Transactions**
* ACID transactions
    + Atomic: the transaction completes completely or not at all. It involves following two operations.
    Abort - If a transaction aborts, changes made to database are not visible.
    Commit - If a transaction commits, changes made are visible.
    + Consistency: This means the integrity constraints must be maintained so that the database is consistent before and after the transaction.
    + isolation: This property ensures that multiple transactions can occur concurrently without leading to inconsistency of database state. Changes occurring in a particular transaction will not be visible to any other transactions until that particular change in that transactions is written to memory or has been committed.
    + Durability
* One transaction can be split into multiple tasks for parallelization, uneven workloads. 
* Responses to failure
    + write-off (throw away)
    + retry 
    + compensating action
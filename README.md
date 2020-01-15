# Patterns
## Lessons learnt while switching to a NoSQL store
```
Embed Versus Reference : Embed when you dont want to use the nested structure without reference of its parent. For e.g in a blog post , comments might be embedded if you dont want to do any order/ranking etc on individual comments to get a performance advantage.
```

## Initial Choices

 ```
 1. MongoDB
 2. Cassandra
 3. MySQL Cluster Sharding[Done by some MNCs , works but expensive]
 4. HBase
 5. Neo4j
 ```
 
 ## Useful Concepts in Database World
 
 ```
 Master Slave Replication
 Multi Master Setup to increase the throughput by scaling both reads and writes.
 Dont Read from Replica, causes a lot of replication lag issues. Issue Read/Writes on multi master setup.
 Always design with shard in mind. At some point you need horizontal scaling so do it from start only.
 By Replication solve the problem of data durability.
 Automatic Failover are nice to have.
 CAP Theorem : Can have two max but that is a blurry line in today's world.
 ```
 

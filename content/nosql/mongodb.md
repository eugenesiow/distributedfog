---
title: "MongoDB"
type: "article"
description: "MongoDB is a free and open-source cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with schemas. MongoDB is developed by MongoDB Inc., and is published under a combination of the GNU Affero General Public License and the Apache License."
tags: ["software","database","document"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{< listcard size="4" title="Cloud-based DBaaS" >}}
    {{<listlink "https://cloud.mongodb.com" "MongoDB Atlas">}}
    {{<listlink "https://www.mlab.com/" "mLab">}}
    {{<listlink "https://scalegrid.io/" "ScaleGrid">}}
{{< /listcard >}}

{{< listcard size="4" title="Visualisation" >}}
    {{<listlink "https://robomongo.org/" "Robo 3T">}}
    {{<listlink "https://www.metabase.com/" "Metabase">}}
    {{<listlink "https://slamdata.com/solution/mongodb-analytics/" "Slam Data">}}
    {{<listlink "https://redash.io/" "Redash">}}
{{< /listcard >}}

{{% card size="8" small="Wikipedia" %}}
### Features
##### Ad hoc queries
MongoDB supports field, range queries, regular expression searches. Queries can return specific fields of documents and also include user-defined JavaScript functions. Queries can also be configured to return a random sample of results of a given size.

##### Indexing
Fields in a MongoDB document can be indexed with primary and secondary indices.

##### Replication
MongoDB provides high availability with replica sets. A replica set consists of two or more copies of the data. Each replica set member may act in the role of primary or secondary replica at any time. All writes and reads are done on the primary replica by default. Secondary replicas maintain a copy of the data of the primary using built-in replication. When a primary replica fails, the replica set automatically conducts an election process to determine which secondary should become the primary. Secondaries can optionally serve read operations, but that data is only eventually consistent by default.

##### Load balancing
MongoDB scales horizontally using sharding. The user chooses a shard key, which determines how the data in a collection will be distributed. The data is split into ranges (based on the shard key) and distributed across multiple shards. (A shard is a master with one or more slaves.). Alternatively, the shard key can be hashed to map to a shard – enabling an even data distribution.

##### File storage
MongoDB can be used as a file system with load balancing and data replication features over multiple machines for storing files.

##### Aggregation
MapReduce can be used for batch processing of data and aggregation operations.

The aggregation framework enables users to obtain the kind of results for which the SQL GROUP BY clause is used. Aggregation operators can be strung together to form a pipeline – analogous to Unix pipes. The aggregation framework includes the $lookup operator which can join documents from multiple documents, as well as statistical operators such as standard deviation.

##### Server-side JavaScript execution
JavaScript can be used in queries, aggregation functions (such as MapReduce), and sent directly to the database to be executed.

##### Capped collections
MongoDB supports fixed-size collections called capped collections. This type of collection maintains insertion order and, once the specified size has been reached, behaves like a circular queue. [Read More](https://en.wikipedia.org/wiki/MongoDB)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.mongodb.com/" "MongoDB.com">}}
    {{<listlink "https://university.mongodb.com" "MongoDB University">}}
    {{<listlink "https://docs.mongodb.com/" "Docs">}}
    {{<listlink "http://meanjs.org/" "MEAN stack">}}
{{< /listcard >}}

{{< listcard size="4" title="Compatible Alternatives" >}}
    {{<listlink "https://www.percona.com/software/mongo-database/percona-server-for-mongodb" "Percona Server (formerly TokuMX)">}}
    {{<listlink "http://consus.io/" "Consus">}}
{{< /listcard >}}
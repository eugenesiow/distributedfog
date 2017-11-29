---
title: "Cassandra"
type: "article"
description: "Apache Cassandra is a free and open-source distributed NoSQL database management system designed to handle large amounts of data across many commodity servers, providing high availability with no single point of failure. Cassandra offers robust support for clusters spanning multiple datacenters, with asynchronous masterless replication allowing low latency operations for all clients."
tags: ["software","database","columnar","LSM"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{< listcard size="4" title="Cloud-based DBaaS" >}}
    {{<listlink "https://www.stratoscale.com/products/dbaas/" "Stratoscale">}}
    {{<listlink "https://www.instaclustr.com/solutions/managed-apache-cassandra/" "Instaclustr">}}
    {{<listlink "https://winguzone.com/" "Winguzone">}}
    {{<listlink "https://cloud.intuz.com/applications/cassandra/aws/how-to-use" "Intuz">}}
    {{<listlink "https://bitnami.com/" "Bitnami">}}
{{< /listcard >}}

{{% card size="4" small="Wikipedia" %}}
### History

Avinash Lakshman (one of the authors of Amazon's Dynamo) and Prashant Malik initially developed Cassandra at Facebook to power the Facebook inbox search feature. Facebook released Cassandra as an open-source project on Google code in July 2008. In March 2009 it became an Apache Incubator project. On February 17, 2010 it graduated to a top-level project.
{{% /card %}}

{{% card size="8" small="Wikipedia" %}}
### Features

##### Decentralized
Every node in the cluster has the same role. There is no single point of failure. Data is distributed across the cluster (so each node contains different data), but there is no master as every node can service any request.
##### Supports replication and multi data center replication
Replication strategies are configurable. Cassandra is designed as a distributed system, for deployment of large numbers of nodes across multiple data centers. Key features of Cassandra’s distributed architecture are specifically tailored for multiple-data center deployment, for redundancy, for failover and disaster recovery.
##### Scalability
Designed to have read and write throughput both increase linearly as new machines are added, with the aim of no downtime or interruption to applications.
##### Fault-tolerant
Data is automatically replicated to multiple nodes for fault-tolerance. Replication across multiple data centers is supported. Failed nodes can be replaced with no downtime.
##### Tunable consistency
Writes and reads offer a tunable level of consistency, all the way from "writes never fail" to "block for all replicas to be readable", with the quorum level in the middle.
##### MapReduce support
Cassandra has Hadoop integration, with MapReduce support. There is support also for Apache Pig and Apache Hive.
##### Query language
Cassandra introduced the Cassandra Query Language (CQL). CQL is a simple interface for accessing Cassandra, as an alternative to the traditional Structured Query Language (SQL). CQL adds an abstraction layer that hides implementation details of this structure and provides native syntaxes for collections and other common encodings. Language drivers are available for Java (JDBC), Python (DBAPI2), Node.JS (Helenus), Go (gocql) and C++. [Read More](https://en.wikipedia.org/wiki/Apache_Cassandra)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://cassandra.apache.org/" "Apache Cassandra">}}
    {{<listlink "https://github.com/apache/cassandra" "Github">}}
    {{<listlink "http://cassandra.apache.org/doc/latest/architecture/index.html" "Architecture">}}
    {{<listlink "http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.161.6751&rep=rep1&type=pdf" "Cassandra Paper">}}
{{< /listcard >}}

{{< listcard size="4" title="Compatible Alternatives" >}}
    {{<listlink "http://www.scylladb.com/" "ScyllaDB">}}
    {{<listlink "https://www.datastax.com/products/datastax-enterprise" "DataStax Enterprise">}}
{{< /listcard >}}
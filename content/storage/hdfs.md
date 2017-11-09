---
title: "HDFS"
full: "Hadoop Distributed File System"
type: "article"
description: "The Hadoop Distributed File System (HDFS) is a distributed file system designed to run on commodity hardware. HDFS is highly fault-tolerant and is designed to be deployed on low-cost hardware. HDFS provides high throughput access to application data and is suitable for applications that have large data sets. HDFS relaxes a few POSIX requirements to enable streaming access to file system data."
weight: 0
tags: ["storage","filesystem","cluster","linux","distributed","hadoop"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="apache.org" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="Depardon et al. (2013). Analysis of Six Distributed File Systems." %}}
||[HDFS](../hdfs)|[iRODS](../irods)|[Ceph](../ceph)|[GlusterFS](../glusterfs)|[Lustre](../lustre)|
|--- |--- |--- |--- |--- |--- |
|__Architecture__ |Centralized |Centralized| Distributed| Decentralized |Centralized|
|__Naming__| Index| Database| CRUSH| EHA| Index|
|__API__| CLI, FUSE, REST, API| CLI, FUSE, API| FUSE, mount, REST| FUSE, mount| FUSE|
|__Fault detection__| Fully connect| P2P| Fully connect| Detected| Manually|
|__System Availability__|No failover| No failover| High| High| Failover|
|__Data availability__|Replication| Replication| Replication| RAID-like| No|
|__Placement strategy__|Auto| Manual| Auto| Manual| No|
|__Replication__| Async| Sync| Sync| Sync| RAID-like|
|__Cache consistency__|WORM, lease| Lock| Lock| No| Lock|
|__Load balancing__| Auto| Manual| Manual| Manual| No|
{{% /card %}}


{{% card size="8" small="Wikipedia and apache.org" %}}
The HDFS is a distributed, scalable, and portable file system written in Java for the Hadoop framework. Some consider it to instead be a data store due to its lack of POSIX compliance, but it does provide shell commands and Java application programming interface (API) methods that are similar to other file systems. A Hadoop cluster has nominally a single namenode plus a cluster of datanodes, although redundancy options are available for the namenode due to its criticality. Each datanode serves up blocks of data over the network using a block protocol specific to HDFS. The file system uses TCP/IP sockets for communication. Clients use remote procedure calls (RPC) to communicate with each other.

HDFS stores large files (typically in the range of gigabytes to terabytes) across multiple machines. It achieves reliability by replicating the data across multiple hosts, and hence theoretically does not require redundant array of independent disks (RAID) storage on hosts (but to increase input-output (I/O) performance some RAID configurations are still useful). With the default replication value, 3, data is stored on three nodes: two on the same rack, and one on a different rack. Data nodes can talk to each other to rebalance data, to move copies around, and to keep the replication of data high. HDFS is not fully POSIX-compliant, because the requirements for a POSIX file-system differ from the target goals of a Hadoop application. The trade-off of not having a fully POSIX-compliant file-system is increased performance for data throughput and support for non-POSIX operations such as Append. [Read more](https://en.wikipedia.org/wiki/Apache_Hadoop#Hadoop_distributed_file_system)

### Assumptions and Goals

##### Hardware Failure
Hardware failure is the norm rather than the exception. An HDFS instance may consist of hundreds or thousands of server machines, each storing part of the file system’s data. The fact that there are a huge number of components and that each component has a non-trivial probability of failure means that some component of HDFS is always non-functional. Therefore, detection of faults and quick, automatic recovery from them is a core architectural goal of HDFS.

##### Streaming Data Access
Applications that run on HDFS need streaming access to their data sets. They are not general purpose applications that typically run on general purpose file systems. HDFS is designed more for batch processing rather than interactive use by users. The emphasis is on high throughput of data access rather than low latency of data access. POSIX imposes many hard requirements that are not needed for applications that are targeted for HDFS. POSIX semantics in a few key areas has been traded to increase data throughput rates.

##### Large Data Sets
Applications that run on HDFS have large data sets. A typical file in HDFS is gigabytes to terabytes in size. Thus, HDFS is tuned to support large files. It should provide high aggregate data bandwidth and scale to hundreds of nodes in a single cluster. It should support tens of millions of files in a single instance.

##### Simple Coherency Model
HDFS applications need a write-once-read-many access model for files. A file once created, written, and closed need not be changed. This assumption simplifies data coherency issues and enables high throughput data access. A MapReduce application or a web crawler application fits perfectly with this model. There is a plan to support appending-writes to files in the future.

##### “Moving Computation is Cheaper than Moving Data”
A computation requested by an application is much more efficient if it is executed near the data it operates on. This is especially true when the size of the data set is huge. This minimizes network congestion and increases the overall throughput of the system. The assumption is that it is often better to migrate the computation closer to where the data is located rather than moving the data to where the application is running. HDFS provides interfaces for applications to move themselves closer to where the data is located.

##### Portability Across Heterogeneous Hardware and Software Platforms
HDFS has been designed to be easily portable from one platform to another. This facilitates widespread adoption of HDFS as a platform of choice for a large set of applications. [Read more](https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html#Introduction)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://hadoop.apache.org/" "Apache Hadoop">}}
    {{<listlink "https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html#Introduction" "HDFS Architecture Guide">}}
    {{<listlink "https://hortonworks.com/" "Hortonworks Hadoop Sandbox">}}
    {{<listlink "http://ieeexplore.ieee.org/document/5496972/" "HDFS Paper">}}
    {{<listlink "http://hadoop.apache.org/docs/current/" "Hadoop Documentation">}}
    
{{< /listcard >}}
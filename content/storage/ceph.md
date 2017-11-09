---
title: "Ceph"
type: "article"
description: "Ceph is a free-software storage platform that implements object storage on a single distributed computer cluster, and provides interfaces for object-, block- and file-level storage. Ceph aims primarily for completely distributed operation without a single point of failure, scalable to the exabyte level, and freely available. As a result of its design, the system is both self-healing and self-managing, aiming to minimize administration time and other costs."
weight: 0
tags: ["storage","filesystem","cluster","distributed","object storage"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
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


{{% card size="8" small="ceph.com" %}}
Ceph’s object storage system offers a significant feature compared to many object storage systems available today: Ceph provides a traditional file system interface with POSIX semantics. Object storage systems are a significant innovation, but they complement rather than replace traditional file systems. As storage requirements grow for legacy applications, organizations can configure their legacy applications to use the Ceph file system too! This means you can run one storage cluster for object, block and file-based data storage.

Ceph’s file system runs on top of the same object storage system that provides object storage and block device interfaces. The Ceph metadata server cluster provides a service that maps the directories and file names of the file system to objects stored within RADOS clusters. The metadata server cluster can expand or contract, and it can rebalance the file system dynamically to distribute data evenly among cluster hosts. This ensures high performance and prevents heavy loads on specific hosts within the cluster.

<a href="http://docs.ceph.com/docs/master/cephfs/" target="_blank"><img src="/img/articles/cephfs.png" title="Ceph Architecture" style="width: 100%;"></a>

To run the Ceph Filesystem, you must have a running Ceph Storage Cluster with at least one Ceph Metadata Server running. Once you have a healthy Ceph Storage Cluster with at least one Ceph Metadata Server, you may create and mount your Ceph Filesystem. Ensure that you client has network connectivity and the proper authentication keyring. [Read more](http://docs.ceph.com/docs/master/cephfs/#using-cephfs)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://ceph.com/" "Ceph.com">}}
    {{<listlink "http://docs.ceph.com/docs/master/" "Documentation">}}
    {{<listlink "https://hal.inria.fr/hal-00789086" "Analysis of Six Distributed File Systems">}}
{{< /listcard >}}
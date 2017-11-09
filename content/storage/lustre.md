---
title: "Lustre"
type: "article"
description: "Lustre is a type of parallel distributed file system, generally used for large-scale cluster computing. The name Lustre is a portmanteau word derived from Linux and cluster. Lustre file system software is available under the GNU GPLv2 and provides high performance file systems for computer clusters ranging in size from small workgroup clusters to large-scale, multi-site clusters."
weight: 0
tags: ["storage","filesystem","cluster","linux","distributed"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia and opensfs.org" style="info">}}
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


{{% card size="8" small="Wikipedia" %}}
The Lustre file system is a open source, parallel file system that supports the requirements of leadership class HPC and Enterprise environments worldwide.  Lustre provides a POSIX compliant interface and scales to thousands of clients, petabytes of storage, and has demonstrated over a terabyte per second of sustained I/O bandwidth.  Many of the largest and most powerful supercomputers on Earth today are powered by the Lustre file system, including over 60% of the TOP100 sites.

##### Architecture

A Lustre file system has three major functional units:

- One or more metadata servers (MDS) nodes that has one or more metadata target (MDT) devices per Lustre filesystem that stores namespace metadata, such as filenames, directories, access permissions, and file layout. The MDT data is stored in a local disk filesystem. However, unlike block-based distributed filesystems, such as GPFS and PanFS, where the metadata server controls all of the block allocation, the Lustre metadata server is only involved in pathname and permission checks, and is not involved in any file I/O operations, avoiding I/O scalability bottlenecks on the metadata server. The ability to have multiple MDTs in a single filesystem is a new feature in Lustre 2.4, and allows directory subtrees to reside on the secondary MDTs, while 2.7 and later allow large single directories to be distributed across multiple MDTs as well.
- One or more object storage server (OSS) nodes that store file data on one or more object storage target (OST) devices. Depending on the server’s hardware, an OSS typically serves between two and eight OSTs, with each OST managing a single local disk filesystem. The capacity of a Lustre file system is the sum of the capacities provided by the OSTs.
- Client(s) that access and use the data. Lustre presents all clients with a unified namespace for all of the files and data in the filesystem, using standard POSIX semantics, and allows concurrent and coherent read and write access to the files in the filesystem. [Read more](https://en.wikipedia.org/wiki/Lustre_(file_system))
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://lustre.org/" "Lustre.org Community Portal">}}
    {{<listlink "http://opensfs.org/" "OpenSFS">}}
    {{<listlink "https://hal.inria.fr/hal-00789086" "Analysis of Six Distributed File Systems">}}
{{< /listcard >}}
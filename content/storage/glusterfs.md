---
title: "GlusterFS"
type: "article"
description: "GlusterFS is a scale-out network-attached storage file system. It has found applications including cloud computing, streaming media services, and content delivery networks. GlusterFS was developed originally by Gluster, Inc. and then by Red Hat, Inc., as a result of Red Hat acquiring Gluster in 2011. Red Hat Gluster Storage is a GlusterFS-based Red Hat Storage Server."
weight: 0
tags: ["storage","filesystem","cluster","distributed"]
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


{{% card size="8" small="gluster.org" %}}
GlusterFS is a scalable network filesystem suitable for data-intensive tasks such as cloud storage and media streaming. GlusterFS is free and open source software and can utilize common off-the-shelf hardware. Gluster is a software defined distributed storage that can scale to several petabytes. It provides interfaces for object, block and file storage. [Read more](http://docs.gluster.org/en/latest/)

##### Types of Volumes
Volume is the collection of bricks and most of the gluster file system operations happen on the volume. Gluster file system supports different types of volumes based on the requirements. Some volumes are good for scaling storage size, some for improving performance and some for both.
1. Distributed Glusterfs Volume
2. Replicated Glusterfs Volume
3. Distributed Replicated Glusterfs Volume
​4. Striped Glusterfs Volume
5. Distributed Striped Glusterfs Volume

##### FUSE
GlusterFS is a userspace filesystem. This was a decision made by the GlusterFS developers initially as getting the modules into linux kernel is a very long and difficult process.

Being a userspace filesystem, to interact with kernel VFS, GlusterFS makes use of FUSE (File System in Userspace). For a long time, implementation of a userspace filesystem was considered impossible. FUSE was developed as a solution for this. FUSE is a kernel module that support interaction between kernel VFS and non-privileged user applications and it has an API that can be accessed from userspace. Using this API, any type of filesystem can be written using almost any language you prefer as there are many bindings between FUSE and other languages. [Read more](http://docs.gluster.org/en/latest/Quick-Start-Guide/Architecture/)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.gluster.org/" "Gluster.org">}}
    {{<listlink "http://docs.gluster.org/en/latest/" "Documentation">}}
    {{<listlink "https://www.redhat.com/en/technologies/storage/gluster" "RedHat Gluster">}}
    {{<listlink "https://hal.inria.fr/hal-00789086" "Analysis of Six Distributed File Systems">}}
{{< /listcard >}}
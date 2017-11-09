---
title: "FusionFS"
type: "article"
description: "FusionFS is a distributed filesystem that co-exists with current parallel filesystems in High-End Computing, optimized for both a subset of HPC and Many-Task Computing workloads. FusionFS is a user-level filesystem that runs on the compute resource infrastructure, and enables every compute node to actively participate in the metadata and data management. Distributed metadata management is implemented using ZHT, a zero-hop distributed hashtable."
weight: 0
tags: ["storage","filesystem","cluster","distributed"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="datasys.cs.iit.edu" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="ceph.com" %}}
### Abstract
State-of-the-art, yet decades-old, architecture of high-performance computing systems has its compute and storage resources separated. It thus is limited for modern data-intensive scientific applications because every I/O needs to be transferred via the network between the compute and storage resources. In this paper we propose an architecture that hss a distributed storage layer local to the compute nodes. This layer is responsible for most of the I/O operations and saves extreme amounts of data movement between compute and storage resources. We have designed and implemented a system prototype of this architecture - which we call the FusionFS distributed file system - to support metadata-intensive and write-intensive operations, both of which are critical to the I/O performance of scientific applications. FusionFS has been deployed and evaluated on up to 16K compute nodes of an IBM Blue Gene/P supercomputer, showing more than an order of magnitude performance improvement over other popular file systems such as GPFS, PVFS, and HDFS. [Read more](http://www.mcs.anl.gov/publication/fusionfs-towards-supporting-data-intensive-scientific-applications-extreme-scale)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://datasys.cs.iit.edu/projects/FusionFS/" "Project Page">}}
    {{<listlink "http://ieeexplore.ieee.org/document/7004214/" "FusionFS Paper">}}
    {{<listlink "https://github.com/dongfangzhao/FusionFS-BluegeneP" "Github">}}
{{< /listcard >}}
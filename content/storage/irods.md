---
title: "iRODS"
full: "Integrated Rule-Oriented Data System"
type: "article"
description: "The integrated Rule-Oriented Data System (iRODS) is open source data management software used by research organizations and government agencies worldwide. iRODS is released as a production-level distribution aimed at deployment in mission critical environments. It virtualizes data storage resources, so users can take control of their data, regardless of where and on what device the data is stored. As data volumes grow and data services become more complex, iRODS is serving an increasingly important role in data management."
weight: 0
tags: ["storage","filesystem","cluster","distributed"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Github" style="info">}}
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


{{% card size="8" small="irods.org" %}}
iRODS, the Integrated Rule-Oriented Data System, is a state-of-the-art open source software system for addressing the key data management tasks that face users as the size and complexity of digital data collections continue to grow rapidly. Because the principal data management tasks are highly interrelated, rather than taking a piecemeal approach or addressing just a single task, the iRODS system takes a comprehensive approach to full data life cycle management.

At the same time, the system design is highly user-driven and avoids the pitfalls of a "one size fits all" design by building on a comprehensive generic platform with a highly configurable architecture. In addition, iRODS offers multiple paths to interoperation with outside systems such as repositories, interfaces, and applications. This lets users adapt iRODS to the details of their own environment in a wide range of production applications that can emphasize different aspects of data management in diverse domains.

### Core Competencies

- iRODS implements data virtualization, allowing access to distributed storage assets under a unified namespace, and freeing organizations from getting locked in to single-vendor storage solutions.
- iRODS enables data discovery using a metadata catalog that describes every file, every directory, and every storage resource in the iRODS Zone.
- iRODS automates data workflows, with a rule engine that permits any action to be initiated by any trigger on any server or client in the Zone.
- iRODS enables secure collaboration, so users only need to log in to their home Zone to access data hosted on a remote Zone.

[Read more](https://docs.irods.org/4.2.2/)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://irods.org/" "iRODS.org">}}
    {{<listlink "https://docs.irods.org/4.2.2/" "Documentation">}}
    {{<listlink "https://github.com/irods/irods" "Github">}}
    {{<listlink "https://hal.inria.fr/hal-00789086" "Analysis of Six Distributed File Systems">}}
{{< /listcard >}}
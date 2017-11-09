---
title: "CSI"
full: "Container Storage Interface"
type: "article"
description: "The goal of the Container Storage Interface (CSI) is to define and interface that will enable storage vendors to develop a plugin once and have it work across a number of container orchestration (CO) systems."
weight: 0
tags: ["storage","container"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="CSI community" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="CSI community" %}}
The CSI specification is an emerging specification that defines an interface along with the minimum operational and packaging recommendations for a storage provider (SP) to implement a CSI compatible plugin. The interface declares the RPCs that a plugin must expose: this is the primary focus of the CSI specification. Any operational and packaging recommendations offer additional guidance to promote cross-CO compatibility. 

### Initial Goals

The Container Storage Interface (CSI) will

- Enable SP authors to write one CSI compliant Plugin that “just works” across all COs that implement CSI.
- Define API (RPCs) that enable:
    - Dynamic provisioning and deprovisioning of a volume.
    - Attaching or detaching a volume from a node.
    - Mounting/unmounting a volume from a node.
    - Consumption of both block and mountable volumes.
    - Local storage providers (e.g., device mapper, lvm).
- Define plugin protocol RECOMMENDATIONS.
    - Describe a process by which a Supervisor configures a Plugin.
    - Container deployment considerations (CAP_SYS_ADMIN, mount namespace, etc.).

[Read more](https://github.com/container-storage-interface/spec/blob/master/spec.md)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://github.com/container-storage-interface/spec" "Specification Draft">}}
    {{<listlink "https://github.com/container-storage-interface" "Github">}}
{{< /listcard >}}
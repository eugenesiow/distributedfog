---
title: "SAN"
full: "Storage Area Network"
type: "article"
description: "A SAN is a network which provides access to consolidated, block level data storage. SANs are primarily used to enhance storage devices, such as disk arrays, tape libraries, and optical jukeboxes, accessible to servers so that the devices appear to the operating system as locally attached devices. A SAN typically has its own network of storage devices that are generally not accessible through the local area network (LAN) by other devices."
weight: 0
tags: ["storage"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="TechTarget" %}}
A storage-area network (SAN) is a dedicated high-speed network (or subnetwork) that interconnects and presents shared pools of storage devices to multiple servers.

A SAN moves storage resources off the common user network and reorganizes them into an independent, high-performance network. This allows each server to access shared storage as if it were a drive directly attached to the server. When a host wants to access a storage device on the SAN, it sends out a block-based access request for the storage device.

The main benefit to using a SAN is that raw storage is treated as a pool of resources that can be centrally managed and allocated on an as-needed basis. SANs are also highly scalable because additional capacity can be added as required.

The main disadvantages to SANs are cost and complexity. SAN hardware tends to be expensive, and building and managing a SAN requires a specialized skill set. [Read more](http://searchstorage.techtarget.com/definition/storage-area-network-SAN)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.redbooks.ibm.com/redbooks/pdfs/sg245470.pdf" "IBM Redbooks: Introduction to SANs">}}
    {{<listlink "https://en.wikipedia.org/wiki/Storage_area_network#Network_types" "Network Types">}}
{{< /listcard >}}
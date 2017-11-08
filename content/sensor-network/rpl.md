---
title: "RPL"
full: "Routing Protocol for Low power and Lossy Networks"
type: "article"
description: "RPL is the IPv6 Routing Protocol for Low-Power and Lossy Networks (LLN), which provides a mechanism whereby multipoint-to-point traffic from devices inside the LLN towards a central control point as well as point-to-multipoint traffic from the central control point to the devices inside the LLN are supported."
weight: 0
tags: ["protocol","wireless","routing","IPv6"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="RFC 6550" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="Network (Journal)" %}}
RPL is a distance vector routing protocol for LLNs that makes use of IPv6. Network devices running the protocol are connected in such a way that no cycles are present. For this purpose a Destination Oriented Directed Acyclic Graph (DODAG), which is routed at a single destination, is built. The RPL specification calls this specific node a DODAG root. The graph is constructed by the use of an Objective Function (OF) which defines how the routing metric is computed. In other words, the OF specifies how routing constraints and other functions are taken into account during topology construction.

The RPL specification defines four types of control messages for topology maintenance and information exchange. The first one is called DODAG Information Object (DIO) and is
the main source of routing control information. It may store information like the current Rank of a node, the current RPL Instance, the IPv6 address of the root, etc. The second one
is called a Destination Advertisement Object (DAO). It enables the support of down trac and is used to propagate destination information upwards along the DODAG. The third one is named DODAG Information Solicitation (DIS) and makes it possible for a node to require DIO messages from a reachable neighbor. The fourth type is a DAO-ACK and is sent by a DAO recipient in response to a DAO message. The RPL specification defines all four types of control messages as ICMPv6 information messages with a requested type of 155. [Read more](https://www.net.in.tum.de/fileadmin/TUM/NET/NET-2011-07-1/NET-2011-07-1_09.pdf)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://tools.ietf.org/html/rfc6550" "RFC 6550 RPL">}}
    {{<listlink "https://tools.ietf.org/html/rfc6553" "RFC 6553 RPL Datagrams Option">}}
    {{<listlink "https://www.net.in.tum.de/fileadmin/TUM/NET/NET-2011-07-1/NET-2011-07-1_09.pdf" "RPL Paper">}}
{{< /listcard >}}
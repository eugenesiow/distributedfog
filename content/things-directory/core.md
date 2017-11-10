---
title: "CoRE RD"
full: "Constrained RESTful Environments Resource Directory"
type: "article"
description: "In many M2M applications, direct discovery of resources is not practical due to sleeping nodes, disperse networks, or networks where multicast traffic is inefficient.  These problems can be solved by employing an entity called a Resource Directory (RD), which hosts descriptions of resources held on other servers, allowing lookups to be performed for those resources."
weight: 0
tags: ["specification", "interoperability","discovery"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="IETF.org Draft" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" %}}
### Introduction
The discovery of resources offered by a constrained server is very important in machine-to-machine applications where there are no humans in the loop and static interfaces result in fragility. The discovery of resources provided by an HTTP Web Server is typically called Web Linking ([RFC5988](https://tools.ietf.org/html/rfc5988)). The use of Web Linking for the description and discovery of resources hosted by constrained web servers is specified by the CoRE Link Format ([RFC6690](https://tools.ietf.org/html/rfc6690)). However, [RFC6690](https://tools.ietf.org/html/rfc6690) only describes how to discover resources from the web server that hosts them by querying /.well-known/core. In many M2M scenarios, direct discovery of resources is not practical due to sleeping nodes, disperse networks, or networks where multicast traffic is inefficient. These problems can be solved by employing an entity called a Resource Directory (RD), which hosts descriptions of resources held on other servers, allowing lookups to be performed for those resources.
{{% /card %}}

{{% card size="8" small="IEEE IoT Newsletter and Github" %}}
### Architecture
The resource directory architecture is illustrated below. A Resource Directory (RD) is used as a repository for Web Links ([RFC5988](https://tools.ietf.org/html/rfc5988)) about resources hosted on other web servers, which are called endpoints (EP). An endpoint is a web server associated with a scheme, IP address and port, thus a physical node may host one or more endpoints. The RD implements a set of REST interfaces for endpoints to register and maintain sets of Web Links (called resource directory registration entries), and for clients to lookup resources from the RD or maintain groups. Endpoints themselves can also act as clients. An RD can be logically segmented by the use of Domains. The domain an endpoint is associated with can be defined by the RD or configured by an outside entity. This information hierarchy is shown in at the bottom of the card.

~~~~
             Registration     Lookup, Group
              Interface        Interfaces
  +----+          |                 |
  | EP |----      |                 |
  +----+    ----  |                 |
                --|-    +------+    |
  +----+          | ----|      |    |     +--------+
  | EP | ---------|-----|  RD  |----|-----| Client |
  +----+          | ----|      |    |     +--------+
                --|-    +------+    |
  +----+    ----  |                 |
  | EP |----      |                 |
  +----+
                    Architecture
~~~~

A mechanism to discover an RD using CoRE Link Format ([RFC6690](https://tools.ietf.org/html/rfc6690)) is defined.

Endpoints proactively register and maintain resource directory registration entries on the RD, which are soft state and need to be periodically refreshed.

An endpoint is provided with interfaces to register, update and remove a resource directory registration entry. It is also possible for an RD to fetch Web Links from endpoints and add them as resource directory registration entries.

At the first registration of a set of entries, a "registration resource" is created, the location of which is returned to the registering endpoint. The registering endpoint uses this registration resource to manage the contents of the registration entry.

A lookup interface for discovering any of the Web Links held in the RD is provided using the CoRE Link Format. [Read more](https://tools.ietf.org/html/draft-ietf-core-resource-directory-12)

~~~~
               +------------+
               |   Domain   | <-- Name
               +------------+
                    |     |
                    |   +------------+
                    |   |   Group    | <-- Name, Scheme, IP, Port
                    |   +------------+
                    |     |
               +------------+
               |  Endpoint  |  <-- Name, Scheme, IP, Port
               +------------+
                     |
                     |
               +------------+
               |  Resource  |  <-- Target, Parameters
               +------------+
                        Information Hierachy
~~~~

{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://tools.ietf.org/html/draft-ietf-core-resource-directory-12" "Draft 12">}}
    {{<listlink "https://github.com/core-wg/resource-directory" "Github">}}
    {{<listlink "https://github.com/JelmerT/coap-rd" "Server Implementation">}}
{{< /listcard >}}
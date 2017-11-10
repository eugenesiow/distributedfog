---
title: "Hypercat"
type: "article"
description: "The Hypercat specification allows Internet of Things (IoT) clients to discover information about IoT assets over the web. With Hypercat developers can write applications that will work across many servers, breaking down the walls between vertical silos."
weight: 0
tags: ["specification", "interoperability","discovery","search"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Hypercat.io" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Reference Server ([Code](https://github.com/HyperCatIoT/hc2-server))

- GET, PUT, POST, DELETE of items
- Multi-search
- Geo search
- Lexicographic search
- Simple search
- Prefix search
- Authentication
{{% /card %}}

{{% card size="4" %}}
### PIOTRe

[PIOTRe](../../decentralisation/piotre) is a Personal IoT Repository that allows applications to be built on interoperable and efficient semantic database technology for deployment on lightweight IoT devices.

PIOTRe provides a means of sharing metadata globally with HyperCat.
{{% /card %}}

{{% card size="8" small="IEEE IoT Newsletter and Github" %}}
HyperCat is an initiative that aims to address the issue of semantic interoperability for IoT. A major objective of the programme was to address interoperability and specifically how interoperability could be achieved between data hubs in different domains: this led to HyperCat1, a standard for representing and exposing Internet of Things data hub catalogues over web technologies, to improve data discoverability and interoperability. The idea is to enable distributed data repositories (data hubs) to be used jointly by applications by making it possible to query their catalogues in a uniform machine readable format. This enables the creation of "knowledge graphs" of available datasets across multiple hubs that applications can exploit and query to identify and access the data they need, whatever the data hub in which they are held.

This is achieved, in the specification, through employing the same principles on which linked data and the web are built: data accessible through standard web protocols and formats (HTTPS, JSON, REST, etc.), the identification of resources through URIs, and the establishment of common, shared semantics for the descriptors of datasets.

HyperCat represents a pragmatic starting point to solving the issues of managing multiple data sources, aggregated into multiple data hubs, through linked data and web approaches. It incorporates a lightweight, JSON-based approach based on a technology stack used by a large population of web developers and as such offers a very low barrier to entry, thereby encouraging the growth of IoT ecosystems. [Read more](https://iot.ieee.org/newsletter/january-2016/hypercat-resource-discovery-on-the-internet-of-things.html)

### Hypercat Catalogue
HyperCat is an open, lightweight JSON-based hypermedia catalogue format for exposing collections of URIs. Each HyperCat catalogue may expose any number of URIs, each with any number of RDF-like triple statements about it. HyperCat is simple to work with and allows developers to publish linked-data descriptions of resources.

HyperCat is designed for exposing information about IoT assets over the web. It allows a server to provide a set of resources to a client, each with a set of semantic annotations. Implementers are free to choose or invent any set of annotations to suit their needs. A set of best practices and tools are currently under development. Where implementers choose similar or overlapping semantics, the possibilities for interoperability are increased. Each HyperCat catalogue lists and annotates any number of URIs (which typically identify data sources), each having a set of relation-value pairs (metadata) associated with it. In this way, HyperCat allows a server to provide a set of resources to a client, each with a set of semantic annotations.

Importantly, there are a small set of core mandatory metadata relations which a valid HyperCat catalogue must include: beyond this, implementers are free to use any set of annotations to suit their needs. One important non-mandatory relation2 in the specification allows a data feed to be associated with an RDFS class, thereby linking to the LOD cloud. With HyperCat, developers can write apps that will access data from many hubs, aiming to break down the walls between today's vertical silos. [Read more](https://hypercatiot.github.io/)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.hypercat.io/" "Hypercat.io">}}
    {{<listlink "http://www.hypercat.io/standard.html" "Hypercat 3.00 Specification">}}
    {{<listlink "https://github.com/HyperCatIoT" "Github">}}
{{< /listcard >}}
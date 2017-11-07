---
title: "PIOTRe"
full: "Personal Internet of Things Repository"
type: "article"
description: "PIOTRe is a Personal IoT Repository that allows applications to be built on interoperable and efficient semantic database technology for deployment on lightweight IoT devices. The name PIOTRe is derived from the name Peter meaning 'stone' or 'rock' and is the foundation for personal IoT device repositories."
tags: ["software","decentralised","distributed","fog computing","S2S","eywa","SPARQL"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="cisco.com" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="cisco.com" %}}
### Architecture
<a href="https://github.com/eugenesiow/PIOTRe" target="_blank"><img src="/img/articles/piotre.png" title="PIOTRe Architecture"></a>
{{% /card %}}

{{% card size="8" small="github.com/eugenesiow/piotre-web" %}}
##### PIOTRe
PIOTRe is a Personal IoT Repository based on sparql2sql, sparql2stream and sparql2fed technologies. The name PIOTRe is also derived from the name Peter meaning "stone" or "rock" and is the foundation for applications built on interoperable and efficient database technology on lightweight IoT devices.

PIOTRe essentially consists of a sink for IoT data streams which flows to an events stream and a historical store and allows applications to be built on top with any programming language and framework. Historical data can be queried via a HTTP SPARQL endpoint while queries on streaming data can be registered most efficiently via the underlying ZeroMQ sockets by publishing streaming SPARQL query to a broker.

##### PIOTRe Web
PIOTRe-web is a frontend for PIOTRe with the goal of making it effortless to add a data source, create a mapping, build an app on top of it and publish the metadata.

PIOTRe-web has a WYSIWYG editor for mappings in S2SML making it easy to create mappings which enhance interoperability with other PIOTRe and semantic web systems.

##### PIOTRe Paper Abstract
Resource-constrained Internet of Things (IoT) devices like Raspberry Pis’, with specific performance optimisation, can serve as interoperable personal Linked Data repositories for IoT applications. In this demo paper we describe PIOTRe, a personal datastore that utilises our sparql2sql query translation technology on Pis’ to process, store and publish IoT time-series historical data and streams. We demonstrate with PIOTRe in a smart home scenario: a real-time dashboard that utilises RDF stream processing, a set of descriptive analytics visualisations on historical data, a framework for registering stream queries within a local network and a means of sharing metadata globally with HyperCat and Web Observatories.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://eugenesiow.com/publications/piotre/" "PIOTRe Paper">}}
    {{<listlink "https://github.com/eugenesiow/piotre-web" "PIOTRe frontend">}}    
{{< /listcard >}}
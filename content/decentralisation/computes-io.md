---
title: "Computes.io"
type: "article"
description: "Computes.io is a mesh networked, distributed supercomputing platform powered by IPFS. Each node on the mesh network acts as both a core and kernel, meaning that each node can perform computations for other machines as well as request computations from itself and other machines."
tags: ["software","decentralised","distributed","IPFS"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="computes.io" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" %}}
Computes.io is a [distributed supercomputer mesh network](https://blog.computes.io/distributed-supercomputer-mesh-network-ec8fc6a2c927). Each node on the mesh network acts as both a [core and kernel](https://blog.computes.io/distributed-computed-centralized-vs-decentralized-c1d21202bde8) — meaning that each node can perform Javascript computations for other machines as well as request computations from itself and other machines. Computes.io uses IPFS’ pubsub capabilities to create a signaling and messaging engine for [distributing computations](https://blog.computes.io/decentralized-distributed-edge-computing-comes-to-computes-io-396aa062bc85) across the mesh network to any machine with available resources.

IPFS pubsub is similar to the MQTT pubsub protocols used in most Internet of Things (IoT) applications and devices but with one major difference. IPFS does not require a dedicated message broker to store and forward IoT messages. IPFS nodes form a mesh network and can communicate with or without the Internet — no message brokers required!

computes.io can distribute javascript applications (via text strings, Gist URLs, IPFS hashes, and/or NodeJS NPM modules) and data to any node on the mesh network. Computations consist of realtime requests and/or massively parallel operations — even coordinated binary app executions. [Read More](blog.computes.io)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://computes.io/" "Computes.io">}}
    {{<listlink "https://blog.computes.io/" "Blog">}}
    {{<listlink "https://github.com/computes" "Github">}} 
{{< /listcard >}}
---
title: "Hermes"
type: "article"
description: "Hermes is a distributed, eventbased middleware platform. Hermes follows a type- and attribute-based publish/subscribe model that places particular emphasis on programming language integration by supporting type-checking of event data and event type inheritance. To handle dynamic, large-scale environments, Hermes uses peer-to-peer techniques for autonomic management of its overlay network of event brokers and for scalable event dissemination."
tags: ["software","research","distributed"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Pietzuch (2004). Hermes: A scalable event-based middleware. PhD Thesis." style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="Pietzuch (2004). Hermes: A scalable event-based middleware. PhD Thesis." %}}

A primary feature of the Hermes event-based middleware is scalability, as it is targeted at the development of large-scale distributed systems. Hermes includes two content-based routing algorithms to disseminate events from event publishers to subscribers. The type-based routing algorithm only supports subscriptions depending on the event type of event publications. It is comparable to a topic-based publish/subscribe service but differs by observing inheritance relationships between event types. The second algorithm is type- and attribute-based routing, which extends type-based routing with content-based filtering on event attributes in publications. In both algorithms, event-type specific advertisements, introduced in Section 3.3.3, are sent by publisher-hosting brokers to set up routing state. Advertisements are not broadcast to all event brokers, but instead event brokers can act as special rendezvous nodes that guarantee that event subscriptions and advertisements join in the network in order to form valid event dissemination trees.

Both routing algorithms use a distributed hash table to set up state for event dissemination trees. The distributed hash table functionality is implemented by a peer-to-peer routing substrate, called Pan, formed by the event brokers in Hermes. Pan is an extended implementation of the Pastry routing substrate. The advantage of such peer-to-peer overlay network are threefold: first, the overlay network can react to failure by changing its topology and thus adding fault-tolerance to Hermes. Second, the peer-to-peer routing substrate that manages the overlay network is responsible for handling membership of event brokers in a Hermes deployment. Third, the discovery of rendezvous nodes, which must be well-known in the
network, is simplified by the standard properties of the distributed hash table.

The bottom layer is the physical network with routers and links that Hermes is deployed in. The middle layer constitutes the peer-to-peer overlay network that offers a distributed hash table abstraction. The top layer consists of multiple event dissemination trees that are constructed by Hermes to realise the event-based middleware service. When a message is routed using the peer-to-peer overlay network, a callback to the upper layer is performed at every hop, that allows the event broker to process the message by altering it or its own state. In addition to scalable event dissemination, Hermes supports event typing, the creation of event type hierarchies through inheritance, and generic, supertype event subscriptions. This enhances its integration with current object-oriented programming languages such as Java or C++.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-590.pdf" "Hermes: A scalable event-based middleware">}}
{{< /listcard >}}
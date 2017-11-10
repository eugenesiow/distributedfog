---
title: "DDS"
full: "Data Distribution Service"
type: "article"
description: "The Data Distribution Service for real-time systems (DDS) is an Object Management Group (OMG) machine-to-machine (sometimes called middleware) standard that aims to enable scalable, real-time, dependable, high-performance and interoperable data exchanges using a publish–subscribe pattern. DDS addresses the needs of applications like financial trading, air-traffic control, smart grid management, and other big data applications. The standard is used in applications such as smartphone operating systems, transportation systems and vehicles, software-defined radio, and by healthcare providers. DDS was promoted for use in the Internet of things."
tags: ["protocol","middleware"]
weight: 0
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="Wikipedia" %}}
DDS is networking middleware that simplifies complex network programming. It implements a publish–subscribe pattern for sending and receiving data, events, and commands among the nodes. Nodes that produce information (publishers) create "topics" (e.g., temperature, location, pressure) and publish "samples". DDS delivers the samples to subscribers that declare an interest in that topic.

DDS handles transfer chores: message addressing, data marshalling and demarshalling (so subscribers can be on different platforms from the publisher), delivery, flow control, retries, etc. Any node can be a publisher, subscriber, or both simultaneously.

DDS supports mechanisms that go beyond the basic publish-subscribe model. The key benefit is that applications that use DDS for their communications are decoupled. Little design time needs be spent on handling their mutual interactions. In particular, the applications never need information about the other participating applications, including their existence or locations. DDS transparently handles message delivery without requiring intervention from the user applications, including:

- determining who should receive the messages
- where recipients are located
- what happens if messages cannot be delivered

DDS allows the user to specify quality of service (QoS) parameters to configure discovery and behavior mechanisms up-front. By exchanging messages anonymously, DDS simplifies distributed applications and encourages modular, well-structured programs. DDS also automatically handles hot-swapping redundant publishers if the primary fails. Subscribers always get the sample with the highest priority whose data is still valid (that is, whose publisher-specified validity period has not expired). It automatically switches back to the primary when it recovers, too.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://portals.omg.org/dds/" "DDS Portal">}}
    {{<listlink "http://www.omg.org/news/whitepapers/index.htm#DDS" "Whitepapers">}}
    {{<listlink "http://www.omg.org/hot-topics/iot-standards.htm" "DDS Industrial IoT">}}
{{< /listcard >}}
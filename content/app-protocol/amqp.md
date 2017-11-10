---
title: "AMQP"
full: "Advanced Message Queuing Protocol"
type: "article"
description: "The Advanced Message Queuing Protocol (AMQP) is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing (including point-to-point and publish-and-subscribe), reliability and security."
tags: ["protocol","middleware","specification"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Architecture
<a href="https://www.amqp.org/product/architecture" target="_blank"><img src="/img/articles/amqp-archi.png" title="Network Protocol" style="width: 100%;"></a>
{{% /card %}}

{{% card size="4" %}}
### Network Protocol
<a href="https://www.amqp.org/product/architecture" target="_blank"><img src="/img/articles/amqp-protocol.png" title="Network Protocol" style="width: 100%;"></a>
{{% /card %}}

{{% card size="8" small="spring.io" %}}
AMQP is a binary, application layer protocol, designed to efficiently support a wide variety of messaging applications and communication patterns. It provides flow controlled, message-oriented communication with message-delivery guarantees such as at-most-once (where each message is delivered once or never), at-least-once (where each message is certain to be delivered, but may do so multiple times) and exactly-once (where the message will always certainly arrive and do so only once), and authentication and/or encryption based on SASL and/or TLS. It assumes an underlying reliable transport layer protocol such as Transmission Control Protocol (TCP).

The AMQP specification is defined in several layers: (i) a type system, (ii) a symmetric, asynchronous protocol for the transfer of messages from one process to another, (iii) a standard, extensible message format and (iv) a set of standardised but extensible 'messaging capabilities.'

##### Advantages of AMQP over JMS

AMQP is often compared to JMS (Java Message Service), the most common messaging system in the Java community. A limitation of JMS is that the APIs are specified, but the message format is not. Unlike AMQP, JMS has no requirement for how messages are formed and transmitted. Essentially, every JMS broker can implement the messages in a different format. They just have to use the same API.

AMQP publishes its specifications in a downloadable XML format. This availability makes it easy for library maintainers to generate APIs driven by the specs while also automating construction of algorithms to marshal and demarshal messages. These advantages and the openness of the spec have inspired the creation of multiple brokers that support AMQP, including:

- RabbitMQ
- ActiveMQ
- Qpid

##### AMQP and JMS terminology

- JMS has queues and topics. A message sent on a JMS queue is consumed by no more than one client. A message sent on a JMS topic may be consumed by multiple consumers. AMQP only has queues. While AMQP queues are only consumed by a single receiver, AMQP producers don't publish directly to queues. A message is published to an exchange, which through its bindings may get sent to one queue or multiple queues, effectively emulating JMS queues and topics.
- JMS and AMQP have an equivalent message header, providing the means to sort and route messages.
- JMS and AMQP both have brokers responsible for receiving, routing, and ultimately dispensing messages to consumers.
- AMQP has exchanges, routes, and queues. Messages are first published to exchanges. Routes define on which queue(s) to pipe the message. Consumers subscribing to that queue then receive a copy of the message. If more than one consumer subscribes to the same queue, the messages are dispensed in a round-robin fashion.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.amqp.org/" "AMQP Home">}}
    {{<listlink "https://spring.io/understanding/AMQP" "Spring Understanding AMQP">}}
    {{<listlink "http://activemq.apache.org/" "AcitveMQ">}}
    {{<listlink "https://www.rabbitmq.com/protocol.html" "RabbitMQ">}}
{{< /listcard >}}
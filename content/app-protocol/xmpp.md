---
title: "XMPP"
full: "Extensible Messaging and Presence Protocol"
type: "article"
description: "XMPP is a communications protocol for message-oriented middleware based on XML. It enables the near-real-time exchange of structured yet extensible data between any two or more network entities."
tags: ["protocol", "XML"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[IoT Deployment](https://www.researchgate.net/profile/Enrico_Ferrera/publication/299445607_XMPP-based_Network_Management_Infrastructure_for_Agile_IoT_Application_Deployment_and_Configuration/links/56f8059d08ae7c1fda30721e.pdf), [Lightweight IoT Pub/Sub](http://ieeexplore.ieee.org/abstract/document/8013677/), [SmartObjects with mDNS](https://opus4.kobv.de/opus4-btu/frontdoor/index/index/docId/3850), [Cryptographic Hashes](https://xmpp.org/extensions/xep-0300.html)
{{% /card %}}

{{% card size="4" %}}
 XMPP supports different communication patterns, such as [Request/Response](https://xmpp.org/uses/iot/patterns#requestresponse), [Asynchronous Messaging](https://xmpp.org/uses/iot/patterns#asynchronous-messaging), [Publish/Subscribe](https://xmpp.org/uses/iot/patterns#publishsubscribe), [Event subscription (Observe)](https://xmpp.org/uses/iot/patterns#event-subscription-observe) and [Delayed delivery](https://xmpp.org/uses/iot/patterns#delayed-delivery). XMPP also has support for different Quality of Service levels for messaging.
{{% /card %}}

{{% card size="8" small="xmpp.org" %}}
XMPP is the Extensible Messaging and Presence Protocol, a set of open technologies for instant messaging, presence, multi-party chat, voice and video calls, collaboration, lightweight middleware, content syndication, and generalized routing of XML data.

XMPP was originally developed in the Jabber open-source community to provide an open, decentralized alternative to the closed instant messaging services at that time. XMPP offers several key advantages over such services:

##### Open
The XMPP protocols are free, open, public, and easily understandable; in addition, multiple implementations exist in the form clients, servers, server components, and code libraries.

##### Standards Based
The Internet Engineering Task Force (IETF) has formalized the core XML streaming protocols as an approved instant messaging and presence technology. The XMPP specifications were published as RFC 3920 and RFC 3921 in 2004, and the XMPP Standards Foundation continues to publish many XMPP Extension Protocols. In 2011 the core RFCs were revised, resulting in the most up-to-date specifications ([RFC 6120](https://tools.ietf.org/html/rfc6120), [RFC 6121](https://tools.ietf.org/html/rfc6121), and [RFC 7622](https://tools.ietf.org/html/rfc7622).

##### Proven
The first Jabber/XMPP technologies were developed by Jeremie Miller in 1998 and are now quite stable; hundreds of developers are working on these technologies, there are tens of thousands of XMPP servers running on the Internet today, and millions of people use XMPP for instant messaging through public services such as Google Talk and XMPP deployments at organizations worldwide.

##### Decentralised
The architecture of the XMPP network is similar to email; as a result, anyone can run their own XMPP server, enabling individuals and organizations to take control of their communications experience.

##### Secure
Any XMPP server may be isolated from the public network (e.g., on a company intranet) and robust security using SASL and TLS has been built into the core XMPP specifications. In addition, the XMPP developer community is actively working on end-to-end encryption to raise the security bar even further.

##### Extensible
Using the power of XML, anyone can build custom functionality on top of the core protocols; to maintain interoperability, common extensions are published in the XEP series, but such publication is not required and organizations can maintain their own private extensions if so desired.

##### Flexible
XMPP applications beyond IM include network management, content syndication, collaboration tools, file sharing, gaming, remote systems monitoring, web services, lightweight middleware, cloud computing, and much more.

##### Diverse
A wide range of companies and open-source projects use XMPP to build and deploy real-time applications and services; you will never get “locked in” when you use XMPP technologies.

{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://xmpp.org/" "XMPP Home">}}
    {{<listlink "https://xmpp.org/getting-started/" "Getting Started">}}
    {{<listlink "http://www.xmpp-iot.org/" "XMPP IoT Site">}}
    {{<listlink "https://xmpp.org/software/libraries.html" "XMPP Libraries">}}
    {{<listlink "https://xmpp.org/software/clients.html" "Clients">}}
    {{<listlink "https://xmpp.org/software/servers.html" "Servers">}}
    {{<listlink "https://oriolrius.cat/blog/wp-content/uploads/2009/10/Oreilly.XMPP.The.Definitive.Guide.May.2009.pdf" "XMPP: The Definitive Guide">}}
{{< /listcard >}}
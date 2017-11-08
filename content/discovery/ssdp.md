---
title: "SSDP"
full: "Simple Service Discovery Protocol"
type: "article"
description: "The Simple Service Discovery Protocol (SSDP) is a network protocol based on the Internet Protocol Suite for advertisement and discovery of network services and presence information. It accomplishes this without assistance of server-based configuration mechanisms, such as the Dynamic Host Configuration Protocol (DHCP) or the Domain Name System (DNS), and without special static configuration of a network host."
weight: 0
tags: ["protocol","UDP","upnp"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="Wikipedia" %}}
The Simple Service Discovery Protocol (SSDP) provides a mechanism where by network clients, with little or no static configuration, can discover network services. SSDP accomplishes this by providing for multicast discovery support as well as server based notification and discovery routing.

SSDP is a text-based protocol based on HTTPU. It uses the User Datagram Protocol (UDP) as the underlying transport protocol. Services are announced by the hosting system with multicast addressing to a specifically designated IP multicast address at UDP port number 1900. In IPv4, the multicast address is 239.255.255.250 and SSDP over IPv6 uses the address set ff0X::c for all scope ranges indicated by X. [Read more](https://en.wikipedia.org/wiki/Simple_Service_Discovery_Protocol)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://tools.ietf.org/html/draft-cai-ssdp-v1-03" "IETF Draft v3">}}
    {{<listlink "https://openconnectivity.org/developer/specifications/upnp-resources/upnp" "OCF UPnP Spec">}}
{{< /listcard >}}
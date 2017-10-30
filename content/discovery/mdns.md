---
title: "mDNS"
full: "multicast Domain Name System"
type: "article"
description: "mDNS resolves host names to IP addresses within small networks that do not include a local name server. It is a zero-configuration service, using essentially the same programming interfaces, packet formats and operating semantics as the unicast Domain Name System (DNS)."
weight: 0
tags: ["protocol", "zeroconf", "DNS", "IETF"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Zeroconf
It is a set of technologies that automatically creates a usable computer network based on TCP/IP when computers or network peripherals are interconnected. It does not require manual operator intervention or special configuration servers for Dynamic Host Configuration Protocol (DHCP) and Domain Name System (DNS).
{{% /card %}}

{{% card size="4" %}}
### Bonjour [...](https://en.wikipedia.org/wiki/Bonjour_(software))
Bonjour is a networking technology developed by Apple that makes it easy to set up and use devices and services on a network. Bonjour locates devices such as printers, other computers, and the services that those devices offer on a local network using multicast Domain Name System (mDNS) service records.
{{% /card %}}

{{% card size="8" small="lora-alliance.org" %}}
##### Overview
When an mDNS client needs to resolve a host name, it sends an IP multicast query message that asks the host having that name to identify itself. That target machine then multicasts a message that includes its IP address. All machines in that subnet can then use that information to update their mDNS caches.

Any host can relinquish its claim to a domain name by sending a response packet with a time to live (TTL) equal to zero.

By default, mDNS only and exclusively resolves host names ending with the .local top-level domain (TLD). This can cause problems if that domain includes hosts which do not implement mDNS but which can be found via a conventional unicast DNS server. Resolving such conflicts requires network-configuration changes that violate the zero-configuration goal.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.multicastdns.org/" "MulticastDNS.org">}}
    {{<listlink "https://tools.ietf.org/html/rfc6762" "RFC 6762">}}
    {{<listlink "https://www.amazon.com/gp/product/0596101007" "Zeroconf Book (By mDNS Author)">}}
    {{<listlink "http://stuartcheshire.org/SleepProxy/" "Apple's Bonjour Sleep Proxy">}}
{{< /listcard >}}
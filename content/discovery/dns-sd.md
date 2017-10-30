---
title: "DNS-SD"
full: "DNS Service Discovery"
type: "article"
description: "DNS-SD allows clients to discover a named list of service instances, given a service type, and to resolve those services to hostnames using standard DNS queries. The specification is compatible with existing unicast DNS server and client software, but works equally well with Multicast DNS in a zero-configuration environment."
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
Bonjour is a networking technology developed by Apple that makes it easy to set up and use devices and services on a network. Wide-Area Bonjour uses DNS Service Discovery along with DNS Update ([RFC 2136](http://www.ietf.org/rfc/rfc2136.txt)) and TSIG security ([RFC 2845](http://www.ietf.org/rfc/rfc2845.txt)). 
{{% /card %}}

{{% card size="8" small="lora-alliance.org" %}}
##### DNS-based service discovery
 Each service instance is described using a DNS SRV ([RFC 2782](https://tools.ietf.org/html/rfc2782)) and DNS TXT ([RFC 1035](https://tools.ietf.org/html/rfc1035)) record. A client discovers the list of available instances for a given service type by querying the DNS PTR ([RFC 1035](https://tools.ietf.org/html/rfc1035)) record of that service type's name; the server returns zero or more names of the form "<Service>.<Domain>", each corresponding to a SRV/TXT record pair. The SRV record resolves to the domain name providing the instance, while the TXT can contain service-specific configuration parameter. A client can then resolve the A/AAAA record for the domain name and connect to the service. [Read More](https://en.wikipedia.org/wiki/Zero-configuration_networking#Service_discovery)

##### DNS-SD with multicast
Multicast DNS (mDNS) is a protocol that uses packets similar to unicast DNS except sent over a multicast link to resolve hostnames. Each host listens on the mDNS port, 5353, and resolves requests for the DNS record of its .local hostname (e.g. the A, AAAA, CNAME) to its IP address. When an mDNS client needs to resolve a local hostname to an IP address, it sends a DNS request for that name to a well-known multicast address; the computer with the corresponding A/AAAA record replies with its IP address. The mDNS multicast address is 224.0.0.251 for IPv4 and ff02::fb for IPv6 link-local addressing.

DNS service discovery (DNS-SD) requests can also be sent over a multicast link, and it can be combined with mDNS to yield zero-configuration DNS-SD. It still uses DNS PTR, SRV, TXT records to advertise instances of service types, domain names for those instances, and optional configuration parameters for connecting to those instances. But SRV records can now resolve to multicastable .local domain names, which mDNS can resolve to local IP addresses.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.dns-sd.org/" "DNS-SD.org">}}
    {{<listlink "https://developer.apple.com/library/content/documentation/Networking/Conceptual/dns_discovery_api/Introduction.html" "Apple's DNS-SD API">}}
    {{<listlink "https://www.amazon.com/gp/product/0596101007" "Zeroconf Book (By DNS-SD's Author)">}}
    {{<listlink "http://stuartcheshire.org/SleepProxy/" "Apple's Bonjour Sleep Proxy">}}
{{< /listcard >}}
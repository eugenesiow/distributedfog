---
title: "IPsec"
full: "Internet Protocol Security"
type: "article"
description: "IPsec is a network protocol suite that authenticates and encrypts the packets of data sent over a network. IPsec includes protocols for establishing mutual authentication between agents at the beginning of the session and negotiation of cryptographic keys to use during the session."
tags: ["protocol", "specifications"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Specifications
[RFC 4301](https://tools.ietf.org/html/rfc4301) defines a Security Architecture for the Internet Protocol, while [RFC 4303](https://tools.ietf.org/html/rfc4303) defines the Encapsulating Security Payload (ESP) protocol and [RFC 4309](https://tools.ietf.org/html/rfc4309) describes the use of Advanced Encryption Standard (AES) in Counter with CBC-MAC (CCM) Mode as an IPsec Encapsulating Security Payload (ESP) mechanism.
{{% /card %}}

{{% card size="4" %}}
### IPsec and VPNs [...](https://www.lifewire.com/vpns-ipsec-vs-ssl-2486720)
A VPN creates a virtual "tunnel" connecting the two endpoints. The traffic within the VPN tunnel is encrypted so that other users of the public Internet can not readily view intercepted communications. Traditional VPN’s rely on IPsec to secure all data between two endpoints without an association to any specific application. 
{{% /card %}}

{{% card size="8" small="Wikipedia" %}}
 IPsec can protect data flows between a pair of hosts (host-to-host), between a pair of security gateways (network-to-network), or between a security gateway and a host (network-to-host). IPsec uses cryptographic security services to protect communications over Internet Protocol (IP) networks. IPsec supports network-level peer authentication, data-origin authentication, data integrity, data confidentiality (encryption), and replay protection.

IPsec is an end-to-end security scheme operating in the Internet Layer of the Internet Protocol Suite, while some other Internet security systems in widespread use, such as Transport Layer Security (TLS) and Secure Shell (SSH), operate in the upper layers at the Transport Layer (TLS) and the Application layer (SSH). IPsec can automatically secure applications at the IP layer.

##### Security Architecture 
The IPsec suite is an open standard. IPsec uses the following protocols to perform various functions:

- [Authentication Headers (AH)](http://www.tcpipguide.com/free/t_IPSecAuthenticationHeaderAH.htm) provides connectionless data integrity and data origin authentication for IP datagrams and provides protection against replay attacks.
- [Encapsulating Security Payloads (ESP)](https://tools.ietf.org/html/rfc4303) provides confidentiality, data-origin authentication, connectionless integrity, an anti-replay service (a form of partial sequence integrity), and limited traffic-flow confidentiality.
- [Security Associations (SA)](http://www.ciscopress.com/articles/article.asp?p=25443) provides the bundle of algorithms and data that provide the parameters necessary for AH and/or ESP operations. The Internet Security Association and Key Management Protocol (ISAKMP) provides a framework for authentication and key exchange, with actual authenticated keying material provided either by manual configuration with pre-shared keys, Internet Key Exchange (IKE and IKEv2), Kerberized Internet Negotiation of Keys (KINK), or IPSECKEY DNS records.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://en.wikipedia.org/wiki/IPsec" "IPsec on Wikipedia">}}
    {{<listlink "http://www.tcpipguide.com/free/t_IPSecurityIPSecProtocols.htm" "TCP/IP Guide to IPsec">}}
    {{<listlink "http://www.unixwiz.net/techtips/iguide-ipsec.html" "Illustrated IPsec guide">}}
{{< /listcard >}}
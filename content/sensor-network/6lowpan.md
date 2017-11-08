---
title: "6LoWPAN"
full: "IPv6 over Low-Power Wireless Personal Area Networks"
type: "article"
description: "The 6LoWPAN concept originated from the idea that 'the Internet Protocol could and should be applied even to the smallest devices,' and that low-power devices with limited processing capabilities should be able to participate in the Internet of Things. The 6LoWPAN group has defined encapsulation and header compression mechanisms that allow IPv6 packets to be sent and received over IEEE 802.15.4 (LR-WPAN) based networks."
weight: 0
tags: ["protocol", "wireless"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="threadgroup.org" %}}
### Thread
[Thread](http://threadgroup.org/What-is-Thread/Overview) is a standard suggested by Nest Labs based on IEEE 802.15.4 and 6LoWPAN to connect and control products in the home.

- Securely and reliably connect products around the home
- Provides open IPv6 device-to-device and device-to-cloud connections
- Provides security at the network layer
- Devices can route messages with no single point of failure with a robust mesh network
- Install using a smartphone, tablet, or computer (simple setup)
- Based on the power-efficient IEEE 802.15.4 MAC/PHY
{{% /card %}}


{{% card size="8" small="RFC 4919" %}}
IPv4 and IPv6 are the work horses for data delivery for local-area networks, metropolitan area networks, and wide-area networks such as the Internet. Likewise, IEEE 802.15.4 low-power personal area network devices provide sensing communication-ability in the wireless domain. The inherent natures of the two networks though, are different.

##### Problems 6LoWPAN tries to solve are [...](https://www.rfc-editor.org/rfc/rfc4919.txt)
- IP Connectivity
- Supporting Topologies like mesh and star
- Limited Packet Size
- Limited Configuration and Management
- Service Discovery
- Security

##### Goals [...](https://www.rfc-editor.org/rfc/rfc4919.txt)
- Fragmentation and Reassembly layer
- Header Compression
- Address Autoconfiguration
- Mesh Routing Protocol
- Network Management
- Implementation Considerations
- Application and higher layer Considerations
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.rfc-editor.org/rfc/rfc4944.txt" "RFC 4944 Packets Spec">}}
    {{<listlink "https://www.rfc-editor.org/rfc/rfc6606.txt" "RFC 6606 Routing">}}
    {{<listlink "https://tools.ietf.org/html/draft-daniel-6lowpan-interoperability-01" "Interoperability">}}
    {{<listlink "https://tools.ietf.org/html/rfc6282" "RFC 6282 Header Compression">}}
    {{<listlink "https://tools.ietf.org/html/rfc6775" "RFC 6775 Neighbour Discovery">}}
{{< /listcard >}}
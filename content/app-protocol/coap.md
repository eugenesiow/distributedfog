---
title: "CoAP"
full: "Constrained Application Protocol"
type: "article"
description: "CoAP is a specialised web transfer protocol for use with constrained nodes and constrained (e.g., low-power, lossy) networks."
tags: ["protocol"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="RFC 7252" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[HTTP/2](https://webofthings.org/2015/10/25/http2-for-internet-of-things-1/), [CoAP on device HTTP/2 everywhere else](http://timkellogg.me/blog/2015/02/20/can-http2-replace-mqtt), [Security](http://ieeexplore.ieee.org/document/7460363/), [Californium Cloud Services](http://ieeexplore.ieee.org/abstract/document/7030106/), [MQTT vs CoAP](https://www.researchgate.net/profile/Hwee_Xian_Tan/publication/267636202_Performance_evaluation_of_MQTT_and_CoAP_via_a_common_middleware/links/5636d46d08ae75884114e431/Performance-evaluation-of-MQTT-and-CoAP-via-a-common-middleware.pdf), [TinyOS Performance](http://ieeexplore.ieee.org/abstract/document/6208761/), Transport: [Logistics](http://www.academia.edu/download/41232455/Implementation_of_CoAP_and_its_Applicati20160114-28513-evheod.pdf20160115-19908-ve6aow.pdf)
{{% /card %}}

{{% card size="4" %}}
__CoAP__ is network-oriented protocol with similar features to __HTTP__ but also allows for low overhead, multicast, etc. CoAP operates over UDP (simpler) instead of TCP compensating for unreliability with a retransmission mechanism.
{{% /card %}}

{{% card size="8" small="coap.technology" %}}
The Internet of Things will need billions of nodes, many of which will need to be inexpensive. [CoAP](http://coap.technology/) has been designed to work on microcontrollers with as low as 10 KiB of RAM and 100 KiB of code space ([RFC 7228](https://tools.ietf.org/html/rfc7228)).

CoAP was developed as an Internet Standards Document, [RFC 7252](https://tools.ietf.org/html/rfc7252). The protocol has been designed to last for decades. Difficult issues such as congestion control have not been swept under the rug, but have been addressed using the state of the art.

##### REST model for small devices
Like HTTP, CoAP is based on the wildly successful REST model: Servers make resources available under a URL, and clients access these resources using methods such as GET, PUT, POST, and DELETE.

##### Efficient
CoAP is designed to use minimal resources, both on the device and on the network. Instead of a complex transport stack, it gets by with UDP on IP. A 4-byte fixed header and a compact encoding of options enables small messages that cause no or little fragmentation on the link layer. Many servers can operate in a completely stateless fashion.

##### Secure
The Internet of Things cannot spread as long as it can be exploited by hackers willy-nilly. CoAP does not just pay lip service to security, it actually provides strong security. CoAP's default choice of DTLS parameters is equivalent to 3072-bit RSA keys, yet still runs fine on the smallest nodes.

##### Supports various data serialisation formats
Like HTTP, CoAP can carry different types of payloads, and can identify which payload type is being used. CoAP integrates with XML, JSON, [CBOR](http://cbor.io/), or any data format of your choice.

##### Integrated Resource Discovery
The CoAP resource directory provides a way to discover the properties of the nodes on your network.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://coap.technology/" "CoAP Home">}}
    {{<listlink "https://github.com/markushx/coap-cheatsheet/" "Cheatsheet">}}
    {{<listlink "https://www.youtube.com/watch?v=4bSr5x5gKvA" "Tutorial Video">}}
    {{<listlink "http://www.openmobilealliance.org/wp/" "Lightweight M2M">}}
    {{<listlink "https://tools.ietf.org/html/rfc7252" "RFC 7252 Specification">}}
    {{<listlink "https://github.com/ibm-security-innovation/crosscoap" "CoAP-to-HTTP Proxy">}}
    {{<listlink "http://people.inf.ethz.ch/mkovatsc/erbium.php" "Contiki: Erbium REST Engine">}}
    {{<listlink "http://www.eclipse.org/californium/" "Java: Californium">}}
    {{<listlink "https://github.com/okleine/nCoAP" "Java: nCoAP">}}
    {{<listlink "https://libcoap.net/" "C: libcoap">}}
    {{<listlink "https://github.com/dustin/go-coap" "Go: Go-CoAP ">}}
    {{<listlink "https://github.com/mcollina/node-coap" "node.js: node-coap">}}
    {{<listlink "https://github.com/mwasilak/txThings" "Python: txThings">}}
    {{<listlink "https://github.com/nning/coap" "Ruby">}}
    {{<listlink "https://github.com/Covertness/coap-rs" "Rust">}}
    {{<listlink "https://github.com/stuffrabbit/iCoAP" "iOS">}}
{{< /listcard >}}
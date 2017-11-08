---
title: "DASH7"
type: "article"
description: "DASH7 Alliance Protocol (D7A) is an open source Wireless Sensor and Actuator Network protocol, which operates in the 433 MHz, 868 MHz and 915 MHz unlicensed ISM band/SRD band. DASH7 provides multi-year battery life, range of up to 2 km, low latency for connecting with moving things, a very small open source protocol stack, AES 128-bit shared key encryption support, and data transfer of up to 167 kbit/s."
weight: 0
tags: ["protocol", "wireless", "open source"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="dash7-alliance.org" %}}
### Why DASH7?
- Open Standard of Ultra Low Power Mid-Range Sensor and Actuator Communication, Open Source Stacks available
- Ultra Low Power, Low energy per bit transmitted / received, Narrow band low silicon complexity, Low infrastructure deployment cost, Multi-year battery performance
- BLAST (Bursty, Light, Asynchronous, Stealth, Transitional)
- Seamless Indoor and Outdoor use, even in presence of concrete, metal and water
- Optimal RF performances, Low signal attenuation
- Context Aware Sensor and Actuator Data Propagation System, Event based data propagation based on sensor value changes, configurable over the air
{{% /card %}}


{{% card size="8" small="Wikipedia and dash7-alliance.org" %}}
##### BLAST networking technology [...](https://en.wikipedia.org/wiki/DASH7)
Networks based on DASH7 differ from typical wire-line and wireless networks utilizing a "session". DASH7 networks serves applications in which low power usage is essential, and data transmission is typically much slower and/or sporadic, like basic telemetry. Thus instead of replicating a wire-line "session", DASH7 was designed with the concept of B.L.A.S.T.:

- Bursty: Data transfer is abrupt and does not include content such as video, audio, or other isochronous forms of data.
- Light: For most applications, packet sizes are limited to 256 bytes. Transmission of multiple, consecutive packets may occur but is generally avoided if possible.
- Asynchronous: DASH7's main method of communication is by command-response, which by design requires no periodic network "hand-shaking" or synchronization between devices.
- Stealth: DASH7 devices does not need periodic beaconing to be able to respond in communication.
- Transitive: A DASH7 system of devices is inherently mobile or transitional. Unlike other wireless technologies DASH7 is upload-centric, not download-centric, thus devices do not need to be managed extensively by fixed infrastructure (i.e. base stations).

##### OSS-7
OSS-7 is an open source implementation of the DASH7 Alliance protocol. The aim of the project is to provide a reference implementation of the protocol stack which allowing fast development and prototyping of DASH7 based products. This implementation focuses on completeness, correctness and being easy to use and understand. Performance and code size are less important aspects. For clarity a clear separation between the ISO layers is maintained in the code. [Read more](http://mosaic-lopow.github.io/dash7-ap-open-source-stack/)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.dash7-alliance.org/" "DASH7 Alliance">}}
    {{<listlink "http://www.dash7-alliance.org/product/d7ap1-1/" "Spec 1.1">}}
    {{<listlink "http://mosaic-lopow.github.io/dash7-ap-open-source-stack/" "Open Source Stack">}}
{{< /listcard >}}
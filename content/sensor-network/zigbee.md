---
title: "Zigbee"
type: "article"
description: "Zigbee is an IEEE 802.15.4-based specification for a suite of high-level communication protocols used to create personal area networks with small, low-power digital radios, such as for home automation, medical device data collection, and other low-power low-bandwidth needs, designed for small scale projects which need wireless connection."
weight: 0
tags: ["protocol", "wireless", "radio", "mesh"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### IEEE 802.15.4
IEEE 802.15.4 is a technical standard which defines the operation of low-rate wireless personal area networks (LR-WPANs). It specifies the physical layer and media access control. It is the basis for the ZigBee, ISA100.11a,WirelessHART, MiWi, SNAP, and Thread specifications, each of which further extends the standard by developing the upper layers not defined.
{{% /card %}}

{{% card size="4" %}}
### Spec Compare
|    | BT           | BT-LE      | Zigbee     |
|---        |---            |---        |---        |
| Range     | 30m           | 50m       | <300m     |
| Rate      | <3Mbps       | 200Kb/s   | 250Kb/s     |
| Latency   | 6s            | 3ms       | 30ms        |
| Battery   | Days          | Days      | Years       |
| Complexity| Cplx          | Cplx      | Simple      |
| Nodes     | 7             | 7         | 64k         |
{{% /card %}}

{{% card size="8" small="Wikipedia" %}}
Zigbee is a low-cost, low-power, wireless mesh network standard targeted at the wide development of long battery life devices in wireless control and monitoring applications. Zigbee devices have low latency, which further reduces average current. Zigbee chips are typically integrated with radios and with microcontrollers that have between 60-256 KB of flash memory. Zigbee operates in the industrial, scientific and medical (ISM) radio bands: 2.4 GHz in most jurisdictions worldwide; though some devices also use 784 MHz in China, 868 MHz in Europe and 915 MHz in the USA and Australia, however even those regions and countries still use 2.4 GHz for most commercial Zigbee devices for home use. Data rates vary from 20 kbit/s (868 MHz band) to 250 kbit/s (2.4 GHz band).

The Zigbee network layer natively supports both star and tree networks, and generic mesh networking. Every network must have one coordinator device, tasked with its creation, the control of its parameters and basic maintenance. Within star networks, the coordinator must be the central node. Both trees and meshes allow the use of Zigbee routers to extend communication at the network level.

Zigbee builds on the physical layer and media access control defined in IEEE standard 802.15.4 for low-rate WPANs. The specification includes four additional key components: network layer, application layer, Zigbee Device Objects (ZDOs) and manufacturer-defined application objects which allow for customization and favor total integration. ZDOs are responsible for some tasks, including keeping track of device roles, managing requests to join a network, as well as device discovery and security.

Zigbee is one of the global standards of communication protocol formulated by the significant task force under the IEEE 802.15 working group. The fourth in the series, WPAN Low Rate/Zigbee is the newest and provides specifications for devices that have low data rates, consume very low power and are thus characterized by long battery life. Other standards like Bluetooth and IrDA address high data rate applications such as voice, video and LAN communications.

Zigbee provides the ability to run for years on inexpensive batteries for a host of monitoring and control applications. The Zigbee network layer ensures that networks remain operable in the conditions of a constantly changing quality between communication nodes. The Zigbee advantage is the Zigbee protocol which is designed to communicate data through hostile RF environments that are common in commercial and industrial application. Its protocol features include support for multiple network topologies such as; point to point and mesh network, collision avoidance and retries, and low latency. Another defining feature of Zigbee is facilities for carrying out secure communications, protecting establishment and transport of cryptographic keys, cyphering frames, and controlling device. It builds on the basic security framework defined in IEEE 802.15.4.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.zigbee.org/what-is-zigbee/" "Zigbee Alliance">}}
    {{<listlink "http://www.zigbee.org/zigbee-products-2/" "Certified Products">}}
    {{<listlink "https://www.tomsguide.com/us/smart-home-wireless-network-primer,news-21085.html" "ZigBee, Z-Wave, Thread and WeMo">}}
{{< /listcard >}}
---
title: "Insteon"
type: "article"
description: "Insteon is a home automation technology that enables light switches, lights, thermostats, leak sensors, remote controls, motion sensors, and other electrically powered devices to interoperate through power lines, radio frequency (RF) communications, or both. It employs a dual-mesh networking topology in which all devices are peers and each device independently transmits, receives, and repeats messages."
weight: 0
tags: ["protocol", "wireless", "smart home"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Insteon Hub
Insteon Hub is a simple and straightforward device that connects you to your home from any smartphone or tablet, anywhere in the world. Control Insteon light bulbs, wall switches, outlets, and thermostats at home or remotely and receive instant email or push notification alerts from motion, door and window, water leak, and smoke sensors while you’re away.
{{% /card %}}

{{% card size="4" %}}
### Insteon HomeKit Hub
[HomeKit](https://developer.apple.com/homekit/) devices use Bluetooth and Wi-Fi to communicate, but Insteon’s family of home control devices (lights, plugs, switches, sensors, cameras, locks, the works) use a different dual-band communication technology that combines both wireless and powerline networking. The Insteon Hub acts as a bridge between Insteon’s mesh network and your regular Wi-Fi network, so you can reach your Insteon devices from outside of the house, and to bridge your Insteon system with HomeKit.
{{% /card %}}


{{% card size="8" small="Insteon Whitepaper" %}}
##### Protocol Specifications
INSTEON messages are fixed in length and synchronized to the AC powerline zero crossings. They do not contain routing information beyond a source and destination address. INSTEON is reliable and affordable because it is optimized for command and control, not high-speed data transport. INSTEON allows infrastructure devices like light switches and sensors to be networked together in large numbers, at low cost. INSTEON stands on its own, but can also bridge to other networks, such as WiFi LANs, the Internet, telephony, and entertainment distribution systems. Such bridging allows INSTEON to be part of very sophisticated integrated home control environments.

<a href="http://cache.insteon.com/pdf/insteondetails.pdf" target="_blank"><img src="/img/articles/insteon.png" title="Insteon Specifications" style="width: 100%;"></a>

{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.insteon.com/" "Insteon (Company)">}}
    {{<listlink "http://www.insteon.com/insteon-hub" "Hub">}}
    {{<listlink "http://cache.insteon.com/pdf/insteondetails.pdf" "Whitepaper">}}
    {{<listlink "http://cache.insteon.com/pdf/INSTEONCompared.pdf" "Comparison to other protocols">}}
{{< /listcard >}}
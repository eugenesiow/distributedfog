---
title: "UPnP"
full: "Universal Plug and Play "
type: "article"
description: "Universal Plug and Play (UPnP) is a set of networking protocols that permits networked devices, such as personal computers, printers, Internet gateways, Wi-Fi access points and mobile devices to seamlessly discover each other's presence on the network and establish functional network services for data sharing, communications, and entertainment."
weight: 0
tags: ["protocol","zeroconf","upnp"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Protocol
UPnP assumes the network must run Internet Protocol (IP) and then leverages HTTP, SOAP and XML on top of IP, in order to provide device/service description, actions, data transfer and eventing. Device search requests and advertisements are supported by running HTTP on top of UDP using multicast (known as HTTPMU). Responses are also sent over UDP, but are sent using unicast (known as HTTPU).
{{% /card %}}

{{% card size="4" %}}
### Features

- [Addressing](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Addressing)
- [Discovery](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Discovery)
- [Description](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Description)
- [Control](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Control)
- [Event Notification](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Event_notification)
- [Presentation](https://en.wikipedia.org/wiki/Universal_Plug_and_Play#Presentation)
{{% /card %}}

{{% card size="8" small="Wikipedia" %}}
The UPnP architecture allows device-to-device networking of consumer electronics, mobile devices, personal computers, and networked home appliances. It is a distributed, open architecture protocol based on established standards such as the Internet Protocol Suite (TCP/IP), HTTP, XML, and SOAP. UPnP control points (CPs) are devices which use UPnP protocols to control UPnP controlled devices (CDs).

The UPnP architecture supports zero configuration networking. A UPnP compatible device from any vendor can dynamically join a network, obtain an IP address, announce its name, advertise or convey its capabilities upon request, and learn about the presence and capabilities of other devices. Dynamic Host Configuration Protocol (DHCP) and Domain Name System (DNS) servers are optional and are only used if they are available on the network. Devices can disconnect from the network automatically without leaving state information. [Read more](https://en.wikipedia.org/wiki/Universal_Plug_and_Play)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://openconnectivity.org/developer/specifications/upnp-resources/upnp" "OCF UPnP Spec">}}
    {{<listlink "https://www.iso.org/standard/57494.html" "ISO/IEC 29341">}}
    {{<listlink "https://openconnectivity.org/developer/specifications/upnp-resources/upnp/iot-management-and-control1" "IoT Management and Control">}}
{{< /listcard >}}
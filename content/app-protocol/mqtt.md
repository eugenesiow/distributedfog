---
title: "MQTT"
full: "Message Queue Telemetry Transport"
type: "article"
description: "MQTT is a publish-subscribe-based lightweight messaging protocol for use on top of TCP/IP. It is designed for connections where a small code footprint is required or the network bandwidth is limited."
tags: ["protocol", "IBM"]
weight: 10
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[CoAP vs MQTT](https://www.researchgate.net/profile/Hwee_Xian_Tan/publication/267636202_Performance_evaluation_of_MQTT_and_CoAP_via_a_common_middleware/links/5636d46d08ae75884114e431/Performance-evaluation-of-MQTT-and-CoAP-via-a-common-middleware.pdf), [MQTT and REST](http://ieeexplore.ieee.org/abstract/document/6362813/), [Push Notifications](https://www.researchgate.net/profile/Yong_Wang29/publication/266650239_Design_and_Implementation_of_Push_Notification_System_Based_on_the_MQTT_Protocol/links/56ae0c0408ae19a38515f575/Design-and-Implementation-of-Push-Notification-System-Based-on-the-MQTT-Protocol.pdf), [Secure MQTT](http://ieeexplore.ieee.org/abstract/document/7280018/)
{{% /card %}}

{{% card size="4" %}}
[MQTT-SN](http://mqtt.org/MQTT-S_spec_v1.2.pdf) is a variation of the main protocol aimed at embedded devices on non-TCP/IP networks, such as ZigBee. As it does not require the TCP/IP stack, it can be used over a serial link where overhead is really small or over UDP.
{{% /card %}}

{{% card size="8" small="mqtt.org" %}}
##### What is MQTT?
[MQTT](http://mqtt.org/) stands for MQ Telemetry Transport. It is a publish/subscribe, extremely simple and lightweight messaging protocol, designed for constrained devices and low-bandwidth, high-latency or unreliable networks. The design principles are to minimise network bandwidth and device resource requirements whilst also attempting to ensure reliability and some degree of assurance of delivery. These principles also turn out to make the protocol ideal of the emerging “machine-to-machine” (M2M) or “Internet of Things” world of connected devices, and for mobile applications where bandwidth and battery power are at a premium.

##### Is MQTT a standard?
MQTT Version 3.1.1 is an [OASIS Standard](https://www.oasis-open.org/news/announcements/mqtt-version-3-1-1-becomes-an-oasis-standard).

##### Are there standard ports for MQTT to use?
Yes. TCP/IP port 1883 is reserved with IANA for use with MQTT. TCP/IP port 8883 is also registered, for using MQTT over SSL.

##### Does MQTT support security?

You can pass a user name and password with an MQTT packet in V3.1 of the protocol. Encryption across the network can be handled with SSL, independently of the MQTT protocol itself (it is worth noting that SSL is not the lightest of protocols, and does add significant network overhead). Additional security can be added by an application encrypting data that it sends and receives, but this is not something built-in to the protocol, in order to keep it simple and lightweight.

##### Who uses MQTT?
Here are lists of notable [Eclipse Paho Users](https://www.eclipse.org/paho/whoisusing/) and [MQTT project users](http://mqtt.org/projects).

{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://mqtt.org/documentation" "MQTT Documentation">}}
    {{<listlink "https://github.com/mqtt/mqtt.github.io/wiki/software" "Software">}}
    {{<listlink "https://github.com/mqtt/mqtt.github.io/wiki/APIs-and-examples" "APIs and Examples">}}
    {{<listlink "https://www.eclipse.org/paho/" "Eclipse Paho">}}
    {{<listlink "https://mosquitto.org/" "Mosquitto Broker">}}
    {{<listlink "https://www.hivemq.com/" "HiveMQ Enterprise Broker">}}
    {{<listlink "https://www.baldengineer.com/mqtt-tutorial.html" "Tutorial for RPi and Arduino">}}
    
    
    
{{< /listcard >}}
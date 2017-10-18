---
title: "Beacon"
type: "article"
description: "Beacons are small devices that enable relatively accurate location within a narrow range (like indoors). Beacons periodically transmit small amounts of data within a range of approximately 70 meters, and are often used for indoor location technology."
tags: ["location","mobile","navigation"]
date: 2017-10-11T16:24:18+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[Smart Wearables Indoor Positioning](http://ieeexplore.ieee.org/abstract/document/7888342/), [Indoor Positioning with Beacons](http://ieeexplore.ieee.org/abstract/document/7562730/)
Health: [Navigation for Wheelchair Users](http://ieeexplore.ieee.org/abstract/document/7897199/), [GuideBeacon](http://ieeexplore.ieee.org/abstract/document/7917858/)
{{% /card %}}

{{% card size="4" %}}
[iBeacon](https://developer.apple.com/ibeacon/) by Apple and [Eddystone](https://github.com/google/eddystone) (formerly UriBeacon) by Google are 2 popular beacon technologies. iBeacon transmits only a UUID (a unique identifier) while Eddystone allows the transmission of URL, UUID and telemetry information, hence, removing the need for a specialised mobile app.
{{% /card %}}

{{% card size="8" small="Wikipedia, Apple, Google and others" %}}
##### iBeacon
[iBeacon](https://developer.apple.com/ibeacon/) is a technology enabling location awareness possibilities for apps from welcoming people as they arrive at a sporting event to providing information about a nearby museum exhibit. Leveraging Bluetooth Low Energy (BLE), a device with iBeacon technology can be used to establish a region around an object. This allows an iOS device to determine when it has entered or left the region, along with an estimation of proximity to a beacon.

iBeacon is based on Bluetooth low energy proximity sensing by transmitting a universally unique identifier (UUID) picked up by a compatible app or operating system. The identifier and several bytes sent with it can be used to determine the device's physical location, track customers, or trigger a location-based action on the device such as a check-in on social media or a push notification.

iBeacon can also be used with an application as an indoor positioning system, which helps smartphones determine their approximate location or context. With the help of an iBeacon, a smartphone's software can approximately find its relative location to an iBeacon in a store. Brick and mortar retail stores use the beacons for mobile commerce, offering customers special deals through mobile marketing,[9] and can enable mobile payments through point of sale systems.

##### Eddystone
[Eddystone](https://github.com/google/eddystone) is a protocol specification that defines a Bluetooth low energy (BLE) message format for proximity beacon messages. It describes several different frame types that may be used individually or in combinations to create beacons that can be used for a variety of applications.

Announced in April 2016, Eddystone-EID (Ephemeral ID) is a new frame type that defines a cryptographically secure method of configuring a beacon to broadcast information that only authorized people may decrypt. It includes support for a secure transmission of the TLM (Telemetry) information.

##### Other Beacons

[GeoBeacon](https://github.com/Tecno-World/GeoBeacon) is an open source beacon protocol that was designed for usage in GeoCaching applications due the very compact type of data storage. [AltBeacon](https://github.com/AltBeacon/spec) is a protocol specification that defines a message format for proximity beacon advertisements. 
{{% /card %}}

{{< listcard size="4" title="Products">}}
    {{<listlink "https://www.webopedia.com/TERM/B/beacon.html" "Webopedia Entry">}}
    {{<listlink "https://developer.apple.com/ibeacon/Getting-Started-with-iBeacon.pdf" "iBeacon: Getting Started">}}
    {{<listlink "https://github.com/google/eddystone" "Eddystone: Github">}}
    {{<listlink "http://altbeacon.org/" "AltBeacon: Home">}}
    {{<listlink "https://github.com/AltBeacon/spec" "AltBeacon: Specification">}}
    {{<listlink "https://github.com/Tecno-World/GeoBeacon" "GeoBeacon: Specification">}}
{{< /listcard >}}
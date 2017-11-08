---
title: "Bluetooth"
type: "article"
description: "Bluetooth is a wireless technology standard for exchanging data over short distances (using short-wavelength UHF radio waves in the industrial, scientific and medical (ISM) radio bands from 2.4 to 2.485 GHz) from fixed and mobile devices, and building personal area networks (PANs). Bluetooth Low Energy or Smart is intended to provide considerably reduced power consumption and cost while maintaining a similar communication range."
weight: 10
tags: ["protocol", "wireless", "mesh"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Feature Compare [...](http://www.argenox.com/bluetooth-low-energy-ble-v4-0-development/library/a-guide-to-selecting-a-bluetooth-chipset/)
| Feature   | BT-LE           | BT      |
|---        |---            |---        |
| Audio/Headset     | No           | Yes       |
| Data      | Yes      | Yes   |
| A/V Control   | Non-Native            | Native      |
| Throughput   | Low          | Medium      |
| Authentication| No          | For Non-Audio Only      |
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

{{% card size="8" small="bluetooth.com" %}}
Bluetooth is a low-power wireless connectivity technology used to stream audio, transfer data and broadcast information between devices. There are two flavors of Bluetooth technology, Basic Rate/Enhanced Data Rate (BR/EDR) and Low Energy (LE).

##### Basic Rate/Enhanced Data Rate (BR/EDR)

Bluetooth BR/EDR enables continuous wireless connections and uses a point-to-point (P2P) network topology to establish one-to-one (1:1) device communications. Bluetooth BR/EDR audio streaming is ideal for wireless speakers, headsets and hands-free in-car systems.

##### Low Energy (LE)

Bluetooth LE enables short-burst wireless connections and uses multiple network topologies, including point-to-point, broadcast and mesh.

__Point-to-point (P2P)__ is a network topology used to create one-to-one (1:1) device communications. Bluetooth LE P2P topology is ideal for data transfers and well suited for connected device products, such as fitness trackers and health monitors.

__Broadcast__ is a network topology that establishes one-to-many (1:m) device communications. Bluetooth LE broadcast topology optimizes localized information sharing, making it ideal for beacon solutions, such as point-of-interest (PoI) information and item and way-finding services.

__Mesh__ is a network topology for many-to-many (m:m) device communications. Bluetooth LE mesh topology creates large-scale device networks tailor-made for building automation, sensor network, asset tracking and any solution where multiple devices need to reliably and securely communicate with one another.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.bluetooth.com/" "Bluetooth Technology">}}
    {{<listlink "https://www.bluetooth.com/develop-with-bluetooth/developer-resources-tools" "Developer Tools">}}
    {{<listlink "http://www.argenox.com/bluetooth-low-energy-ble-v4-0-development/library/a-guide-to-selecting-a-bluetooth-chipset/" "Chipsets and Devices">}}
{{< /listcard >}}
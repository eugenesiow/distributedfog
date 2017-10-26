---
title: "LoRaWAN"
full: "Long Range Wide Area Network"
type: "article"
description: "LoRaWAN is a Low Power Wide Area Network (LPWAN) specification intended for wireless battery operated Things in a regional, national or global network. It is designed to allow low-powered devices to communicate with Internet-connected applications over long range wireless connections."
tags: ["protocol", "WAN"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="lora-alliance.org" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### The Things Network
[The Things Network](http://thethingsnetwork.org/) is a first-of-its-kind system that uses low-power, low-bandwidth LoRaWAN technology to cover the city with a wireless signal that allows objects like boats, trash cans and street lights to become tools for developers. Unlike other ‘smart city’ projects, this one is entirely crowdsourced by citizens and was put together in just six weeks.
{{% /card %}}

{{% card size="4" %}}
### Things Connected
[Things Connected](https://www.thingsconnected.net/) is an initiative by Digital Catapult, to support UK businesses using LPWAN technologies. It is a free LoRaWAN network and it is intended for the prototyping of new products and services that can benefit from the unique features of LPWAN. 
{{% /card %}}

{{% card size="8" small="lora-alliance.org" %}}
##### What is LoRa?
LoRa is the physical layer or the wireless modulation utilized to create the long range communication link. Many legacy wireless systems use frequency shifting keying (FSK) modulation as the physical layer because it is a very efficient modulation for achieving low power. LoRa is based on chirp spread spectrum modulation, which maintains the same low power characteristics as FSK modulation but significantly increases the communication range. Chirp spread spectrum has been used in military and space communication for decades due to the long communication distances that can be achieved and robustness to interference, but LoRa is the first low cost implementation for commercial usage. 

The advantage of LoRa® is in the technology’s long range capability. A single gateway or base station can cover entire cities or hundreds of square kilometers. Range highly depends on the environment or obstructions in a given location, but LoRa and LoRaWAN have a link budget greater than any other standardized communication technology. The link budget, typically given in decibels (dB), is the primary factor in determining the range in a given environment. 

##### What is LoRaWAN?
LoRaWAN defines the communication protocol and system architecture for the network while the LoRa physical layer enables the long-range communication link. The protocol and network architecture have the most influence in determining the battery lifetime of a node, the network capacity, the quality of service, the security, and the variety of applications served by the network. [Read More](https://www.lora-alliance.org/what-is-lora)

##### How secure is it?
LoRaWAN has been designed to include a certain amount of security, authentication and encryption. The Network Session key is used to ensure security at network level - from device to the network. The key is 128 bits in length represented by a 32-character hexadecimal string. The Application Session key is used to ensure end-to-end security at application level – from device to the users end application server. The key is 128 bits in length represented by a 32-character hexadecimal string. A developer is of course free to further encrypt the data payload should they have the requirement to do so.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.lora-alliance.org/" "LoRa Alliance">}}
    {{<listlink "https://www.lora-alliance.org/lorawan-for-developers" "LoRa Alliance Developers Page">}}
    {{<listlink "https://www.thethingsnetwork.org/wiki/LoRaWAN/Home" "The Things Network LoRaWAN">}}
{{< /listcard >}}
---
title: "Contiki"
type: "article"
tags: ["rtos"]
description: "An open source operating system for the Internet of Things. Contiki connects tiny low-cost, low-power microcontrollers to the Internet. Contiki is a powerful toolbox for building complex wireless systems."
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="contiki-os.org" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[vs TinyOS](https://www.net.in.tum.de/fileadmin/TUM/NET/NET-2012-08-2/NET-2012-08-2_02.pdf), [IoT-Lab Testbed](https://www.iot-lab.info/operating-systems/), [WSN OS Comparisons](https://www.researchgate.net/publication/241635004_A_comparative_study_on_operating_system_for_Wireless_Sensor_Networks)
{{% /card %}}

{{% card size="4" %}}
Programming on __Contiki__ is done using the __Cooja__ network simulator. To program, control and monitor the remote IoT devices, the back-end C base libraries of RFID chips and sensors can be customised and recompiled to get the desired results.
{{% /card %}}

{{% card size="8" small="Wikipedia and contiki-os.org" %}}
Contiki is an operating system for networked, memory-constrained systems with a focus on low-power wireless Internet of Things devices. Extant uses for Contiki include systems for street lighting, sound monitoring for smart cities, radiation monitoring, and alarms. It is open-source software released under a [BSD](https://choosealicense.com/licenses/bsd-3-clause/) license.

Contiki provides multitasking and a built-in Internet Protocol Suite (TCP/IP stack), yet needs only about 10 kilobytes of random-access memory (RAM) and 30 kilobytes of read-only memory (ROM).  A full system, including a graphical user interface, needs about 30 kilobytes of RAM.

##### Networking
Contiki provides a full IP network stack, with standard IP protocols such as UDP, TCP, and HTTP, in addition to the new low-power standards like 6lowpan, RPL, and CoAP. 

##### Power Awareness
Contiki is designed to operate in extremely low-power systems: systems that may need to run for years on a pair of AA batteries. To assist the development of low-power systems, Contiki provides mechanisms for estimating the system power consumption and for understanding where the power was spent.

##### Hardware Platforms
Contiki runs on a wide range of tiny platforms, ranging from 8051-powered systems-on-a-chip through the MSP430 and the AVR to a variety of ARM devices. 

##### Programming Model: Protothreads
To save memory but provide a nice control flow in the code, Contiki uses a mechanism called protothreads. Protothreads is a mixture of the event-driven and the multi-threaded programming mechanisms. With protothreads, event-handlers can be made to block, waiting for events to occur.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://www.contiki-os.org/index.html" "Contiki Home">}}
    {{<listlink "http://www.ti.com/ww/en/wireless_connectivity/sensortag/" "Texas Instruments SensorTag">}}
    {{<listlink "http://www.ti.com/tool/CC2650DK" "CC2650 Development Kit">}}
    {{<listlink "https://sourceforge.net/projects/contiki/files/Instant%20Contiki/" "Instant Contiki Dev Env">}}
    {{<listlink "http://contiki-os.blogspot.co.uk/" "Official Blog">}}
    {{<listlink "http://www.contiki-os.org/community.html" "Community Support">}}
    {{<listlink "http://anrg.usc.edu/contiki/index.php/Cooja_Simulator" "Cooja Network Simulator">}}
    {{<listlink "http://webbtv.compodium.se/trefpunkt22/007/" "Talk on Contiki by Adam Dunkels">}}
    {{<listlink "http://anrg.usc.edu/contiki/index.php/Contiki_tutorials" "Tutorials">}}
    {{<listlink "http://anrg.usc.edu/contiki/index.php/Interfacing_with_Python" "Python Interfacing">}}
    {{<listlink "https://www.wsnmagazine.com/step-by-step-method-of-writing-contiki-programs/" "Programming Step-by-Step">}}
    {{<listlink "http://www.cs.wayne.edu/~hzhang/courses/6290/Lectures/0-2%20-%20Contiki-tutorial.pdf" "Course Tutorial">}}
    {{<listlink "https://www.youtube.com/watch?v=VFxnktInifw" "Tutorial Video">}}
    {{<listlink "https://www.youtube.com/watch?v=DXGdllpDyVs" "Cooja Tutorial Video">}}
{{< /listcard >}}

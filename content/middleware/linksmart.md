---
title: "LinkSmart"
type: "article"
description: "LinkSmart, formerly Hydra, is an open source IoT platform for developing IoT applications for various domains, such as Smart Cities, Industrie 4.0, Smart Grid and much more. The LinkSmart platform provides building blocks as generic and domain-specific services to efficiently implement applications in the Internet of Things. These include basic services such as device abstraction, data storage, live data management, and advanced ones such as stream mining and online machine learning."
tags: ["software","research"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="linksmart.eu" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="docs.linksmart.eu" %}}

### LinkSmart Architecture

<a href="https://docs.linksmart.eu/display/HOME/What+is+LinkSmart" target="_blank"><img src="/img/articles/linksmart.png" title="LinkSmart Architecture" style="width:100%;"></a>

##### Device Integration & Abstraction
The LinkSmart® Device Integration & Abstraction subset takes care of connecting devices and exposing them through an IP network protocol. This process is the first basic step into an IoT infrastructure. The service responsible for doing this is the DeviceConnector. A DeviceConnector integrates the physical devices into the IP-network infrastructure by abstracting them into OGC SensorThings objects, providing an endpoint to access the devices, propagate any change in the status of devices, and allow secure interaction with devices. The LinkSmart® platform comes with various DeviceConnector implementations for different use cases:

- DGW: IoT Device Gateway - for consumer IoT use cases 
- IGW: IndustrialOPC Gateway - for IIoT or Industry 4.0 use cases
- SP: Sensor Platform - for embedded data management

##### Service Provisioning
In an IoT infrastructure, the number of devices and services can grow quickly and their status' and connectivity can change dynamically. To be able to manage such infrastructure, LinkSmart® platform provides a set of services to manage and keep track of the running devices, services, systems, and sub-systems. In this subset, LinkSmart® uses following solutions:\

- SC: Service Catalogue - for service registration and monitoring 
- RC: Resource Catalogue - for devices registration and monitoring 
- MR: Model Repository - for storing and managing domain and deployment models describing devices and services integrated into a particular application context

##### Data Management & Processing 
IoT applications need to deal with large amounts of data produced by growing amounts of sensors and other devices. Depending on the use case, such data needs to stored, processed, or managed in another way. Sometimes it may be sufficient to store simple time-series data while on other occasions it may be necessary to do stream mining or online machine learning. LinkSmart® provides the following services for data management & processing:

- HDS: Historical Datastore - for storing, querying, and aggregating (time-series) sensor data
- DPA: IoT Data-Processing agent - for stream mining and on-demand data analysis 
- LA: IoT Learning agent - for stream learning and complex analysis processes
- BPA: BPMN Annotator - for annotating sensor data coming from complex business process

##### Networking & Security
For any internet system, some basic infrastructure is needed for secure and reliable communication. In the LinkSmart® Platform, we provide or use some services to intelligently manage the secure network communication in it. 

- BGW: IoT Border Gateway - for managing IoT security policies in Authorization, Authentication, and Accounting
- MQTT Broker: for most of the internal communication in the LinkSmart® Platform, we rely on third party MQTT brokers.

##### Human-Computer Interaction
The LinkSmart platform provides out-of-the-box visualization for rapid prototyping based on Grafana or FreeBoard. Currently, there are two plug-ins for visualizing and manipulating data:

- HDS: for visualizing stored data 
- DPA: for visualizing live data
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://docs.linksmart.eu/" "LinkSmart">}}
    {{<listlink "http://www.hydramiddleware.eu/" "Hydra Project">}}
    {{<listlink "http://www.hydramiddleware.eu/downloads.php?cat_id=2" "List of Papers">}}
{{< /listcard >}}
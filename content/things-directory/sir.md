---
title: "SIR"
full: "Sensor Instance Registry"
type: "article"
description: "The Sensor Instance Registry (SIR) is a web service interface for managing sensor catalogues. It is based on the OGC discussion paper 10-171 and 09-163r2 (SensorML discovery profile) and presents a pragmatic solution that may serve as the basis for further discussion and development. The paper contains extensive descriptions of the service operations (requests and responses) for GET and POST requests."
weight: 0
tags: ["research", "interoperability","search","discovery"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="52north.org" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### SensorML discovery profile ([Paper](https://portal.opengeospatial.org/files/?artifact_id=37944))
This Discussion Paper describes the mapping of sensor metadata encoded following SensorML specification 1.0 ([OGC 07-000](https://portal.opengeospatial.org/files/?artifact_id=21273)) and a SensorML profile for discovery to an ebRIM structure within an OGC Catalogue 2.0.2 ([OGC 07-006r1](https://portal.opengeospatial.org/files/?artifact_id=20555)) implementing the CSW-ebRIM Registry Service – part 1: ebRIM profile of CSW ([OGC 07-110r4](https://portal.opengeospatial.org/files/?artifact_id=31137)).
{{% /card %}}

{{% card size="4" %}}
### OpenGIS Catalogue Services ([Paper](https://portal.opengeospatial.org/files/?artifact_id=20555))
Catalogue services support the ability to publish and search collections of descriptive information (metadata) for data, services, and related information objects. Metadata in catalogues represent resource characteristics that can be queried and presented for evaluation and further processing by both humans and software. Catalogue services are required to support the discovery and binding to registered information resources within an information community. 
{{% /card %}}

{{% card size="8" small="OGC Sensor Instance Registry Discussion Paper" %}}
The specified Sensor Instance Registry is capable of harvesting, managing and transforming sensor metadata. In particular is provides operations for searching sensors, inserting metadata, handling the status of sensors and for linking SIR instances to OGC Catalogs. The SIR interface (currently) specifies 14 operations that can be requested by a client and performed by a SIR server. These operations are: 

- GetCapabilities
- Operations for searching sensors and retrieving sensor metadata: 
    - SearchSensor
    - DescribeSensor
- Operations for inserting, deleting and updating sensor metadata:
    - HarvestService
    - InsertSensorInfo 
    - DeleteSensorInfo
    - UpdateSensorDescription
- Operations for managing sensor status information: 
    - GetSensorStatus
    - SubscribeSensorStatus
    - RenewSensorStatusSubscription
    - CancelSensorStatusSubscription
    - InsertSensorStatus
- Operations for managing the links between SIR instances and OGC Catalogs: 
    - ConnectToCatalog
    - DisconnectFromCatalog

Many of these interface aspects are common with other OWSs and thus specified in the OpenGIS Web Services Common Implementation Standard ([OGC 06-121r3](http://www.opengeospatial.org/standards/common)).
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "http://portal.opengeospatial.org/files/?artifact_id=40609" "Original Paper">}}
    {{<listlink "https://portal.opengeospatial.org/files/?artifact_id=37944" "SensorML discovery profile">}}
    {{<listlink "https://wiki.52north.org/SensorWeb/SensorInstanceRegistry" "Wiki on 52north.org">}}
    {{<listlink "https://wiki.52north.org/SensorWeb/OpenSensorSearch" "OpenSensorSearch">}}
{{< /listcard >}}
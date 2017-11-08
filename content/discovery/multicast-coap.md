---
title: "Multicast CoAP"
type: "article"
description: "Group communication involves a one-to-many relationship between CoAP endpoints. Specifically, a single CoAP client can simultaneously get (or set) resources from multiple CoAP servers using CoAP over IP multicast. CoAP is a web transfer protocol based on Representational State Transfer (REST) for resource constrained devices operating in an IP network."
weight: 0
tags: ["protocol","multicast","CoAP","CoRE"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="RFC 7390" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="RFC 6690" %}}
In M2M applications, for example, home or building automation, there is a need for local clients and servers to find and interact with each other without human intervention. The [CoRE Link Format](https://tools.ietf.org/html/rfc6690) can be used by servers in such environments to enable Resource Discovery of the resources hosted by the server.

Resource Discovery can be performed either unicast or multicast. When a server's IP address is already known, either a priori or resolved via the Domain Name System (DNS), unicast discovery is performed in order to locate the entry point to the resource of interest.  In this specification, this is performed using a GET to "/.well-known/core" on the server, which returns a payload in the CoRE Link Format. A client would then match the appropriate Resource Type, Interface Description, and possible media type for its application.  These attributes may also be included in the query string in order to filter the number of links returned in a response.

Multicast Resource Discovery is useful when a client needs to locate a resource within a limited scope, and that scope supports IP multicast. A GET request to the appropriate multicast address is made for "/.well-known/core". In order to limit the number and size of responses, a query string is recommended with the known attributes. Typically, a resource would be discovered based on its Resource Type and/or Interface Description, along with possible application-specific attributes. [Read more](https://tools.ietf.org/html/rfc6690#section-1.2.1)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://tools.ietf.org/html/rfc7390" "RFC 7390">}}
    {{<listlink "https://tools.ietf.org/html/rfc6690" "RFC 6690 CoRE Link Format">}}
    {{<listlink "https://www.iotivity.org/documentation/linux/programmers-guide/finding-resource" "IoTivity Finding a Resource">}}
{{< /listcard >}}
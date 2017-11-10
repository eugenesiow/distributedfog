---
title: "Websocket"
type: "article"
description: "WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C."
tags: ["protocol", "HTTP"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### µWebSockets ([Code](https://github.com/uNetworking/uWebSockets))
µWS is one of the most lightweight, efficient & scalable WebSocket & HTTP server implementations available. It features an easy-to-use, fully async object-oriented interface and scales to millions of connections using only a fraction of memory compared to the competition.
{{% /card %}}

{{% card size="4" %}}
### SocketCluster ([Site](https://socketcluster.io))
SocketCluster is an open source real-time framework for Node.js. It supports both direct client-server communication and group communication via pub/sub channels. It is designed to easily scale to any number of processes/hosts.
{{% /card %}}

{{% card size="8" small="Wikipedia" %}}
WebSocket is a different TCP protocol from HTTP. Both protocols are located at layer 7 in the OSI model and, as such, depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 80 and 443 as well as to support HTTP proxies and intermediaries" thus making it compatible with the HTTP protocol. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol.

The WebSocket protocol enables interaction between a browser and a web server with lower overheads, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the browser without being solicited by the client, and allowing for messages to be passed back and forth while keeping the connection open. In this way, a two-way (bi-directional) ongoing conversation can take place between a browser and the server. The communications are done over TCP port number 80 (or 443 in the case of TLS-encrypted connections), which is of benefit for those environments which block non-web Internet connections using a firewall. Similar two-way browser-server communications have been achieved in non-standardized ways using stopgap technologies such as Comet. [Read more](https://en.wikipedia.org/wiki/WebSocket)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://tools.ietf.org/html/rfc6455" "RFC 6455 The Websocket Protocol">}}
    {{<listlink "http://www.websocket.org/aboutwebsocket.html" "Websocket.org">}}
    {{<listlink "https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API" "Websockets API">}}
    {{<listlink " https://www.html5rocks.com/en/tutorials/websockets/basics/" "Introducing Websockets">}}
{{< /listcard >}}
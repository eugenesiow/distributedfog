---
title: "HTTP/2"
full: "Hypertext Transfer Protocol 2.0"
type: "article"
description: "HTTP/2 is a major revision of the HTTP network protocol used by the World Wide Web and derived from Google's earlier experimental SPDY protocol."
tags: ["protocol", "HTTP"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[HTTP/1.1 pipelining vs HTTP2 in-the-clear](http://ieeexplore.ieee.org/abstract/document/7745823/), [HTTP/2 multiplexed stream](http://ieeexplore.ieee.org/abstract/document/7748934/), [HTTP/2 in Web Services](https://www.researchgate.net/profile/Nagy_Ramadan/publication/307906792_Impact_of_Implementing_HTTP2_in_Web_Services/links/57d1514208ae6399a38b411c/Impact-of-Implementing-HTTP-2-in-Web-Services.pdf)
{{% /card %}}

{{% card size="4" %}}
__HTTP/2 Server Push__ allows you to send site assets to the user before they’ve even asked for them. It’s an elegant way to achieve the performance benefits of HTTP/1 optimization practices such as inlining, but without the drawbacks that come with that practice. [More](https://www.smashingmagazine.com/2017/04/guide-http2-server-push/)
{{% /card %}}

{{% card size="8" small="http2.github.io" %}}
HTTP/2 is a replacement for how HTTP is expressed “on the wire.” It is not a ground-up rewrite of the protocol; HTTP methods, status codes and semantics are the same, and it should be possible to use the same APIs as HTTP/1.x (possibly with some small additions) to represent the protocol.

The focus of the protocol is on performance; specifically, end-user perceived latency, network and server resource usage. One major goal is to allow the use of a single connection from browsers to a Web site.

The basis of the work was [SPDY](https://www.chromium.org/spdy/spdy-whitepaper), but HTTP/2 has evolved to take the community’s input into account, incorporating several improvements in the process.

##### Goals
- Create a negotiation mechanism that allows clients and servers to elect to use HTTP 1.1, 2.0, or potentially other non-HTTP protocols.
- Maintain high-level compatibility with HTTP 1.1 (for example with methods, status codes, URIs, and most header fields).
- Decrease latency to improve page load speed in web browsers by considering:
    - Data compression of HTTP headers
    - HTTP/2 Server Push
    - Pipelining of requests
    - Fixing the head-of-line blocking problem in HTTP 1.x
    - Multiplexing multiple requests over a single TCP connection
- Support common existing use cases of HTTP, such as desktop web browsers, mobile web browsers, web APIs, web servers at various scales, proxy servers, reverse proxy servers, firewalls, and content delivery networks.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://http2.github.io/" "HTTP/2 Home">}}
    {{<listlink "https://github.com/http2/http2-spec/wiki/Implementations" "Implementations">}}
    {{<listlink "http://httpwg.org/specs/rfc7540.html" "RFC 7540">}}
{{< /listcard >}}
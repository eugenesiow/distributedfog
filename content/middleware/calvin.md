---
title: "Calvin"
type: "article"
description: "Calvin is an application environment that lets things talk to things. It comprises of both a development framework for IoT application developers, and a runtime environment which handles the running application. Calvin is based on the fundamental idea that application development should be simple and fun. There should be no unnecessary impediments between an idea and its implementation, and an app developer should not have to worry about communication protocols or hardware specifics (but will not stop you from doing it if you want to.)"
tags: ["software","research","ericsson"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Github" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="2017 IEEE 37th International Conference on Distributed Computing Systems (ICDCS)" %}}
### Abstract
Calvin is an IoT framework for application development, deployment and execution in heterogeneous environments, that includes clouds, edge resources, and embedded or constrained resources. Inside Calvin, all the distributed resources are viewed as one environment by the application. The framework provides multi-tenancy and simplifies development of IoT applications, which are represented using a dataflow of application components (named actors) and their communication. The idea behind Calvin poses similarity with the serverless architecture and can be seen as Actor as a Service instead of Function as a Service. This makes Calvin very powerful as it does not only scale actors quickly but also provides an easy actor migration capability. In this work, we propose Calvin Constrained, an extension to the Calvin framework to cover resource-constrained devices. Due to limited memory and processing power of embedded devices, the constrained side of the framework can only support a limited subset of the Calvin features. The current implementation of Calvin Constrained supports actors implemented in C as well as Python, where the support for Python actors is enabled by using MicroPython as a statically allocated library, by this we enable the automatic management of state variables and enhance code re-usability. As would be expected, Python-coded actors demand more resources over C-coded ones. We show that the extra resources needed are manageable on current off-the-shelve micro-controller-equipped devices when using the Calvin framework.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://www.ericsson.com/research-blog/open-source-calvin/" "Article">}}
    {{<listlink "https://github.com/EricssonResearch/calvin-base" "Github">}}
    {{<listlink "https://github.com/EricssonResearch/calvin-base/wiki" "Getting Started">}}
{{< /listcard >}}
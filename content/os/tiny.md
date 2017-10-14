---
title: "TinyOS"
type: "article"
tags: ["RTOS"]
description: "TinyOS is an embedded, component-based operating system and platform for low-power wireless devices, such as those used in wireless sensor networks (WSNs), smartdust, ubiquitous computing, personal area networks, building automation, and smart meters."
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Research
[Original Paper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.129.7716&rep=rep1&type=pdf), [Hybrid Network Evaluation](http://ieeexplore.ieee.org/document/4416801/), [Ten-years on Paper](https://sing.stanford.edu/pubs/tinyos-retrospective-osdi2012.pdf)
{{% /card %}}

{{% card size="4" %}}
Programming on __TinyOS__ is done using a C-like language called __nesC__. It is a  component-based, event-driven programming language with components "wired" together to run applications. Phil Levis's book, [TinyOS Programming](http://tinyos.stanford.edu/tinyos-wiki/index.php/Reference,_TEPs,_Papers,_and_User_Notes) is a good guide.
{{% /card %}}

{{% card size="8" small="Wikipedia and tinyos.stanford.edu" %}}
[TinyOS](https://github.com/tinyos/tinyos-main) is an "operating system" designed for low-power wireless embedded systems. Fundamentally, it is a work scheduler and a collection of drivers for microcontrollers and other ICs commonly used in wireless embedded platforms.

TinyOS applications are written in the programming language [nesC](https://github.com/tinyos/nesc), a dialect of the C language optimized for the memory limits of sensor networks. TinyOS programs are built of software components, some of which present hardware abstractions. Components are connected to each other using interfaces. TinyOS provides interfaces and components for common abstractions such as packet communication, routing, sensing, actuation and storage.

TinyOS is fully non-blocking: it has one call stack. Thus, all input/output (I/O) operations that last longer than a few hundred microseconds are asynchronous and have a callback. To enable the native compiler to better optimize across call boundaries, TinyOS uses nesC's features to link these callbacks, called events, statically. While being non-blocking enables TinyOS to maintain high concurrency with one stack, it forces programmers to write complex logic by stitching together many small event handlers. To support larger computations, TinyOS provides tasks, which are similar to a Deferred Procedure Call and interrupt handler bottom halves. A TinyOS component can post a task, which the OS will schedule to run later. Tasks are non-preemptive and run in first in, first out order. This simple concurrency model is typically sufficient for I/O centric applications, but its difficulty with CPU-heavy applications has led to developing a thread library for the OS, named TOSThreads.
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://github.com/tinyos/tinyos-main" "Github Repo">}}
    {{<listlink "https://github.com/tinyos/nesc" "nesC Repo">}}
    {{<listlink "http://tinyos.stanford.edu/tinyos-wiki/index.php/TinyOS_Overview" "TinyOS Wiki">}}
    {{<listlink "http://csl.stanford.edu/~pal/pubs/tos-programming-web.pdf" "Programming Book (Phil Levis)">}}
    {{<listlink "http://homepage.cs.uiowa.edu/~ochipara/classes/wsn/lectures/tinyos-tutorial.pdf" "TinyOS Tutorial">}}
{{< /listcard >}}
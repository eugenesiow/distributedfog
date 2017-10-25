---
title: "Resin.io"
type: "article"
description: "Resin.io offers a development and deployment framework based upon Linux and containers that is designed to facilitate control of the on-device environment, provision devices on the network, and manage a fleet of systems."
tags: ["software","API","cloud","linux"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="resin.io" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### The Good

- Developer friendly: iterate and push
- [20 supported](https://docs.resin.io/hardware/devices/) maker devices
- Container-based
- Open Source: [ResinOS](https://resinos.io/), [Balena](https://www.balena.io/)
- First 10 devices free
{{% /card %}}

{{% card size="4" %}}
| Features [...](https://resin.io/features/)      |
|---        |
| Control on-device environment |
| Provision devices easily |
| Manage device fleet at scale |
| Automate device fleet from own cloud |
| Encrypted communication |
| Continuous updates |
{{% /card %}}

{{% card size="8" small="docs.resin.io" %}}
[Resin.io](http://resin.io/) makes it simple to deploy, update, and maintain code running on remote devices. We are bringing the web development and deployment workflow to hardware, using tools like git and Docker to allow you to seamlessly update all your embedded linux devices in the wild. We handle cross-compilation, device monitoring, VPNs, and log collection, so you can focus on your product and not the infrastructure.

##### Code Deployment

We use the familiar and popular git version control tool to push your code changes to a remote repository on our build servers. Each resin.io application has a unique remote repository associated to it and all code changes on the master branch of this repository will be built and delivered to your device fleet. When our servers receive your changes on master a chain reaction is set in motion in which your code is built for the specified target architecture, bundled into a Docker container and then systematically rolled out to your fleet of devices in the field.

##### Building Containers

The method our builders use to build your code depends on the project you are pushing. If your project includes a Dockerfile, the builders will execute every command in the Dockerfile, from including the base OS you define, to installing packages, pulling git repositories, and running any other commands you specify.

Alternatively, if your project includes a package.json (i.e. a node.js project), then that will be used instead to create an implicit Dockerfile, which simulates the build process a node.js/npm project expects. In this way, we are able to transparently run node.js projects on resin.io, while taking advantage of some of Docker’s caching features.

A Dockerfile will always give you more power to fine-tune the build process, but it’s also good to start fast without one, since you can shift to a Dockerfile whenever you like. We will soon add more languages to the “first-class” support we give to node.js. Until then, any other language can be used by adding a Dockerfile. It’s important to note that the environment within which your code gets built will match the devices you use for your app. So if you’re for example pushing to an app containing BeagleBone Black devices, we’ll build your code in an ARMv7 environment, while for the Raspberry Pi B+ it would be ARMv6.

Now that you have a better view of the build and deployment process, you may want to read about how the resin.io device OS is composed and [what is installed on a device](https://docs.resin.io/understanding/understanding-devices).
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://resin.io/" "Resin.io">}}
    {{<listlink "https://resin.io/usecases/" "Use Cases">}}
    {{<listlink "https://resin.io/how-it-works/" "How it Works">}}
    {{<listlink "https://docs.resin.io/raspberrypi/nodejs/getting-started/" "Getting Started">}}
{{< /listcard >}}
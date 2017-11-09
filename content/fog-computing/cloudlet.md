---
title: "Cloudlet"
type: "article"
description: "A cloudlet is a mobility-enhanced small-scale cloud datacenter that is located at the edge of the Internet. The main purpose of the cloudlet is supporting resource-intensive and interactive mobile applications by providing powerful computing resources to mobile devices with lower latency. It is a new architectural element that extends today’s cloud computing infrastructure."
tags: ["software","virtualisation","distributed","cloud","edge"]
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="8" small="elijah.cs.cmu.edu" %}}
### Cloudlet VS Cloud
There is significant overlap in the requirements for cloud and cloudlet. At both levels, there is the need for: (a) strong isolation between untrusted user-level computations; (b) mechanisms for authentication, access control, and metering; ( c) dynamic resource allocation for user-level computations; and, (d) the ability to support a very wide range of user-level computations, with minimal restrictions on their process structure, programming languages or operating systems. At a cloud datacenter, these requirements are met today using the virtual machine (VM) abstraction. For the same reasons they are used in cloud computing today, VMs are used as an abstraction for cloudlets. Meanwhile, there are a few but important differentiators between cloud and cloudlet.

##### Rapid provisioning
Different from cloud data centers that are optimized for launching existing VM images in their storage tier, cloudlets need to be much more agile in their provisioning. Their association with mobile devices is highly dynamic, with considerable churn due to user mobility. A user from far away may unexpectedly show up at a cloudlet (e.g., if he just got off an international flight) and try to use it for an application such as a personalized language translator. For that user, the provisioning delay before he is able to use the application impacts usability.

##### VM handoff across cloudlets
If a mobile device user moves away from the cloudlet he is currently using, the interactive response will degrade as the logical network distance increases. To address this effect of user mobility, the offloaded services on the first cloudlet need to be transferred to the second cloudlet maintaining end-to-end network quality. This resembles live migration in cloud computing but differs considerably in a sense that the VM handoff happens in Wide Area Network (WAN).
{{% /card %}}

{{% card size="8" small="cisco.com" %}}
A cloudlet is a new architectural element  that arises from the convergence of mobile computing / IoT  and cloud computing.  It represents the middle tier of a 3-tier hierarchy:  mobile or IoT device cloudlet cloud. A cloudlet can be viewed as a "data center in a box" whose  goal is to "bring the cloud closer".    

A cloudlet has four key attributes:

- only soft state:   It is does not have any hard state, but may contain cached state from the cloud.  It may also buffer data originating from a mobile device (such as video or photographs) en route to safety in the cloud.  The avoidance of hard state means that each cloudlet adds close to zero management burden after installation:  it is entirely self-managing.    
- powerful, well-connected and safe:  It possesses sufficient compute power (i.e., CPU, RAM, etc.) to offload resource-intensive computations from one or more mobile devices.  It has excellent connectivity to the cloud (typically a wired Internet connection) and is not limited by finite battery life (i.e., it is plugged into a power outlet).    Its integrity as a computing platform is assumed; in a production-quality implementation this will have to be enforced through some combination of tamper-resistance, surveillance, and run-time attestation.
- close at hand:  It is logically proximate to the associated mobile devices. "Logical proximity" is defined as  low end-to-end latency and high bandwidth (e.g., one-hop Wi-Fi).   Often, logical proximity implies physical proximity.  However, because of "last mile" effects, the inverse may not be true: physical proximity may not imply logical proximity.
- builds on standard cloud technology: It encapsulates offload code from mobile devices in  virtual machines (VMs), and thus resembles classic cloud infrastructure such as Amazon EC2 and OpenStack.  In addition, each cloudlet has functionality that is specific to its cloudlet role. [Read more](http://elijah.cs.cmu.edu/)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://en.wikipedia.org/wiki/Cloudlet" "Cloudlet Wikipedia">}}
    {{<listlink "http://elijah.cs.cmu.edu/" "Cloudlet-based Edge Computing">}}
    {{<listlink "https://www.akamai.com/uk/en/products/web-performance/cloudlets/" "Akamai Cloudlets">}}
    {{<listlink "http://elijah.cs.cmu.edu/DOCS/satya-ieeepvc-cloudlets-2009.pdf" "The Case for VM-based Cloudlets in Mobile Computing">}}
    
{{< /listcard >}}
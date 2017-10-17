---
title: "Android Things"
type: "article"
tags: ["RTOS","google"]
description: "Android Things (codenamed/rebranded from Brillo) is an Android-based embedded operating system platform by Google. It is aimed to be used with low-power and memory constrained Internet of Things (IoT) devices, which are usually built from different microcontroller platforms."
date: 2017-10-11T17:56:48+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
Like updates for Android Phones, developers can push Google-provided OS updates and custom app updates using the same over-the-air infrastructure that Google uses for its products and services. This provides a pathway for security updates on IoT devices.
{{% /card %}}

{{% card size="4" %}}
Android Things was first launched at Google I/O 2015 and was called Brillo, the "underlying operating system for the internet of things". Additionally the [Weave API](https://developers.nest.com/weave/), the (cross platform) common language that will let Brillo devices, phones, and the internet all talk to one another was also announced.
{{% /card %}}

{{% card size="8" small="developer.android.com" %}}
Android Things allows developers to build a smart device using Android APIs and Google Services. This takes the usual Android development stack—Android Studio, the official SDK, and Google Play Services—and applies it to the IoT. Developers will be able to use the Google Weave protocol to communicate between devices along with Google APIs and Google Cloud services like Google Cloud Vision.

![Android Things Architecture](/img/articles/android-things-architecture.png "Android Things Architecture from developer.android.com")

Android Things extends the core Android framework with additional APIs provided by the Things Support Library. These APIs allow apps to integrate with new types of hardware not found on mobile devices.

The Android Things platform is also streamlined for single application use. System apps are not present, and your app is launched automatically on startup to immerse your users in the app experience. [More](https://developer.android.com/things/sdk/index.html)
{{% /card %}}

{{< listcard size="4" title="Links" >}}
    {{<listlink "https://developer.android.com/things/index.html" "Android Things Home">}}
    {{<listlink "https://developer.android.com/things/sdk/index.html" "SDK">}}
    {{<listlink "https://developer.android.com/things/training/first-device/create-studio-project.html" "Getting Started">}}
    {{<listlink "https://developer.android.com/things/hardware/raspberrypi.html" "Raspberry Pi 3 Support">}}
    {{<listlink "https://developer.android.com/things/hardware/hardware-101.html" "Hardware 101">}}
{{< /listcard >}}
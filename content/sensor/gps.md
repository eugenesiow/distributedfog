---
title: "GPS"
full: "Global Positioning System"
type: "article"
tags: ["navigation", "transport", "wearables", "mobile"]
date: 2017-10-11T16:24:18+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
GPS provides geolocation and time information to a receiver anywhere on or near the Earth. It  does not require the user to transmit any data, and it operates independently of any telephonic or internet reception.
{{</card>}}

{{% card size="4" %}}
### Research
[Stanford GPS Lab](https://gps.stanford.edu/publications/all-publications), [Supply Chains](http://ieeexplore.ieee.org/abstract/document/6041225/), [Indoor Navigation](https://pdfs.semanticscholar.org/68ca/cbf271518bbf6f6d177b978f962c9acae0c2.pdf)
{{% /card %}}

{{% card size="4" %}}
### Alternatives
__GLONASS__ is the most developed of the GPS alternatives, and is operated by Russia. 
Quora [article](https://www.quora.com/What-alternatives-are-there-to-GPS-considering-those-satellites-would-be-the-first-things-knocked-out-in-a-war) on alternatives.
{{% /card %}}

{{% card size="8" small="sparkfun.com" %}}
##### How does a GPS receiver calculate its position and time?

The data sent down to earth from each satellite contains a few different pieces of information that allows your GPS receiver to accurately calculate its position and time. An important piece of equipment on each GPS satellite is an extremely accurate atomic clock. The time on the atomic clock is sent down to earth along with the satellite’s orbital position and arrival times at different points in the sky. In other words, the GPS module receives a timestamp from each of the visible satellites, along with data on where in the sky each one is located (among other pieces of data). From this information, the GPS receiver now knows the distance to each satellite in view. If the GPS receiver’s antenna can see at least 4 satellites, it can accurately calculate its position and time. More from [GPS Fundamentals](https://cdn.sparkfun.com/datasheets/Sensors/GPS/fundamentals_of_gps_receivers-v1.pdf) by Dan Doberstein. Also read about [GPS accuracy](https://learn.sparkfun.com/tutorials/gps-basics#gps-accuracy-) and [reading GPS data](https://learn.sparkfun.com/tutorials/gps-basics#reading-gps-data) on SparkFun.
{{% /card %}}

{{< listcard size="4" title="Learn">}}
    {{<listlink "https://learn.sparkfun.com/tutorials/gps-basics" "SparkFun's GPS Tutorial">}}
    {{<listlink "https://www.sparkfun.com/pages/GPS_Guide" "GPS Buying Guide">}}
    {{<listlink "https://developer.android.com/guide/topics/location/strategies.html" "Android Location Tutorial">}}
    {{<listlink "https://developer.apple.com/documentation/corelocation" "iOS Location API">}}
    {{<listlink "https://playground.arduino.cc/Tutorials/GPS" "Arduino GPS Guide">}}
    {{<listlink "http://www.libelium.com/development/waspmote/documentation/gps-programming-guide/" "Libelium GPS Guide">}}
{{< /listcard >}}
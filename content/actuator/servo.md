---
title: "Servo"
full: "Servomechanism"
type: "article"
description: "In control engineering a servomechanism, sometimes shortened to servo, is an automatic device that uses error-sensing negative feedback to correct the action of a mechanism. It usually includes a built-in encoder or other position feedback mechanism to ensure the output is achieving the desired effect. The term correctly applies only to systems where the feedback or error-correction signals help control mechanical position, speed or other parameters."
tags: ["industrial","control"]
date: 2017-10-11T16:24:18+01:00
---

{{<card size="4" small="Wikipedia" style="info">}}
{{<description>}}
{{</card>}}

{{% card size="4" %}}
### Servomotor

A servomotor is a specific type of motor that is combined with a rotary encoder or a potentiometer to form a servomechanism. This assembly may in turn form part of another servomechanism. A potentiometer provides a simple analog signal to indicate position, while an encoder provides position and usually speed feedback, which by the use of a PID controller allow more precise control of position and thus faster achievement of a stable position (for a given motor power). Potentiometers are subject to drift when the temperature changes whereas encoders are more stable and accurate. [Read more](https://en.wikipedia.org/wiki/Servomotor)
{{% /card %}}

{{% card size="4" %}}
### Radio Control

Servos (also RC servos) are small, cheap, mass-produced servomotors or other actuators used for radio control and small-scale robotics. 

Most servos are rotary actuators although other types are available. Linear actuators are sometimes used, although it is more common to use a rotary actuator with a bellcrank and pushrod. Some types, originally used as sail winches for model yachting, can rotate continuously. [Read more](https://en.wikipedia.org/wiki/Servo_(radio_control))
{{% /card %}}

{{% card size="8" %}}
### Applications
##### Position control
Globe control valve with pneumatic actuator and "positioner". This is a servo which ensures the valve opens to the desired position regardless of friction
A common type of servo provides position control. Commonly, servos are electrical, hydraulic or pneumatic. They operate on the principle of negative feedback, where the control input is compared to the actual position of the mechanical system as measured by some sort of transducer at the output. Any difference between the actual and wanted values (an "error signal") is amplified (and converted) and used to drive the system in the direction necessary to reduce or eliminate the error. This procedure is one widely used application of control theory. Typical servos can give a rotary (angular) or linear output.

##### Speed control
Speed control via a governor is another type of servomechanism. The steam engine uses mechanical governors; another early application was to govern the speed of water wheels. Prior to World War II the constant speed propeller was developed to control engine speed for maneuvering aircraft. Fuel controls for gas turbine engines employ either hydromechanical or electronic governing.

##### Others
Positioning servomechanisms were first used in military fire-control and marine navigation equipment. Today servomechanisms are used in automatic machine tools, satellite-tracking antennas, remote control airplanes, automatic navigation systems on boats and planes, and antiaircraft-gun control systems. Other examples are fly-by-wire systems in aircraft which use servos to actuate the aircraft's control surfaces, and radio-controlled models which use RC servos for the same purpose. Many autofocus cameras also use a servomechanism to accurately move the lens. A hard disk drive has a magnetic servo system with sub-micrometre positioning accuracy. In industrial machines, servos are used to perform complex motion, in many applications.
{{% /card %}}

{{< listcard size="4" title="Products">}}
    {{<listlink "https://www.jlab.org/ir/MITSeries/V25.PDF" "Servo Systems Paper">}}
    {{<listlink "https://en.wikipedia.org/wiki/Servomechanism" "Wiki">}}
    {{<listlink "http://www.instructables.com/id/IoT-Motion-Controlled-Servos/" "IoT Motion Controlled Servos">}}
{{< /listcard >}}
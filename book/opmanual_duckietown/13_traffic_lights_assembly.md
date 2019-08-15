# Traffic Lights Assembly {#traffic-light-assembly status=ready}

<div class='requirements' markdown="1">

Requires: Material: Traffic light components. To obtain them contact info@duckietown.org.

Requires: An [initialized SD-card](+opmanual_duckiebot#setup-duckiebot).

Requires: Tools: (strong) wood glue or hot glue gun, tape, double-sided tape.

Result: Traffic light.    
</div>  


Traffic lights are useful to coordinate traffic at intersections. Traffic lights can be used at three or four way intersections. Hardware wise, Traffic lights are Duckiebots without wheels, and a beautiful different chassis.

Reminder: for traffic lights to be recognized by Duckiebots, appropriate signage must be placed at intersections (traffic light traffic sign instead of stop sign).

This section describes the physical assembly and installation of traffic lights.  

## Overview

<!--

Traffic lights are crucial parts in modern cities. We rely on them to have well-organized traffic. While autonomous cars could communicate with each other through so many different kinds of protocols, humans can't. Unless you are a terminator, or a RoboCop, or Neo. In the near future where autonomous cars drive with human drivers, we still need the help of traffic lights.

-->

Traffic lights are composed of two wooden stands standing on opposing sides of the diagonal direction of an intersection. One of them is equipped with the computational stack and connection to a camera, the other one only serves as physical support for the tube.
The stand with the computational stack inside is designed to fulfill the purpose needed for a traffic light as well as serving as a Watchtower. A Watchtower is a system which is used in [Autolabs](+opmanual-autolab#part:autolab-definition) to  serve as localization system. As the hardware is exactly the same, we will first jump to the [instructions to build a Watchtower](+opmanual_autolab#part:watchtower-hardware) and then come back to this section to make the adjustments needed to turn a Watchtower into a traffic light. You do not need to understand what the purpose of a Watchtower is to finish the assembly of your traffic light. If you are interested in the functionality of the localization system though, you will find [this section](+opmanual_autolab##part:autolab-localization) interesting. A picture of the final result is found in[](#fig:TL-25).

<!--

Traffic lights node are expected to launch whenever they turn on.

-->

## Assembly of the traffic light parts

This section shows how to assemble the components from the laser cut traffic light parts.

Warning: The small parts with the hole in the middle, i.e., the ones in the top part of [](#fig:G2-1), are not all equal. Some have a round hole, others a polygonal hole. Double check you are using the right ones in the process (compare with the pics).

All parts should be glued together as showed in the pictures for enhanced structural stability.

### Build the Stand for the Raspberry Pi, a.k.a. a Watchtower

As previously mentioned, we will start by building the stand with the Raspberry Pi inside, using the instructions from [here](+opmanual_autolab#part:watchtower-hardware).


### Tube holder with small ground plate

<div figure-id="fig:G2-1">
<img src="images/G2-1.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-2">
<img src="images/G2-2.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-3">
<img src="images/G2-3.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-4">
<img src="images/G2-4.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-5">
<img src="images/G2-5.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-6">
<img src="images/G2-6.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:G2-7">
<img src="images/G2-7.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  



### Traffic light LED housing

<div figure-id="fig:L-1">
<img src="images/L-1.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:L-2">
<img src="images/L-2.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:L-3">
<img src="images/L-3.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:L-4">
<img src="images/L-4.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:L-5">
<img src="images/L-5.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:L-6">
<img src="images/L-6.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  



### Joint module

<div figure-id="fig:J-1">
<img src="images/J-1.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-2">
<img src="images/J-2.jpg" style="width: 40%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-3">
<img src="images/J-3.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-4">
<img src="images/J-4.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-5">
<img src="images/J-5.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-6">
<img src="images/J-6.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-7">
<img src="images/J-7.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:J-8">
<img src="images/J-8.jpg" style="width: 50%"/>
<figcaption>
</figcaption>
</div>  

## Components of the traffic light {#tl-mat}

Now that you have assembled the traffic light chassis, you are ready to add the electronics.

<div figure-id="fig:tl_components">
<img src="images/TL-01.jpg" style="width: 100%"/>
<figcaption>
Parts of a traffic light needed to complete these instructions.
</figcaption>
</div>



These components are needed for one traffic light:

* Tube holder with big ground plate
* Tube holder with small ground plate (Duckietown)
* Cable with soldered LED strip
* Joint module (2x)
* Traffic light LED housing
* Raspberry Pi base plate
* Ground module cover (Duckietown)
* Camera mount
* Camera mount cover
* Short tube
* Medium tube (2x)
* Long tube with hole at the side
* Raspberry Pi
* Raspberry Pi shield
* M2.5x10 MF Nylon spacers (8x)
* M2.5x8 Nylon screws (4x)
* SD card with Duckietown software
* USB cable
* Ethernet cable

Additionally, the traffic light structure can host:

* Traffic sign stands (4x)
* Traffic sign stand supports (4x).


## Assembling the Traffic Light



### Put the LEDs into the housing

Bend the LED strip at an angle to reduce the chance that the exposed soldered wires short. The exposed part of the wires should **not** be in contact, **especially** when turning on the power.

Warning: the actual traffic light in your hands might vary slightly from the pictures above. In particular, the electrical cables could have different colors or be soldered in different positions. Take note of what each color cable is soldered to, as same will go go with same on the other end.


<div figure-id="fig:L-0">
<img src="images/L-0.png" style="width: 80%"/>
<figcaption>
Bended LED strip cable
</figcaption>
</div>

<div figure-id="fig:TL-02">
<img src="images/TL-02.jpg" style="width: 80%"/>
<figcaption>
Cable with soldered LED strip LED housing
</figcaption>
</div>  
<div figure-id="fig:TL-03">
<img src="images/TL-03.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Carefully push the LEDs into the designated holes.
<div figure-id="fig:TL-05">
<img src="images/TL-05.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-04">
<img src="images/TL-04.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Fix the LEDs with some tape, don't use glue.
<div figure-id="fig:TL-06">
<img src="images/TL-06.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>

### Connect the tubes


<div figure-id="fig:TL-07">
<img src="images/TL-07.jpg" style="width: 80%"/>
<figcaption>
Medium tubes and LED housing.
</figcaption>
</div>  
Stick the tubes into the sides of the LED housing and pull the cable through one side.
<div figure-id="fig:TL-08">
<img src="images/TL-08.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Add the joint modules on the side of the tube without the cable.  
<div figure-id="fig:TL-09">
<img src="images/TL-09.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  

<div figure-id="fig:TL-10">
<img src="images/TL-10.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>    
Mount the other joint module on the long tube, such that it aligns with the hole.

You can add additional tape under the joint modules to prevent them to slip down.
<div figure-id="fig:H-1">
<img src="images/H-1.png" style="width: 80%"/>
<figcaption>
Fully assembled traffic light.
</figcaption>
</div>


<div figure-id="fig:TL-11">
<img src="images/TL-11.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-12">
<img src="images/TL-12.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-13">
<img src="images/TL-13.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Pull the cable through longer tube and stick the tube into the joint module.
<div figure-id="fig:TL-14">
<img src="images/TL-14.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-15">
<img src="images/TL-15.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Put the tubes into the tube holders.  

<div figure-id="fig:TL-16">
<img src="images/TL-16.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-17">
<img src="images/TL-17.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>


### Connect the Raspberry Pi


Use the spacers and the screws to mount the Raspberry Pi on the Raspberry Pi ground plate as shown in [](#fig:TL-18).

<div figure-id="fig:TL-18">
<img src="images/TL-18.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Plug the shield on top of the Raspberry Pi.  
Insert the SD card.  
Connect the LED cable to the shield.  
Connect the Ethernet cable.  
Connect the USB cable.
<div figure-id="fig:TL-19">
<img src="images/TL-19.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
If done correctly the LEDs should be on.  
<div figure-id="fig:TL-20">
<img src="images/TL-20.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
Close the ground module with the case.    

<div figure-id="fig:TL-21">
<img src="images/TL-21.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>
<div figure-id="fig:TL-22">
<img src="images/TL-22.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>

### Add traffic sign stands
<div figure-id="fig:TL-23">
<img src="images/TL-23.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  
<div figure-id="fig:TL-24">
<img src="images/TL-24.jpg" style="width: 80%"/>
<figcaption>
</figcaption>
</div>  

### Fully assembled traffic light

<div figure-id="fig:TL-25">
<img src="images/TL-25.jpg" style="width: 80%"/>
<figcaption>
Fully assembled traffic light.
</figcaption>
</div>

Place the traffic light at an intersection such that the LEDs are exactly in the middle and are facing each incoming lane perpendicularly.

You can verify the position is correct by verifying that Duckiebots at the red stop lines can see only one light blinking, and no reflections of LEDs facing other directions.

You can finally use the provided double-sided tape pads to fix the traffic light to the tiles.

### SD-card image Preparation {#dt-ops-tl-prep status=ready}

At hardware and software level, traffic lights are Duckiebots without wheels. In initializing the SD-card of your traffic light, treat is as if it were a Duckiebot: [](+opmanual_duckiebot#setup-duckiebot). Don't forget the `--compress` option for 16GB sd cards.

- For Robotarium users: since traffic lights are coupled to watchtowers, please use the watchtower setup:
        hostname : watchtowerXX
        linuxname : mom
        password: MomWatches

- However, if you just want to use it as a traffic light, use the trafficlight setup:
        hostname : trafficlightXX
        linuxname : tlo
        password: quackquack

After this step, you should have a traffic light image name.

    tlo@trafficlight01.local
or

    mom@watchtower01.local


<!--

`DB17` instructions

Prepare a Duckiebot image following the instructions on `DB17` Duckiebot initialization and remember to generate the new machine file.


See setup-duckiebot
and this chapter
See rc-control


`DB18` instructions {#dt-ops-tl-init status=draft}
 write detailed instruction, verify functionality with docker infrastructure

-->

### Launch Traffic Lights {#dt-ops-tl-launch status=ready}
To download and run the trafficlight docker image, simply run:

    docker -H ![hostname].local run -dit --privileged --name trafficlight --network=host duckietown/traffic-lights:master18


<!--

Semantics of LEDS {#LED-semantics status=draft}

headlights: white, constant

Assumption:

- **20 fps** to do LED detection

- 1s to decide

- 3 frequencies to detect

tail lights: red, **6 hz square wave**

traffic light "GO" = green, **1 hz square wave**

traffic light "STOP" = red, **1.5 Hz** square wave**

duckie light on top, state 0 = off

duckie light on top, state 1 = blue, **3 Hz, square wave**

duckie light on top, state 2 = ?, **2.5 Hz square wave**

duckie light on top, state 3 = ?, **2 Hz square wave**

verify if this info is still up to date.

-->

Here we document our build of Ben Eater's 8-bit breadboard computer. 

## Contents
* [Project Overview](#project-overview)
* [Setup](#setup)
* [Clock Module](#clock-module)
* [Registers](#registers)
* [ALU](#alu)
* [RAM](#ram)
* [Program Counter](#program-counter)
* [Display](#display)
* [Control Unit](#control-unit)
* [Programming](#programming)

## Project Overview

## Setup

## Clock Module
We followed along with [Ben's first video for the clock module](https://www.youtube.com/watch?v=kRlSFm519Bo&list=PLowKtXNTBypGqImE405J2565dvjafglHU&index=2&ab_channel=BenEater). We assembled the clock as Ben did in the video using the parts from the kit. 

**Problem: Ben's Kit Doesn't Include a 100K Resistor**

When we powered the circuit, we found that the LED was faintly lit, but it was not blinking. After unsuccessfully troubleshooting for a bit, we [asked the r/beneater subreddit for assistance](https://www.reddit.com/r/beneater/comments/1ktz0w6/help_with_clock/) and quickly received a number of helpful replies. We learned that the problem was with the 1K resistor we used. In the video, Ben uses a 100K resistor, but his kit only includes, 220, 1K, and 1M resistors. We used the 1K resistor instead of the 100K, but this turned out to be a mistake. The clock speed depends on the resistor. The less resistance, the speedier the clock. Since we used a resistor that was 100 times weaker than the resistor Ben uses in the video, the clock was blinking too fast to see. Following advice from Reddit, we swapped the 1K resistor for a 100K we had on hand, and it solve the problem. If you don't have a 100K resistor, you can proceed to the end of the video where Ben adds a potentiometer. The potentiometer is included in the kit and provides sufficient resistance to slow the clock down enough to see the LED blink. 

![clock_resistor_problem_1](https://github.com/user-attachments/assets/15e0650c-3ba0-44df-b79b-a7fdd49dce10)

**Potentiometer Issue**
One issue we ran into while following along with the [second clock module video](https://youtu.be/81BgFhm2vz8) was that the potentiometer sometimes got knocked lose when we accidentally bumped it. We were able to secure the potentiometer a little better by straightening out the pins, but we still need to be careful not to bump it.

![clock_video_2](https://github.com/user-attachments/assets/d619e982-e294-4983-ba80-3329a376d1de)

## Registers
We tried to keep all wires visible and accessible. This required us to elevate some of the wires slightly.
![IMG_1824_register](https://github.com/user-attachments/assets/10e443b8-69e8-430a-96da-649f1e6f3bbb)

## Bus
We used extra power rails from the breadboard to create the bus. 
![IMG_1833_bus](https://github.com/user-attachments/assets/2b9e8d12-551f-4b52-a448-fb2bcac3d651)

We soldered resistors to the bus LEDs and connected the cathodes together. Our soldering skills are not the best. 
![IMG_1815_ugly_soldering](https://github.com/user-attachments/assets/f778e9f4-b6e2-4ebe-a6d4-48250835b111)

## ALU
The ALU wiring is complex because, so we needed to be creative to avoid overlapping as much as possible. 
![IMG_1834_ALU](https://github.com/user-attachments/assets/4f365334-177a-4c75-b537-c32847a4a97f)

ALU adding by 1: 
![ALU_GIF](https://github.com/user-attachments/assets/77cb6284-b2e1-497d-b318-f1efe95fa001)

## RAM

## Program Counter

## Display

## Control Unit

## Programming

#### Parts List
* 1 × Breadboard (High quality BusBoard Prototype Systems BB830)
* 1 × 140-piece jumper wire kit
* 3 × LM-555 Timer ICs
* 1 × 74LS04 Hex inverter
* 1 × 74LS08 Quad 2-input AND gate
* 1 × 74LS32 Quad 2-input OR gate
* 10 × Yellow LEDs
* 5 × Blue LEDs
* 1 × Momentary tact switch
* 1 × SPST slide switch
* 1 × 1MΩ potentiometer
* 5 × 220Ω resistors
* 5 × 1KΩ resistors
* 5 × 1MΩ resistors
* 5 × 0.01µF capacitors
* 5 × 0.1µF capacitors
* 5 × 1µF capacitors
* 5 × 10µF capacitors
* 1 × 10 watt AC-to-DC regulated switching wall adapter (US)
* 1 × DC jack to screw terminal adapter for connecting power


---
layout: post
title:  Cal AIAA
tags: [rover, aiaa, competition, team, lead]
main_image: /assets/blog_pictures/2017-12-rover-full-assembly-render-1.jpg
main_image_alt: URC 2018 Rover Design
---

# Cal AIAA
I started out Sophmore year as the Software & Computer Systems Lead for the Rover Team and worked my way to President of the club and Project Manager for the Rover Team.

# Rover Team

## University Rover Challenge 2018
Large refactors and improvments using URC 2017 design as a base.
- Electrical Design: <br />
  Performed component selection, analysis, and simulation for all aspects of the rover control systems. Included developing from scratch a dual motor control using [KiCAD](http://kicad-pcb.org/), [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html), and an [Othermill Pro](https://www.bantamtools.com/products/bantam-tools-desktop-pcb-milling-machine). Specifically, designed circuitry and control code using the following:
    - [Roboclaw 2x60A](http://www.basicmicro.com/RoboClaw-2x60A-Motor-Controller_p_8.html)
    - [PDX256:1 Gearmotor](http://www.robotmarketplace.com/products/0-pdx256.html)
    - [PDX104:1 Gearmotor](http://www.robotmarketplace.com/products/0-pdx104.html)
    - [CM-785HB Servo](https://www.servocity.com/cm-785hb-servo-gearbox#197=4&198=9)
    - [HSR-2645CR Servo](https://www.servocity.com/cm-2645crh-cr-servo-gearbox)
    - [Zippy Flightmax 3S1P 5000mAh](https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-40c.html)
    - [AEAT-6600-T16 Magnetic Encoder](https://www.broadcom.com/products/motion-control-encoders/magnetic-encoders/aeat-6600-t16)
    - [ADA746 GPS Breakout Module](https://www.amazon.com/gp/product/B01H1R8BK0)
    - [Arty Z7: APSoC Zynq-7000](https://store.digilentinc.com/arty-z7-apsoc-zynq-7000-development-board-for-makers-and-hobbyists/)
    - [DE0-Nano: Cyclone IV FPGA](https://www.terasic.com.tw/cgi-bin/page/archive.pl?Language=English&CategoryNo=165&No=593&PartNo=1)
    - [Analog Discovery 2](https://store.digilentinc.com/analog-discovery-2-100msps-usb-oscilloscope-logic-analyzer-and-variable-power-supply/)
- Software: <br />
  Authored a three program multi-threaded control system from scratch that reliably handled multiple user clients/commands and safely managed the rover hardware. The first program consisted of a frontend GUI written in Qt Creator. The GUI was the users main point of interaction with the rover. It contained buttons, sliders, a 3D live view generation of the arm, and dials for controlling all aspects of the rover. Inbetween the client and rover existed the second program, a server responsbile for managing user permissions and handling the low bandwith rover connection (both camera and commands tunneled through this for pipelining and verification). Lastly, the third program was an embedded C/Verilog application that handled requests from the server and directly managed the hardware systems on the rover. This package was extermely modular with simple class/structure definitions to flexibly adjust to any expansions or new features. For instance, some modules we needed to create were: communication modules for magnetic absolute encoder ICs, quadrature encoders, our high power motor controllers (), and servos.
- Mechanical Design: <br />
  Helped mechanical teams work through issues with designing and building the rover. Included troubleshooting for our six wheeled rocker bogie system with completly turnable wheels. Provided guidance and feedback from a control prespective and aided in setting up mount points for electrical systems.

Watch our [2018 System Acceptance Review (SAR)](https://www.youtube.com/watch?v=YEJpmT6PJ08). The github group for this team can be found [here](https://github.com/cal-roboops).

## University Rover Challenge 2017

## Robo-Ops 2016
![2016 Robo-Ops Design](/assets/blog_pictures/2016-08-aiaa-rover-robo-ops-1.jpg)


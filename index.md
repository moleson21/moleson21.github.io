---
id: main_index
---
# About Me
Hello! My name is Mitchell and I am a UC Berkeley graduate who majored in Mechanical Engineer and Electrical Engineering & Computer Science. I am extremely passionate about hardware systems and the software that supports them. Throughout my professional work and in the clubs/classes at Berkeley, I have utilized my multi-disciplinary skillset to develop advanced solutions to challenging problems. I enjoy tinkering with hardware to create efficient and cost effective solutions in addition to writing my own embedded software to further optimize space and speed constraints.

Outside of school & work, I enjoy camping and have achieved the Eagle Scout rank in the [Boy Scouts of America](https://www.scouting.org/). Most recently, I traveled for three weeks up the US-101 along the California and Oregon coast then back down through Crater Lake and Lassen National Parks.

# Recent Posts
<div style="width:100%; float:left" markdown="1">
{% for post in site.posts limit:5 %}
<div style="font-size:80%; width:20%; word-wrap:break-word; text-align:center; float:left;" markdown="1">
<a href="{{ post.url }}">
<img src="{{ post.main_image }}" alt="{{ post.main_image_alt }}" style="padding-bottom:0.5em;"/>
<br />
{{ post.title | truncate: 75}}
<small>{{ post.date | date: "%m/%d/%Y" }}</small>
</a>
</div>
{% endfor %}
</div>

[See all posts](blog/)

# Professional Experience
See my [LinkedIn](https://www.linkedin.com/in/mitchell-oleson-42381a101/) for more detailed and up to date information. In short, I have previously worked for:

- [SpaceX](https://www.spacex.com/): <br />
  Spent two summers (one as a Launch Intern and another as an Associate Engineer) at the SpaceX Vandenberg launch site. During both of these experiences, I was involved wtih ground side command & control deployment, camera installation/configuration/control, system management, sensor troubleshooting, and camera control software creation.

- [Intel](https://www.intel.com): <br />
  Spent a summer as a technical intern benchmarking new Optane Memory solutions using SYSMark 2014, PCMark Vantage/8, 3DMark, and IOMeter across numerous system configurations. Additionally, I authored a whitepaper that put forth compelling reasons why current benchmarking needs to be adjusted by analyzing datasets generated across numerous computers and user workloads.


# Projects

- [uC Interface](https://moleson21.github.io/uc-interface) <br />
  This started out as a side project and has slowly grown both in scope and capabilities. It started out as a simple interface for controlling an arduino via serial for rapidily bringing up hardware testing systems with little to no software & hardware modifications for Berkeley Hyperloop. In this use case, we had a varying number solenoids to control as well as some analog temperature sensors to monitor. Since the intial creation, I have added the ability to dynamically set aspects of the program via a config file, added support for TCP & UDP connections, added checksums for command verification, modified the transmission protocol for dynamic length adjustment, and added new interfaces for expanded functionality.

- [Cal AIAA](https://aiaa.berkeley.edu/) <br />
  This was the primary competition team I was involved with during college and we competed in both the [University Rover Challenge](http://urc.marssociety.org/) hosted by the Mars Society and [Design Build Fly](https://www.aiaadbf.org/) hosted by AIAA competitions. See [this post](2018/12/10/cal-aiaa-club.md) for further information on this team and what we did.

- [Berkeley Hyperloop](https://berkeleyhyperloop.com/) <br />
  See [this post](2018/12/10/berkeley-hyperloop-club.md) for further information about this team and what we did. 

- FPGA RISC-V Softcore <br />
  Developed a three stage CPU for the [RISC-V](https://riscv.org/) instruction set. Included developing software implementations for button debouncing, quadrature encoders, communication to onboard audio/VGA/HDMI output chips, and UART/I2C/SPI protocols.

- Compiler <br />
  Wrote a compiler for a subset of the python language. The compiler consisted of the following three stages:
  1. Lexer & Parser: Took a source file and produced an abstract syntax tree (AST) utilizing FLEX and BISON
  1. Static Analyzer: Takes the AST from stage 1 as input and performs static correctness checks and annotates with identifier information (indexed declarations and links id & typevar to declarations) before outputing another AST
  1. Code Generation: Takes the AST from stage 2 as input and outputs a C equivalent program (including required libraries) for final compilation and running

- Pintos <br />
  Wrote a basic operating system and priority schedular in C. Included creating a mutex & semaphore structures that correctly adjust priorty of threads. Utilized [QEMU](https://www.qemu.org/) for testing and running the OS.

- [Crust OS](https://github.com/moleson21/crust-os) <br />
  A basic operating system written in Rust. Gained experience working with assembly code and understanding how the lowest level of an OS works. Hoping to continue its expansion as a side project. Utilized [QEMU](https://www.qemu.org/) for testing and running the OS.

- [Balancing Cube](https://github.com/moleson21/ME135_BalancingCube) <br />
  Designed and developed a cube that would jump up and balance on one if its sides or points. Using three flywheels (one along each axis), the cube attempted to stabalize itself by spinning each of these up in response to a 6-axis MPU that was fixed to the cube body. This project took inspirtion from and sought to mimic [The Cubli](https://www.youtube.com/watch?v=n_6p-1J551Y).

- [Air Doodle](https://github.com/williampsmith/air-doodle) <br />
  This projects goal was to develop a wearable device that was capable of recognizing buttons and letters traced out by a user. In order to achieve this, we used a 6-axis MPU, the [Gesture Recognition Toolkit (GRT)](https://github.com/nickgillian/grt), and a small microcontroller mounted to a glove. In order to capture a digit, the user would tap a button present on the thumb (easily done by pressing the thumb and pinky together) and then draw their desired character using their index finger in 3-space. During the drawing phase, the microcontroller polled an onboard 6-DOF accelerometer/gyro for data. This data was entered into a timeseries that, upon release of the button, was fed as an argument into a spawned thread for analysis wth our trained GRT model. The final classification was logged locally, as well as, sent across a bluetooth connection to an Arduino that was connected to a small LED Matrix display. This data was then presented on the LED Matrix display.

- [Connection Tester](https://github.com/moleson21/connection-tester) <br />
  Similar to my [uC Interfacer](https://moleson21.github.io/uC-Interface) project, this started out as a project to optimize testing of our hardware systems on the Rover Team. Originally, it served as a proxy rover, server, or client connection which allowed us to monitor and inject command packets. This helped us verify functionality and test edge cases that would've been hard to simulate during the development/prototyping phase. Since this use, I have tweaked the interface a bit for usability and fixed some errors that the team located as they continued to use it.

- Python Secure File Server <br />
  Created a python program for securly storing, sharing, and protecting files on an unsecure remote storage system. Used RSA Encryption, Symmetric Key Block Ciphers, and Hash MACs for securly storing, downloading, and verifying data.

- Misc Smaller Projects
  - [OwnCloud](https://owncloud.org/) File Server: Setup and hosted a private OwnCloud file server instance using an Ubuntu server running in Windows Hyper-V.
  - Chess: Created a Java chess game with simple GUI for seeing the board and controlling the pieces


# Contact Info
moleson21 [at] gmail [dot] com <br />
[LinkedIn](https://www.linkedin.com/in/mitchell-oleson-42381a101/) | [Github](https://moleson21.github.com)


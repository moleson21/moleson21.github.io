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
  This was the primary competition team I was involved with during college and we competed in both the [University Rover Challenge](http://urc.marssociety.org/) hosted by the Mars Society and [Design Build Fly](https://www.aiaadbf.org/) hosted by AIAA competitions. I started out Sophmore year as the Software & Computer Systems Lead for the Rover Team and worked my way to President of the club and Project Manager for the Rover Team.
  
  - Electrical Design: <br />
    Performed component selection, analysis, and simulation for all aspects of the rover control systems. Included developing from scratch a dual motor control using [KiCAD](http://kicad-pcb.org/), [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html), and an [Othermill Pro](https://www.bantamtools.com/products/bantam-tools-desktop-pcb-milling-machine).
  - Software: <br />
    Authored a three program control system that reliably handled multiple user clients/commands and safely managed the rover hardware. The first frontend GUI written in Qt Creator. The command handler and connection manager server. The backend rover client. Developed embedded software to communicate with magnetic absolute encoder ICs, quadrature encoders, high pwoer motor controllers, and servos.
  - Mechanical Design: <br />
    Provided guidance and feedback from a control prespective and aided in setting up mount points for electircal systems.
  
  Watch our [2018 System Acceptance Review (SAR)](https://www.youtube.com/watch?v=YEJpmT6PJ08). The github group for this team can be found [here](https://github.com/cal-roboops).

- [Berkeley Hyperloop](https://berkeleyhyperloop.com/) <br />
  The github group for this team can be found [here](https://github.com/Berkeley-Hyperloop).

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
  A basic operating system written in Rust. Utilized [QEMU](https://www.qemu.org/) for testing and running the OS.

- [Balancing Cube](https://github.com/moleson21/ME135_BalancingCube)

- [Air Doodle](https://github.com/williampsmith/air-doodle)

- [Connection Tester](https://github.com/moleson21/connection-tester) <br />
  Similar to my [uC Interfacer](https://moleson21.github.io/uC-Interface) project, this started out as a project to optimize testing of our hardware systems for the Rover Team. It served as a proxy rover or server connection and allowed us to monitor and inject command packets. This helped us verify functionality and test edge cases that would've been hard to simulate during the development/prototyping phase.

- Python Secure File Server <br />
  Created a secure file server for storing, sharing, and protecting files using RSA Encryption, Symmetric Key Block Cipher, and Hash MAC.

- Misc Smaller Projects
  - Chess: Created a Java chess game with GUI
  - [OwnCloud](https://owncloud.org/) File Server: Setup and hosted a private OwnCloud file server instance using an Ubuntu server running in Windows Hyper-V.


# Contact Info
moleson21 [at] gmail [dot] com <br />
[LinkedIn](https://www.linkedin.com/in/mitchell-oleson-42381a101/) | [Github](https://moleson21.github.com)


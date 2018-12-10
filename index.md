---
id: main_index
title: Mitchell Oleson
description: Welcome to my website!
show_downloads: false
---
# About Me
Hello! My name is Mitchell and I am a UC Berkeley graduate who majored in Mechanical Engineer and Electrical Engineering & Computer Science. I am extremely passionate about hardware systems and the software that supports them. Throughout my professional work and in the clubs/classes at Berkeley, I have utilized my multi-disciplinary skillset to develop advanced solutions to challenging problems. I enjoy tinkering with hardware to create efficient and cost effective solutions in addition to writing my own embedded software to further optimize space and speed constraints.

Outside of school & work, I enjoy camping and have achieved the Eagle Scout rank in the [Boy Scouts of America](https://www.scouting.org/). Most recently, I traveled for three weeks up the US-101 along the California and Oregon coast then back down through Crater Lake and Lassen National Parks.

# Recent Posts
{% for post in site.posts limit:3 %}
  [![{{ post.title }}]({{ post.main_image }})]({{ post.url }})
{% endfor %}
<br />
<br />

# Professional Experience
See my [LinkedIn](https://www.linkedin.com/in/mitchell-oleson-42381a101/) for more detailed and up to date information. In short, I have previously worked for:

- SpaceX: <br />
  Spent two summers (one as a Launch Intern and another as an Associate Engineer) at the SpaceX Vandenberg launch site. During both of these experiences, I was involved wtih ground side command & control deployment, camera installation/configuration/control, system management, sensor troubleshooting, and camera control software creation.

- Intel: <br />
  Spent a summer as a technical intern benchmarking new Optane Memory solutions using SYSMark 2014, PCMark Vantage/8, 3DMark, and IOMeter across numerous system configurations. Additionally, I authored a whitepaper that put forth compelling reasons why current benchmarking needs to be adjusted by analyzing datasets generated across numerous computers and user workloads.


# Projects

- [uC Interface](https://moleson21.github.io/uc-interface) <br />
  This is a side project that has slowly grown in scope and capabilities. It started out as a simple IO GUI for controlling an arduino via serial to rapidily bring up the Berkeley Hyperloop teams hardware testing systems with little to no software & hardware modifications. For this use case, we had a varying number solenoids to control as well as some analog temperature sensors to monitor. Since then, I have added the ability to dynamically set various aspects of the program via a config file, added support for TCP & UDP connections, added checksums for verification, and modified the transmission protocol for minimal tranmission lengths and dynamic length adjustments.

- [Cal AIAA](https://aiaa.berkeley.edu/) <br />
  This was the primary team I was involved with starting Sophmore year as Software & Computer Systems Lead for the Rover Team. I later went on to become the President of Cal AIAA and Project Manager for the Rover Team. Through my time we spent a great deal of effort building from scratch a modular software system that utilizes a front end control client, middle manager server (to collate and enforce rover commands), and back end rover client that carried out/responded to requests from the server. Furthermore, I also worked closely with the mechanical engineers helping them design their systems with controlability in mind. This included placements of motors, encoders, servos, cameras, strain guages, and power distribution busses. We also attempted to design our own motor controller using [KiCAD](http://kicad-pcb.org/) and [LTSpice](https://www.analog.com/en/design-center/design-tools-and-calculators/ltspice-simulator.html), however, despite succesfully desgining, milling, assembling, and intial testing of a dual motor controller, it was found to be unfeasable as the required current wat too high for the copper thickness and available cooling. The github group for this team can be found [here](https://github.com/cal-roboops).

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

- [OwnCloud](https://owncloud.org/) File Server <br />
  Created and hosted a private OwnCloud instance using an Ubuntu server running in windows hyper-v.

- Misc Smaller Projects
  - Chess: Created a Java chess game with GUI


# Contact Info
moleson21 [at] gmail [dot] com <br />
[LinkedIn](https://www.linkedin.com/in/mitchell-oleson-42381a101/) | [Github](https://moleson21.github.com)

# BIOENG 0056 / BIOENG 2156 Curriculum Prototyping

The document below describes the ideas for a University of Pittsburgh "Workshop in Prototyping 2" for graduate bioengineering students. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to participate.

## Goals

- Students will be able to positively discuss the work completed in this course as part of an interview process.
- Students will be exposed to tools, terminologies, and frameworks used in software and embedded systems. Exposure will serve as the foundation for continued self-learning via online resources.

## Topics

### 1. Command-line interfaces

All modern operating systems have a command-line interface (CLI) for system maintenance and operation, be it Bash for Linux or macOS, or Powershell for Windows. Programming languages, including Python and C, implicitly expect knowledge of CLIs. Moreover, in order for students to understand many online resources, they must be comfortable using established tools on the command line.

The workshop will describe the basics of a CLI, with a focus on filesystem exploration and maintenance, software and package installation, version control, and remote management of machines. The workshop will touch on system troubleshooting and how to fix issues such as `command not found: python`. The knowledge will directly transfer into future workshops when students will remotely manage their Raspberry Pis from the command line.

### 2. Version control

As a co-op student, my colleagues and I did not follow best practices for software version control. Zipping up source files and passing them around as email attachments leads to confusion among developer teams, introduces software bugs, and slows down development. Familiar tools like Dropbox and Google Drive also fall short for software version control, as they are designed for a more general use case. Additionally, many online resources expect an understanding of version control systems, as is the case when installing some third-party libraries for Python.

The workshop exposes the students to Git, one of the most popular distributed version control systems (DVCS). The workshop builds on the CLI workshop, as the default Git interface is command-line driven. Students will be exposed to the concepts of git repositories, branches, commits, diffs, and merges. Upon completing the workshop, students will feel comfortable using Git for software version control and as a tool for managing software development across multiple developers. Students will create a free GitHub account that will be used (1) for developing and reviewing future workshop projects, and (2) as a public portfolio of their work.

### 3. Introduction to Python

Python is a versatile scripting language that can be used in multiple environments. Python allows developers to write less and get more done with a well-established standard library and numerous well-regarded (and free) third-party libraries. Python is the default language for the Raspberry Pi, and it is is widely used in the scientific community for data analysis and machine learning (numpy, TensorFlow).

The workshop teaches students the foundations of Python. Specifically, we will use Python 3 and discuss the differences between the Python 2 variant. Topics cover data types including numbers, strings, and `None`; functions; flow control including `if`, `while`, and `for`; collection types including lists, dictionaries, and sets; and classes and object-oriented programming. As an outcome, students will feel comfortable writing basic Python programs and comprehending online resources.

https://mciantyre.github.io/dhub-python/#/

### 4. Advanced Python

The Python module and library system might feel unfamiliar for students with existing programming experience (MATLAB). It becomes relevant for students to understand how Python programs are structured, and how students may make use of Python libraries. Additionally, Python is a highly-expressive language with what are called “Pythonic” idioms. Students will need to understand the meaning of these Pythonic idioms and how to use the idioms in their own programs.

Advanced Python covers the Python module system, particularly how the layout of Python scripts in the file system dictates the structure of a Python project. The workshop covers how Python libraries are installed and how to troubleshoot library installations. The workshop also covers some Pythonic idioms, including list and dict comprehensions and filtering; functions- and classes-as-data; tuple destructuring, multiple returns, and multiple assignment; and iterators and generators. Once complete, students should feel comfortable using libraries, creating Python modules, understanding Pythonic constructs used in libraries, and employing Pythonic constructs in their own programs.

### 5. Embedded systems: Raspberry Pi

The Raspberry Pi (RPi) is a popular single-board computer (SBC). The RPi is widely used as a platform for learning and system development. Online resources for the platform are abound. RPis are easy to setup and control, and they have a wide array of hardware input-output (I/O) for data acquisition and hardware actuation. As a result, RPIs may be the choice platform for IoT applications and embedded development.

The workshop teaches students how to configure a RPi for remote control and deployment. The discussion describes RPi hardware capabilities with a particular focus on communication protocols (SPI, I2C, UART, etc). The workshop concludes with an exploration into Python libraries that control hardware, allowing the students to use their Python knowledge to create applications with hardware sensing and control.

### 6. Embedded Systems: sensors and actuators

TODO flesh this out.

- ADCs and DACs; understanding bit resolution
- Accelerometrs, gyroscopes, magnetometers, IMUs
- Sampling and basics of DSP
- LEDs, buttons, motors
- Electrical control: MOSFETs, relays
- Interpreting data sheets and communication commands
- Online resources: Sparkfun, Adafruit, etc.
- Suppliers: Mouser, Digikey, Arrow, etc.

### 7. Embedded systems: Arduino

In cost- or power-constrained embedded systems, or for systems requiring deterministic timing (medical, aviation, etc), the RPi may not be the platform of choice. These contexts may require a bare-metal, low-cost microcontroller that is programmed in C. Although there are many available platforms, the Arduino is a simple and accessible microcontroller for learning and development.

Students are introduced to the Arduino and C programming. The workshop draws parallels to the RPi and Python with a focus on low-level software development. Topics include an introduction to C, data type sizes and memory allocation, and a dive into the Arduino programming environment. Upon completion, students will be able to write simple Arduino programs and understand online resources for C and Arduino programming.


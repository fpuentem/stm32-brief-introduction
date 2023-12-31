---
theme: default
marp: true
title: Introduction to Embedded Systems with STM32
paginate: true
---

# Introduction to Embedded Systems with STM32
### *Fabricio Renato Puente Mansilla*

---

# **Lecture A**:
# Introduction to Embedded Systems

---

# What is an Embedded System?
- **Embedded System**: Combination of hardware and software designed for a specific purpose within a larger system.
- Often dedicated to perform a single or a few functions.
- EXAMPLES: Microcontrollers, microprocessors, FPGA-based systems.

###### Reference: *Embedded Systems: Architecture, Programming, and Design* by Raj Kamal.

---

# Characteristics of Embedded Systems
## Key Characteristics
- **Real-time Operation**: Timely response to external events.
- **Constraints on Resources**: Limited memory, processing power, energy.
- **Reliability**: Critical in applications like medical devices and automotive systems.
- **Low Power Consumption**: Prolonged battery life in portable devices.

###### Reference: *Embedded Systems Design: An Introduction to Processes, Tools, and Techniques* by Arnold S. Berger.

---

# Examples in daily life
## Examples in Daily Life
- **Smartphones**: Combines communication, computation, and multimedia.
- **Automotive**: Engine control, safety systems, infotainment.
- **Home Appliances**: Washing machines, microwave ovens, thermostats.
- **Medical Devices**: Pacemakers, insulin pumps, medical imaging.

###### Reference: *Embedded Systems: Real-Time Operating Systems for Arm Cortex M Microcontrollers* by Jonathan Valvano.

---

# Differences between embedded systems and general-purpose computers
### Contrasting Embedded Systems & General-Purpose Computers
- **Dedicated Functionality**: Embedded systems have a specific purpose; general-purpose computers are versatile.
- **Resource Constraints**: Limited resources in embedded systems; computers have abundant resources.
- **Real-time Requirements**: Many embedded systems require real-time responses; general-purpose computers prioritize throughput.
- **Form Factor**: Embedded systems often compact; computers come in various sizes.

###### Reference: *Embedded Systems: A Contemporary Design Tool* by James K. Peckol.


---

# Overview of Microcontrollers

---

# What is a Microcontroller?
## Unveiling the Microcontroller Magic
- **Definition**: A compact integrated circuit (IC) that contains a processor, memory, and input/output peripherals.
- **Functionality**: Executes pre-programmed tasks, controls devices, and processes data.
- **Brains & Brawn**: Like the heart and muscles of an embedded system.

###### Reference: *The 8051 Microcontroller and Embedded Systems* by Muhammad Ali Mazidi.

---

# What is a Microcontroller?
## Exploring the Microcontroller Realm
- **Core Components**: CPU, RAM, ROM/Flash memory, timers, and I/O ports.
- **Variety**: Diverse microcontrollers for various applications (8-bit, 16-bit, 32-bit).
- **Applications**: Powering everything from washing machines to spacecraft!
- **Programming**: Develop code in languages like C/C++. And Python too.

###### Reference: *Embedded Microcontroller Interfacing: Designing Integrated Projects* by Gourab Sen Gupta.

---

# Key components
## Components in Detail
1. **CPU**: Represents the central processing unit that executes instructions.
2. **Program Memory**: This can be ROM (Read-Only Memory) or Flash memory where the program instructions are stored.
3. **Data Memory**: This is RAM (Random Access Memory) where temporary data is stored during program execution.

###### Reference: *Microcontroller Design Using 8051* by S. R. Deb.

---

# Key components
## Components in Detail
4. **I/O Ports**: These are the input/output pins that allow the microcontroller to communicate with external devices.
5. **Timers**: Hardware components used for generating time-based events or delays.
6. **ADC/DAC**: Analog-to-Digital Converter and Digital-to-Analog Converter for interfacing with analog signals.

###### Reference: *Embedded Systems: Introduction to Arm® Cortex™-M Microcontrollers* by Jonathan W. Valvano.

---

# How microcontrollers differ from microprocessors
## Unraveling the Distinctions
- **Microcontrollers**: All-in-one devices tailored for specific tasks.
- **Microprocessors**: General-purpose computing powerhouses.

###### Reference: *Embedded Systems: Architecture, Programming, and Design* by Raj Kamal.

---

# How microcontrollers differ from microprocessors
## Contrasting Characteristics
- **Functionality**: Microcontrollers are task-specific; microprocessors are versatile.
- **Components**: Microcontrollers have CPU, memory, I/O, timers; microprocessors focus on CPU.
- **Complexity**: Microcontrollers are simpler; microprocessors are more complex.
- **Cost**: Microcontrollers are cost-effective; microprocessors may be pricier.

###### Reference: *Microcontroller Theory and Applications: HC12 and S12* by Daniel J. Pack.

---

# How microcontrollers differ from microprocessors

| Aspect              | Microcontrollers       | Microprocessors         |
|---------------------|------------------------|-------------------------|
| **Functionality**   | Task-specific          | General-purpose        |
| **Components**      | CPU, memory, I/O, timers| Emphasis on CPU        |
| **Complexity**      | Simpler design         | More intricate design  |
| **Cost**            | Cost-effective         | Potentially pricier    |


###### Reference: *Microcontroller Theory and Applications: HC12 and S12* by Daniel J. Pack.

---

# Applications of microcontrollers
## Exploring the Microcontroller Universe
- **Embedded Systems**: Heart of countless devices in our daily lives.
- **Automotive**: Engine control, safety systems, infotainment.
- **Consumer Electronics**: Smartphones, TVs, home appliances.
- **Medical Devices**: Pacemakers, blood glucose monitors, medical imaging.

###### Reference: *Embedded Systems: Real-Time Operating Systems for Arm Cortex M Microcontrollers* by Jonathan Valvano.

---

# Applications of microcontrollers
## Microcontrollers Everywhere
- **Industrial Automation**: PLCs, control systems, robotics.
- **Aerospace**: Avionics, spacecraft control.
- **IoT (Internet of Things)**: Smart devices, environmental monitoring.
- **Entertainment**: Gaming consoles, musical instruments, toys.

###### Reference: *The 8051 Microcontroller and Embedded Systems* by Muhammad Ali Mazidi.

---

# Why STM32?

---

# Brief history and evolution of STM32
## Unveiling the Evolution
- **1987**: SGS-Thomson (now STMicroelectronics) enters the microcontroller market.
- **2007**: Introduction of STM32 series, ARM-based 32-bit microcontrollers.
- **Diverse Offerings**: STM32F, STM32L, STM32H, STM32G families cater to various applications.

###### Reference: STMicroelectronics website - "STM32 32-bit Arm Cortex MCUs."

---

# Brief history and evolution of STM32
## Advancements Over Time
- **2009**: Launch of STM32F2 with advanced peripherals and larger memory.
- **2011**: STM32F4 debuts, bringing more processing power and graphics capabilities.
- **2013**: STM32L0 introduced for ultra-low-power applications.
- **2017**: STM32G0 series launched with a focus on performance and efficiency.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Brief history and evolution of STM32
## Modern Marvels and Future Prospects
- **Today**: STM32 ecosystem flourishes with extensive development tools and support.
- **Focus Areas**: IoT, embedded AI, connectivity, and real-time control.
- **AI Integration**: STM32Cube.AI for integrating machine learning.
- **Future**: Continued innovation in performance, power efficiency, and connectivity.

###### Reference: STMicroelectronics website - "STM32: Unlocking the full potential of IoT."

---

# Popularity and market presence
## Exploring STM32's Popularity
- **Widespread Adoption**: STM32 gained popularity in diverse industries.
- **Engineering Community**: Engineers and hobbyists embrace STM32 for projects.
- **Educational Institutes**: STM32 integrated into electronics curriculum.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Popularity and market presence
## STM32's Impressive Market Presence
- **Global Reach**: STM32 dominates embedded system market share.
- **Versatility**: Used in consumer electronics, automotive, industrial automation, and more.
- **Innovation and Performance**: STM32 evolves to meet industry demands.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Popularity and market presence
## STM32's Role in Connectivity
- **IoT Pioneer**: STM32's low-power capabilities cater to IoT devices.
- **Smart Everything**: STM32 powers smart homes, wearables, industrial IoT, and more.
- **Expanding Ecosystem**: Growing community, resources, and development tools.

###### Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# Series and families within STM32
## Navigating the STM32 Universe
- **Series Classification**: STM32 microcontrollers are categorized into different series.
- **Differentiation Factors**: Each series tailored to specific application domains.
- **Example Families**: STM32F0, STM32F1, STM32L4, and more.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Series and families within STM32
## Diving into STM32F Family
- **STM32F**: Popular series with a wide range of applications.
- **Variants**: STM32F0 for cost-effective solutions, STM32F4 for high-performance.
- **Ecosystem Support**: Rich development tools, libraries, and community resources.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Series and families within STM32
## Spotlight on STM32L Family
- **STM32L**: Focuses on low-power consumption for battery-operated devices.
- **Energy Efficiency**: Ideal for IoT, wearable devices, and portable electronics.
- **Peripherals and Features**: Balancing power savings with performance.

###### Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# Architecture of STM32

---

# Cortex-M series introduction
## Cortex-M Series: A New Era in Microcontrollers
- **Introduction**: ARM Cortex-M series designed for embedded applications.
- **Power and Performance**: Strikes a balance between energy efficiency and processing power.
- **Versatility**: Scalable architecture for various use cases.

###### Reference: *The Definitive Guide to ARM® Cortex®-M0 and Cortex-M0+ Processors* by Joseph Yiu.

---

# Cortex-M series introduction
## Exploring the Cortex-M Family Tree
- **Cortex-M0/M0+**: Ultra-low-power, cost-efficient cores.
- **Cortex-M3**: Offers better performance and broader feature set.
- **Cortex-M4**: Adds DSP extensions for signal processing tasks.
- **Cortex-M7**: Higher performance and advanced features for complex systems.

###### Reference: *The Designer's Guide to the Cortex-M Processor Family* by Trevor Martin.

---

# Cortex-M series introduction
## Why Choose Cortex-M for Your Designs?
- **Standardized Architecture**: Consistency across Cortex-M cores for ease of development.
- **Rich Ecosystem**: Abundant development tools, libraries, and community support.
- **Scalability**: Select the right core for your application's requirements.

###### Reference: *The Definitive Guide to ARM® Cortex®-M3 and Cortex®-M4 Processors* by Joseph Yiu.

---

# Block diagram of a typical STM32 microcontroller
## Navigating the Block Diagram
- **Introduction**: STM32 microcontrollers feature a diverse set of components.
- **Central Processing Unit (CPU)**: Executes instructions and manages operations.
- **Memory**: Stores program code and data temporarily during execution.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Block diagram of a typical STM32 microcontroller
## Components at a Glance
- **Peripherals**: Include I/O ports, timers, communication interfaces.
- **Bus System**: Interconnects components for data and control flow.
- **Clock and Power Management**: Regulate clock frequencies and power modes.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Block diagram of a typical STM32 microcontroller
## Exploring the Architecture
- **Flexibility**: Customize the microcontroller to meet your project's needs.
- **Software Development**: Write code to utilize CPU, memory, and peripherals.
- **Hardware Interfacing**: Connect external devices to I/O ports and communication interfaces.

###### Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# Key components
## GPIO, ADC, Timers, Communication Interfaces
- **GPIO (General-Purpose Input/Output)**: Flexible pins for interfacing with external devices.
- **ADC (Analog-to-Digital Converter)**: Converts analog signals to digital data for processing.
- **Timers**: Generate precise time intervals for various applications.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Key components
## Enabling Connectivity and Control
- **Communication Interfaces**: SPI, I2C, UART facilitate data exchange.
- **SPI (Serial Peripheral Interface)**: High-speed synchronous communication.
- **I2C (Inter-Integrated Circuit)**: Multi-device communication with simple addressing.
- **UART (Universal Asynchronous Receiver-Transmitter)**: Serial communication for point-to-point connections.

Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Key components
## Leveraging STM32's Components
- **GPIO**: Configure pins for input or output, control logic levels.
- **ADC**: Measure real-world analog values like temperature, light intensity.
- **Timers**: Generate accurate time delays, PWM signals for motor control.
- **Communication Interfaces**: Interact with sensors, displays, external devices.

Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# STM32 Development Environment

---

# Introduction to STM32CubeIDE
- **What is STM32CubeIDE**: An integrated development environment by STMicroelectronics.
- **Features**: Combines STM32CubeMX for code configuration with Eclipse-based IDE.
- **Advantages**: Streamlines development, debugging, and code generation.
- **Rich Ecosystem**: Supports various STM32 series, libraries, and middleware.

Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# STM32CubeMX for peripheral initialization
- **What is STM32CubeMX**: A graphical tool for configuring STM32 microcontroller peripherals.
- **Simplified Setup**: Generates initialization code, reducing setup complexity.
- **Time-Saver**: Speeds up the process of configuring pins, clocks, and peripherals.
- **Integration with IDEs**: Seamlessly integrates with STM32CubeIDE for smooth workflow.

Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Debugging tools and options
- **Why Debugging Matters**: Identify and resolve issues in your code.
- **Tools at Your Disposal**: Use breakpoints, watches, and real-time variable tracking.
- **On-Chip Debugging**: Connect microcontroller to debugging interfaces.
- **Integrated Development Environments (IDEs)**: STM32CubeIDE offers robust debugging features.

Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Hardware Abstraction Layer (HAL) vs Low-Level (LL) drivers
- **Hardware Abstraction Layer (HAL)**: Provides high-level, user-friendly APIs.
- **Low-Level (LL) Drivers**: Offer direct access to hardware registers.
- **HAL**: Simplifies coding, supports various peripherals.
- **LL**: Offers fine-grained control, ideal for optimization.

Reference: *Mastering STM32* by Carmine Noviello.

---

# GPIOs and Basic I/O

---

# What is GPIO?
## GPIO: Unveiling the Basics
- **GPIO Definition**: GPIO stands for General-Purpose Input/Output.
- **Versatility**: GPIO pins are like the Swiss Army knives of microcontrollers.
- **Functionality**: Used for both input (sensing) and output (controlling) purposes.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# What is GPIO?
## Understanding GPIO's Role
- **Input Mode**: GPIO pins can read external signals like button presses or sensor data.
- **Output Mode**: GPIO pins can drive external devices like LEDs, motors, or relays.
- **Configurability**: Flexible configuration through software for various applications.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# GPIO configuration
## Unleashing the Versatility
- **Input**: Read external signals, like switches and sensors.
- **Output**: Control external devices, like LEDs and relays.
- **Analog**: Capture analog signals using ADC (Analog-to-Digital Converter).
- **Alternate Functions**: Enable specialized functions, e.g., communication interfaces (UART, SPI, I2C).

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# GPIO configuration
## Practical Application and Beyond
- **GPIO Configuration**: Define pin direction (input or output), pull-up/pull-down resistors, and speed.
- **Analog Mode**: Configure pins for precise analog signal measurement.
- **Alternate Functions**: Customize pins for specific communication protocols or other advanced tasks.
- **Design Flexibility**: GPIOs are the backbone of microcontroller-based projects.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Digital read/write operations
## Understanding the Basics
- **Digital GPIO**: General-Purpose Input/Output pins for digital signals.
- **Read Operation**: Retrieve the logic level (high or low) from a GPIO pin.
- **Write Operation**: Set or clear the logic level on a GPIO pin.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Digital read/write operations
## Utilizing GPIO in Your Projects
- **Input Use Cases**: Reading sensor data, monitoring switches, receiving digital signals.
- **Output Use Cases**: Controlling LEDs, driving relays, triggering external devices.

###### Reference: *Programming with STM32: Getting Started with the Nucleo Board and C/C++* by Donald Norris.

---

# Demonstration with LED blinking
## A Hands-On Introduction to Embedded Programming
- **Why LED Blinking**: A fundamental step in embedded systems.
- **What You Need**: An STM32 microcontroller board, IDE (e.g., STM32CubeIDE).
- **Code Setup**: Initialize GPIO pin, toggle it on/off, control blinking speed.

###### Reference: *Getting Started with STM32: A Hands-On Introduction to RTOS and Embedded Systems* by Ray Yao.

---

# Demonstration with LED blinking
## Witness the LED Blinking Demo
- **Compile and Upload**: Compile your code, upload it to the STM32 board.
- **LED Behavior**: Observe the LED blinking as per your program.
- **Building Block**: Foundation for more complex embedded projects.

###### Reference: *Mastering STM32* by Carmine Noviello.

---

# Other usefull tools

---

# Distributed Version Control System Git and GitHub
## Empowering Collaborative Engineering
- **What is Git?**: A distributed version control system for tracking changes in code.
- **Why Git?**: Tracks changes, enables collaboration, and safeguards code.
- **GitHub**: A web-based platform for hosting and sharing Git repositories.

###### Reference: *Pro Git* by Scott Chacon and Ben Straub.

---

# Distributed Version Control System Git and GitHub
## Key Concepts and Benefits
- **Repositories**: Store and manage your project's code.
- **Branches**: Isolate work, experiment, and collaborate.
- **Pull Requests**: Facilitate code review and collaboration.
- **Version Control**: Rollback to previous states and resolve conflicts.

###### Reference: *GitHub For Dummies* by Sarah Guthals, Phil Haack, and Lee Naylor.

---

# Basic concepts of Git
## Navigating the World of Version Control
- **Repository (Repo)**: A project's folder that Git is managing.
- **Commit**: A snapshot of the repository's current state.

###### Reference: *Pro Git* by Scott Chacon and Ben Straub.

---

# Basic concepts of Git
## Understanding the Building Blocks
- **Branches**: Independent lines of development within a repository.
- **Merge**: Combining different branches or histories.
- **Clone**: Copying a remote repository to your local machine.
- **Push and Pull**: Sending and receiving changes from a remote repository.

###### Reference: *Version Control with Git* by Jon Loeliger and Matthew McCullough.

---

# Folder tree of a repository
## Understanding the Folder Tree
- **Repository**: A container for your project files and history.
- **Top-Level Directory**: The root folder of your repository.
- **Subdirectories**: Organize files logically within the repository.
- **Files**: Individual components, scripts, documents, and more.

###### Reference: *Pro Git* by Scott Chacon and Ben Straub.

---

# Folder tree of a repository
## Structuring Your Project
- **Clarity**: Organize files and folders for readability.
- **Common Practices**: Separate source code, documentation, assets.
- **Version Control**: Every file and folder is tracked.
- **Collaboration**: A well-structured repository aids teamwork.

###### Reference: *GitHub For Dummies* by Sarah Guthals, Phil Haack, and Lee Naylor.

---

# **Lecture B**:
# GPIOs and Basic I/O

---

# Introduction to GPIOs

---

# Definition and role of GPIOs in microcontrollers
## Understanding Their Significance
- **What Are GPIOs?**: GPIOs are pins on a microcontroller that can be configured as input or output.
- **Versatility**: They provide a bridge for microcontrollers to interact with the external world.
- **Key Roles**: Used for reading sensors, driving LEDs, and more.

###### Reference: *Embedded Systems: Introduction to Arm® Cortex™-M Microcontrollers* by Jonathan W. Valvano.

---

# Definition and role of GPIOs in microcontrollers
## Their Vital Role in Microcontroller Projects
- **Flexibility**: GPIOs are like the "fingers" of microcontrollers, allowing them to touch the physical world.
- **Foundation**: GPIOs are fundamental to many embedded systems projects.

###### Reference: *The 8051 Microcontroller and Embedded Systems* by Muhammad Ali Mazidi.

---

# Differentiating GPIOs from specialized pins
## Unraveling the Differences
- **GPIO (General-Purpose Input/Output)**: Versatile pins for user-defined functions.
- **Specialized Pins**: Designed for specific purposes like UART, SPI, I2C.
- **GPIO Flexibility**: Can be configured as inputs or outputs as needed.

###### Reference: *Microcontroller Theory and Applications: HC12 and S12* by Daniel J. Pack.

---

# Differentiating GPIOs from specialized pins
## Leveraging Pin Types
- **GPIO**: Use for custom logic, sensing, control, or interfacing.
- **Specialized Pins**: Designed for communication and specific protocols.
- **Choosing Wisely**: Select pins based on your project requirements.

###### Reference: *Embedded Systems: Introduction to Arm® Cortex™-M Microcontrollers* by Jonathan W. Valvano.

---
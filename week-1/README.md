# Week 1

## Lecture A (Tuesday)
1. **Introduction to Embedded Systems (10 minutes)**
    - What is an embedded system?
    - Characteristics of embedded systems
    - Examples in daily life
    - Differences between embedded systems and general-purpose computers

2. **Overview of Microcontrollers (20 minutes)**
    - What is a microcontroller?
    - Key components: CPU, memory, I/O
    - How microcontrollers differ from microprocessors
    - Applications of microcontrollers

3. **Why STM32? (20 minutes)**
    - Brief history and evolution of STM32
    - Popularity and market presence
    - Series and families within STM32 (e.g., STM32F0, STM32F1...)

4. **Architecture of STM32 (20 minutes)**
    - Cortex-M series introduction
    - Block diagram of a typical STM32 microcontroller
    - Key components: GPIO, ADC, Timers, Communication Interfaces (SPI, I2C, UART)

5. **STM32 Development Environment (40 minutes)**
    - Introduction to STM32CubeIDE
    - STM32CubeMX for peripheral initialization
    - Debugging tools and options
    - Hardware Abstraction Layer (HAL) vs Low-Level (LL) drivers

6. **GPIOs and Basic I/O (40 minutes)**
    - What is GPIO?
    - GPIO configuration (Input, Output, Analog, and Alternate functions)
    - Digital read/write operations
    - [Demonstration with LED blinking](./exercises/exercise_1_blinky.md)
    
7. **Other usefull tools (30 minutes)**
    - Distributed Version Control System Git and GitHub
    - Basic concepts of Git
    - Folder tree of a repository

## Lecture B (Thursday) - GPIOs and Basic I/O

1. **Introduction to GPIOs (20 minutes)**
    - Definition and role of GPIOs in microcontrollers
    - Differentiating GPIOs from specialized pins
    - A glimpse into STM32's GPIO architecture

2. **Detailed GPIO Configuration (1 hour)**
    - Modes of operation:
      - Input mode: When a GPIO is used to read the state of a pin (e.g., to check if a button is pressed)
      - Output mode: When a GPIO is used to set the state of a pin (e.g., to light up an LED)
      - Analog mode: When a GPIO is set to interface with analog peripherals
      - Alternate function: When the pin is utilized for a specialized purpose (e.g., SPI or UART communication)
    - GPIO settings:
      - Pull-up and Pull-down resistors: Why they're needed and how to use them
      - Output type: Push-pull vs. Open-drain
      - Output speed: Importance and when to adjust

3. **Digital Read/Write Operations (40 minutes)**
      - Reading a digital state: Checking if a button is pressed/not pressed
      - Setting a digital state: Turning on/off an LED
      - Monitoring state changes: Polling vs interrupts
      - Introduction to debouncing (relevant when reading switches or buttons)
        
4. **Practical Exercises (1 hour)**
      - Hands-on: Setting up STM32CubeIDE and creating a new project
      - Coding exercise: LED Blinking
      - Coding exercise: Button as an input to control the LED

5. **Potential Pitfalls and Troubleshooting (20 minutes)**
      - Common mistakes when setting up GPIOs
      - Introduction to tools like the logic analyzer or oscilloscope for troubleshooting

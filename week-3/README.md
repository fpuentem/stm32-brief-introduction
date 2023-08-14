# Week 3

## Lecture A (Tuesday) - ADC and Analog Interfacing
**1. Understanding Analog and Digital Domains (20 minutes)**
- What is analog data? Natural continuous signals.
- What is digital data? Discrete values.
- Why the need for conversion between analog and digital?

**2. ADC (Analog to Digital Converter) In-Depth (40 minutes)**
- **Basic Principle of ADC (10 minutes)**
  - Continuous analog signals to discrete digital values
  - Concept of resolution and quantization: bit depth (e.g., 8-bit, 10-bit, 12-bit ADCs)
- **ADC Architectures (10 minutes)**
  - Successive Approximation Register (SAR) ADC
  - Sigma-Delta ADC
  - Flash ADC (Parallel ADC)
  - Dual Slope ADC
- **Key Specifications of ADCs (10 minutes)**
  - Resolution and accuracy
  - Sampling rate & Nyquist theorem
  - Input impedance and its importance
  - Reference voltage
- **ADC in STM32 Microcontrollers (10 minutes)**
  - Features: multi-channel, DMA support, differential input mode, etc.
  - Configuration aspects: STM32 ADC resolution, clock prescaler, scan mode, etc.

**3. Analog Interfacing with Sensors (30 minutes)**
- **Types of Analog Sensors (10 minutes)**
  - Examples: Temperature sensors (e.g., LM35), Light sensors (LDR), Pressure sensors
  - How these sensors produce analog voltage based on environmental changes
- **Interfacing Techniques (10 minutes)**
  - Proper grounding
  - Shielding of analog signals
  - Use of operational amplifiers for signal conditioning
- **Challenges in Analog Interfacing (10 minutes)**
  - Noise and interference
  - Cable length issues
  - ADC errors: Quantization error, aliasing

**4. Hands-on Exercise: Analog Sensor Reading with STM32 (1 hour 20 minutes)**
- **Setting Up the Environment (20 minutes)**
  - Connecting a simple potentiometer or any other analog sensor to the STM32 board
  - Configuring ADC pins using STM32CubeIDE
  - Setting up ADC parameters: channel selection, resolution, sampling time
- **Writing the ADC Code (20 minutes)**
  - Initializing the ADC and starting an ADC conversion
  - Reading the ADC value and converting it to a meaningful measurement
- **Displaying the Sensor Reading (20 minutes)**
  - Optionally, you can interface with an LCD or send data to a PC terminal via UART to display sensor readings
- **Troubleshooting Common Issues (20 minutes)**
  - Debugging ADC conversions, dealing with noisy readings, understanding ADC errors and inaccuracies

**5. Advanced Features and Beyond (20 minutes)**
- **STM32's Dual and Triple ADC modes**
- **ADC with DMA**: Efficiently reading ADC values without CPU intervention
- **Calibration of ADC**: Ensuring accurate readings
- **Over-sampling and Resolution Enhancement**: Improving ADC results beyond hardware limitations

## Lecture B - Part 1  (Thrusday) - Development Kits and Boards (1.5 hours)

**1. The Landscape of STM32 Development Kits (15 minutes)**
- Historical context: How development boards evolved
- Why STM32 and its popularity in the industry

**2. Introduction to STM32 Development Boards (20 minutes)**
- **Nucleo Boards**
  - Features: mbed-enabled, Arduino headers, on-board debugger
  - Different families: Nucleo-32, Nucleo-64, and Nucleo-144
- **Discovery Boards**
  - Features: Rich peripherals, demos for onboard sensors/actuators, and comprehensive development ecosystem
  - Specialty boards, e.g., with graphical displays, audio capabilities

**3. Features and Connectivity Options (30 minutes)**
- **Onboard Features**
  - Debugging capabilities: ST-LINK/V2 debugger & programmer
  - GPIOs, ADCs, UART, SPI, I2C headers
- **Expandability**
  - Arduino-compatible headers: Why they matter and how they make prototyping easier
  - ST morpho headers
- **Demonstration (if possible): Setting up a development board for the first time**

**4. Importance of Development Kits for Learning and Prototyping (20 minutes)**
- Accelerated learning: Immediate hands-on experience
- Rapid prototyping: Quick transition from idea to a working model
- Ecosystem and community support

**5. Use Cases (15 minutes)**
- Real-world applications built using Nucleo and Discovery boards
- Importance in industry R&D and academia

## Lecture B - Part 2  (Thrusday) - Best Practices and Tips (1.5 hours)

**1. Importance of Reading Datasheets and Reference Manuals (20 minutes)**
- Differentiating between datasheets and reference manuals
- Key sections in these documents: Pinouts, electrical characteristics, peripheral details, memory layout
- Case study: Extracting vital information from a datasheet for a project

**2. Tips for Efficient Coding on STM32 Platforms (30 minutes)**
- Using STM32CubeIDE and HAL (Hardware Abstraction Layer) library
- Code organization and modular design
- Memory considerations: Stack, Heap, and optimal data storage
- Power management and energy-efficient coding

**3. Common Pitfalls and Challenges (30 minutes)**
- Common errors with STM32 development: Clock configuration, incorrect pin initialization
- Debugging techniques: Using the onboard debugger, print-based debugging, logic analyzers, oscilloscopes
- Dealing with noise, especially in ADC readings and analog interfaces
- Interrupt priorities and related issues

**4. Transitioning to Real-Time OS for Embedded Systems (30 minutes)**
- What is a Real-Time Operating System (RTOS)?
- Why consider an RTOS? (Deterministic behavior, multitasking)
- Introduction to FreeRTOS on STM32: Tasks, Queues, Semaphores
- How previous topics lay the foundation for RTOS: 
  - **Hardware Understanding**: Knowing your board and its capabilities (from Development Kits and Boards)
  - **Interfacing**: Efficient communication with peripherals (from ADC and Communication Protocols)
  - **Coding Practices**: Writing efficient and modular code (from Best Practices and Tips)

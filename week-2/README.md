# Week 2

## Lecture A (Tuesday) - Interrupts and Event Handling 
  1. **Introduction to Interrupts (20 minutes)**
     - Definition and basic concept: Why polling isn’t always efficient
     - The importance of interrupts in real-time systems
     - How interrupts can make a system more responsive
       
  2. **Types of Interrupts and their Applications (1 hour)**
     - External interrupts: Triggered by external events like a button press
     - Timer-based interrupts: Triggered after a set duration
     - Peripheral events: Triggered by internal peripherals (like when data is ready to be read from a UART module)
     - System exceptions: Reset, NMI, Hard fault, etc.
       
  3. **Nested Vectored Interrupt Controller (NVIC) in STM32 (40 minutes)**
     - Role of NVIC in handling multiple interrupts
     - Setting interrupt priorities
     - Enabling and disabling interrupts
     - Understanding and handling interrupt latency
       
  4. **Practical Exercises (1 hour)**
     - Hands-on: Setting up interrupts using STM32CubeMX and STM32CubeIDE
     - Coding exercise: Using an external interrupt to detect a button press
     - Advanced exercise: Combining timer interrupt with GPIO to create a PWM signal for LED brightness control

  5. **Debouncing in Interrupts (20 minutes)**
      - Why simple button presses aren't always simple
      - Software-based debouncing techniques
      - Introduction to hardware-based debouncing
        
  6. **Potential Pitfalls and Troubleshooting (20 minutes)**
      - Common mistakes when setting up interrupts
      - Debugging interrupt-related issues
      - Using the debugger's features to track interrupt behaviors
        
## Lecture B (Thursday) - Communication Protocols
  1. **Introduction to Communication in Embedded Systems (15 minutes)**
     - Why do devices need to communicate?
     - Types of communication: Serial vs Parallel
     - Importance of standardized communication protocols
       
  2. **UART (Universal Asynchronous Receiver-Transmitter) (1 hour 15 minutes)**
     - *UART's Role in Embedded Systems (15 minutes)*
       - When and why to use UART
       - Typical use-cases: Debugging, data transfer to PC, communication with other     microcontrollers
     - *Setting Up UART Communication on STM32 (15 minutes)*
       - STM32's USART/UART modules introduction
       - Configuration parameters: Baud rate, Flow control, Mode selection
     - *Hands-on Exercise: UART Communication (20 minutes)*
       - Setting up UART on STM32 using STM32CubeIDE
       - Simple UART echo program: Send and receive data
     - *Potential Pitfalls and Troubleshooting (10 minutes)* 
       - Common UART communication issues: Baud rate mismatch, noise, framing errors
       - Using tools like logic analyzers to diagnose UART problems
    
  3. **I2C (Inter-Integrated Circuit) (1 hour 15 minutes)**
     - *Basic Concept and Architecture (15 minutes)*
       - Serial communication, Master/Slave model
       - Components: SDA (Serial Data Line), SCL (Serial Clock Line), Acknowledgement, Addresses
     - *I2C's Role in Embedded Systems (15 minutes)*
       - When and why to use I2C
       - Typical use-cases: Sensor interfacing, EEPROM data storage, peripheral expansions
     - *Setting Up I2C Communication on STM32 (15 minutes)*
       - STM32's I2C modules introduction
       - Configuration parameters: Clock speed (Standard mode, Fast mode, Fast mode plus), addressing mode (7-bit vs. 10-bit)
     - *Hands-on Exercise: I2C Communication (20 minutes)*
       - Setting up I2C on STM32 using STM32CubeIDE
       - Simple I2C communication: Read temperature data from an I2C sensor
     - *Potential Pitfalls and Troubleshooting (10 minutes)*
       - Common I2C issues: Bus contention, missing pull-up resistors, clock stretching
       - Using oscilloscopes or logic analyzers to visualize and debug I2C communication
  4. **SPI vs I2C vs UART (15 minutes)**
     - A quick comparative review to understand the different scenarios where each protocol shines
     - Speed, mode of communication, bus complexity, use-cases

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
        
## Lecture B (Thursday)

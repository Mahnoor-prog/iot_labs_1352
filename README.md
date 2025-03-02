LAb3 Task Questions

Task 2: Running the Code Without Interrupt
Observations and Comparison
When running the lab functionality without interrupts, the following issues may arise:

Polling Waste CPU Resources – The microcontroller continuously checks for events (e.g., button press), which consumes processing power.
Slower Response Time – The system may respond with a delay since it checks conditions at regular intervals instead of reacting immediately.
Inefficient Power Consumption – The CPU remains active, even when unnecessary, leading to increased energy use.
Before Using Interrupts – The microcontroller keeps looping and checking for inputs.
After Using Interrupts – The microcontroller only responds when an event occurs, improving efficiency.


Task 3: Understanding the Debounce Issue
1. What is a debounce issue, and why do we get rid of it?
A debounce issue occurs when a button or switch is pressed, and instead of registering a single press, multiple signals are detected due to mechanical vibrations. This can lead to unintended multiple activations of a function.

We eliminate debounce issues to ensure:

Reliable and accurate button presses.
Preventing multiple triggers from a single press.
Avoiding unintended operations in IoT systems.

2. In which applications/domains can debounce issues be threatening if unresolved?
Debounce issues can cause major problems in:

IoT-based Smart Home Systems – Multiple triggers can lead to incorrect device operations.
Industrial Automation – False sensor readings can disrupt production lines.
Medical Devices – Inaccurate button presses can lead to critical failures in devices like pacemakers.
Keyboards & Input Devices – Multiple key registrations cause unwanted behavior in user inputs.
Robotics & Embedded Systems – Motors and actuators may receive wrong signals, leading to mechanical failures.

3. Why does debounce occur? Is it a compiler error, logical error, or a cheap microcontroller?
Debounce occurs due to mechanical limitations of buttons/switches, not due to compiler or logical errors.

However, the possible reasons include:

Mechanical Design Issue – Physical button vibrations create multiple signals.
Software Processing Issue – If software does not handle input filtering, it will register multiple signals.
Cheap Microcontroller – Some low-cost microcontrollers may lack hardware debounce features, requiring software-based solutions.

Task 4: Why Do We Use Interrupts?
1. Why do we use interrupts?
Interrupts are used in IoT to efficiently handle real-time events without constant CPU polling.

Benefits of using interrupts:

Efficient Processing – The microcontroller does not need to keep checking for events.
Faster Response Time – Reacts instantly to events like button presses or sensor triggers.
Power Saving – The microcontroller can enter a low-power mode and wake up only when needed.
Multitasking – Allows the system to perform multiple tasks simultaneously without waiting for an event.
2. How does an interrupt lower the processing cost of a microcontroller?
Interrupts reduce CPU usage and power consumption by:

Eliminating the need for polling, where the processor constantly checks for input changes.
Allowing the microcontroller to execute other tasks until an event occurs.
Entering sleep mode and waking up only when necessary.
Example:
A temperature sensor in an IoT system can trigger an interrupt when the temperature exceeds a threshold instead of continuously checking the temperature.

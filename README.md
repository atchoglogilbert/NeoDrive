# NeoDrive
Advanced embedded system &amp; C development project with features such as a RTOS, sensor fusion, control algorithms and V2V communication.

## Subject file
https://docs.google.com/document/d/1eehwzec5uO5huPw9I_m6vhSdpnuiUYqCmYa_DYuJEUI/edit?usp=sharing

## Certs
Differential Equations -> Control Systems -> Arduino -> RTOS

1. **Ordinary Differential Equations (ODEs)**:
   - **First-order ODEs**: Equations involving only first derivatives of the unknown function.
   - **Higher-order ODEs**: Equations involving derivatives of order higher than one.

2. **Partial Differential Equations (PDEs)**:
   - Equations involving partial derivatives of multivariable functions.
   - Types of PDEs include: 
     - **Elliptic PDEs**: e.g., Laplace's equation.
     - **Parabolic PDEs**: e.g., Heat equation.
     - **Hyperbolic PDEs**: e.g., Wave equation.

3. **Linear Differential Equations**:
   - Equations where the dependent variable and its derivatives appear linearly.

4. **Nonlinear Differential Equations**:
   - Equations where the dependent variable or its derivatives appear nonlinearly.

5. **Exact and Inexact Differential Equations**:
   - **Exact**: Equations where an integrating factor can be found to make them exact differentials.
   - **Inexact**: Equations that are not exact and typically require other methods for solution.

6. **Initial Value Problems (IVPs)**:
   - Differential equations with prescribed initial conditions.

7. **Boundary Value Problems (BVPs)**:
   - Differential equations with prescribed boundary conditions.

8. **Systems of Differential Equations**:
   - Sets of equations where there are multiple unknown functions and their derivatives.

9. **Analytical Methods**:
   - Techniques like separation of variables, integrating factors, series solutions, and transformation methods (e.g., Laplace transforms).

10. **Numerical Methods**:
    - Techniques for approximating solutions to differential equations numerically, such as Euler's method, Runge-Kutta methods, finite difference methods, and finite element methods.

11. **Applications**:
    - Differential equations are widely used in physics, engineering, biology, economics, and many other fields to model real-world phenomena.

12. **Existence and Uniqueness of Solutions**:
    - Theory regarding when solutions to differential equations exist and whether they are unique.


1. RTOS Design and Architecture:
Task Scheduler:
Define Task Structures: Design a structure to hold information about tasks such as task ID, priority, state, stack pointer, etc.
Scheduler Algorithm: Choose a preemptive scheduling algorithm (e.g., Priority-based preemptive scheduling) and implement it. This involves deciding how tasks will be scheduled based on their priorities and ensuring that higher priority tasks preempt lower priority tasks when necessary.
Context Switching: Implement context switching routines to save and restore task contexts during scheduling.
2. Task Management:
Task Creation and Destruction:

Develop functions to create and delete tasks dynamically.
Allocate and manage task stacks.
Task Synchronization:

Implement mechanisms like semaphores, mutexes, and message queues for task synchronization and inter-task communication.
Ensure these mechanisms handle mutual exclusion and synchronization correctly to prevent race conditions.
3. Interrupt Handling:
Interrupt Management:
Develop interrupt service routines (ISRs) for handling hardware interrupts.
Implement interrupt prioritization and management to handle time-sensitive operations and external events effectively.
Design mechanisms to safely synchronize interrupt-driven data with tasks.
4. RTOS Kernel Initialization:
System Initialization:
Set up the system timer for task scheduling and timing operations.
Initialize memory allocation and management routines.
Configure interrupt vector table and enable necessary interrupts.
5. Testing and Debugging:
Unit Testing:

Develop unit tests to validate each component of the RTOS (e.g., scheduler, synchronization mechanisms).
Use simulation tools if available to test RTOS behavior in controlled environments before deploying on hardware.
Debugging:

Use debugging tools (e.g., printf debugging, simulator debuggers) to trace and debug issues related to task scheduling, synchronization, and interrupt handling.
6. Integration with Autonomous Vehicle System:
Integrate RTOS with Application:
Adapt the RTOS to manage tasks related to sensor data acquisition, control algorithms, actuator control, and communication within the autonomous vehicle system.
Ensure RTOS tasks meet real-time constraints and deadlines required by the application.
Tools Needed:
Development Environment: Arduino IDE or PlatformIO for Arduino board programming.
Simulation Tools: Depending on availability, use simulation environments or plugins to test RTOS functionality before deployment.
Debugging Tools: Serial Monitor, debugger tools (if using hardware debuggers), and printf statements for debugging RTOS components.
Example Tool Chain:
RTOS Development: Custom RTOS developed in C/C++ based on project specifications.
Development Environment: Arduino IDE or PlatformIO.
Debugging: Serial Monitor for basic debugging; hardware debuggers (if available) for more complex issues.
Testing: Unit testing frameworks compatible with Arduino (e.g., Unity for Arduino).

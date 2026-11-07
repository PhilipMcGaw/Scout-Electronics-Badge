# H-bridge motor drivers

## Working title

How an H-bridge reverses a brushed DC motor

## Audience and scope

Adult-facing introductory article about the operating idea and design risks of a four-switch H-bridge for a brushed DC motor. Keep it conceptual until a specific circuit, motor and driver have been selected and checked. This is not a high-current construction guide and is outside the Scouts booklet's practical scope.

## Draft

### Why use an H-bridge?

A brushed DC motor turns one way when current flows through it in one direction. Reverse the current and the motor turns the other way. An H-bridge uses four controlled switches around the motor to select the direction of current while using one DC supply.

The name comes from the usual diagram: the four switches form the sides of an H and the motor sits across its middle. To drive the motor in one direction, switch on one diagonal pair. To reverse it, switch on the other diagonal pair. A motor-driver IC or module packages much of the switching and protection needed to do this safely.

### Why the switches need careful control

The two switches in either vertical leg must not conduct at the same time. If the upper and lower switch overlap, they connect the supply directly to ground. This is called shoot-through and can destroy the switches or driver very quickly. A properly designed driver prevents overlap, often by inserting a short dead time between switching one device off and the other on.

A motor is an inductive load. Its current cannot stop instantly when a switch changes state. The bridge must provide a safe path for that current to continue and decay. Driver designs use the MOSFET body diodes or controlled switching paths for this recirculation. The chosen current path affects braking, coasting, heating and electrical noise.

### Speed control with PWM

Pulse-width modulation (PWM) switches the motor supply rapidly on and off. Changing the proportion of each cycle spent on changes the motor’s average applied voltage and usually changes its speed under a particular load. Speed is not simply a fixed percentage of duty cycle: motor current, torque, supply voltage, load and the driver’s current path all matter.

### Choosing a driver

Start with the motor’s rated voltage and its stall current, not only its no-load running current. Check the driver’s continuous and peak current limits under the intended board and cooling conditions. Also check its supply range, switching method, current limiting, thermal shutdown, and how it handles inductive current when the motor is turned off or reversed.

For discrete MOSFET bridges, the gate drive needs particular attention. A high-side N-channel MOSFET usually needs a gate voltage above its source; a gate driver or charge-pump arrangement may be required. P-channel devices can simplify the high-side drive at low voltages, but their on-resistance and heat loss still need checking. In either case, verify gate-to-source voltage limits, on-resistance at the actual drive voltage, switching timing and device temperature from the datasheets.

Do not reverse the motor instantly while it is still turning unless the driver and control system are designed for that operation. The motor’s stored energy and current can create high stress. Use the driver manufacturer’s truth table and current-recirculation guidance, add suitable supply decoupling, and test within the limits of the selected motor and driver.

For a first project, a suitable integrated motor-driver module is generally a more manageable learning platform than a hand-built high-current bridge. Choose one using the exact motor’s data and the module manufacturer’s specifications; a headline current rating alone is not enough.

## Editorial and source notes

- Circuit Digest, [“Simple H Bridge Motor Driver Circuit using MOSFET”](https://circuitdigest.com/electronic-circuits/simple-h-bridge-motor-driver-circuit-using-mosfet), published 2019-05-06. Useful for the basic diagonal-switching concept. Do not reuse its schematic or build claims without independent review and rights checks.
- Texas Instruments, [SLVA321A, “Current Recirculation and Decay Modes”](https://www.ti.com/lit/pdf/SLVA321), revised 2021-04. Supports explaining inductive current paths and why the bridge must safely manage motor current during switching.
- Texas Instruments, [DRV8411A data sheet](https://www.ti.com/lit/ds/symlink/drv8411a.pdf), provides an example of integrated H-bridge current paths and automatic dead time. It is an example device, not a recommendation for an unselected motor.
- The Circuit Digest page's broad 20 A/40 V construction claim and its PWM/efficiency generalisations are not adopted. Its discussion contains potentially confusing statements about switch states and should not be used as a build-ready design.
- A specific low-voltage demonstrator, motor, driver and wiring diagram need datasheet review before any construction steps are added.

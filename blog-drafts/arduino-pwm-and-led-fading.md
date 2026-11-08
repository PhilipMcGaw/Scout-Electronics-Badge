# Fading an LED with Arduino PWM

The Arduino `analogWrite()` function can make an LED appear brighter or dimmer. Despite its name, it does not produce a smoothly adjustable analogue voltage on most boards. It switches a digital output on and off rapidly. The fraction of each cycle that the output is on is called the **duty cycle**.

At a low duty cycle, the LED receives short on-pulses with longer off periods, so it appears dim. At a high duty cycle, it stays on for more of each cycle and appears brighter. The switching happens quickly enough that the eye sees a steady change in brightness. This technique is called pulse-width modulation, or **PWM**.

## A simple fade

The core of a fade sketch is to change the PWM value over time: `analogWrite(pwmPin, value)`. On some familiar boards, the value ranges from 0 to 255, where 0 means always off and 255 means always on. The resolution and available PWM pins depend on the board and its software core, so check the exact board’s documentation. A pin marked with `~` often indicates PWM support, but the pinout is the final reference.

Use an LED with a current-limiting resistor in series, as you would in a basic LED circuit. PWM controls the proportion of time the pin is high; it does not remove the need to limit LED current. Also, apparent brightness does not necessarily change in a perfectly even way as the code value changes.

## PWM is not a power supply

PWM is useful for controlling the brightness of an LED and, with suitable driver hardware, the average power delivered to some loads. It is not a substitute for checking a component’s voltage and current requirements. Do not connect a motor directly to a microcontroller output pin. Motors can draw more current than a pin can safely provide and can create voltage spikes; use a suitable driver and follow its documentation.

The Arduino documentation describes `analogWrite()` as PWM on supported pins. Its [Fading example](https://docs.arduino.cc/built-in-examples/analog/Fading/) shows the LED circuit and a basic fade, while the [PWM guide](https://docs.arduino.cc/tutorials/generic/secrets-of-arduino-pwm/) explains the switched waveform. Treat example pin numbers and output ranges as board-specific.

## Further reading

- Link to the [resistor article](resistors.md) for choosing a current-limiting resistor.
- Check the exact board’s pinout and output limits, and the LED or driver datasheet, before building a circuit.
- Iain Sharp, [Electronics for Artists, Part 2](https://lushprojects.com/electronicsforartists/electronicsforartistsp2.pdf) (revision 2.2, 2019), introduces PWM using a classic Uno. Its 0–255 values and pin examples are board/software-specific. Treat “average voltage” as a simplified description: the pin produces a switched waveform, and the effect depends on the load or filtering. The notes are CC BY-NC-SA 3.0 Unported; do not copy the diagrams or code without meeting the licence terms.

*This article draws on the PWM and LED-fade lessons in the supplied DFRobot beginner tutorial but does not reuse its diagrams or code. Check the selected board and parts before publication.*

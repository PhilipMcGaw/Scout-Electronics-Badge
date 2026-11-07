# Arduino buttons: reading a reliable digital input

A pushbutton looks simple: press it, and an Arduino should notice. The key is to make sure the input pin has a defined voltage when the button is open. If the pin is left unconnected, it can pick up electrical noise and read unpredictably. This is called a **floating input**.

## Give the input a default state

A pull-up or pull-down resistor gently connects the input to a known voltage when the button is not pressed. A pull-up connects it towards the board’s logic supply; a pull-down connects it towards ground. When the button is pressed, the circuit changes the pin to the opposite state.

Many Arduino boards provide an internal pull-up resistor that can be enabled in software with `INPUT_PULLUP`. For a compatible board, connect a momentary button between a digital input pin and GND, then set that pin to `INPUT_PULLUP`. The input reads `HIGH` while the button is open and `LOW` when pressed. This is called **active-low** logic: the action is represented by a low signal. Check the board documentation before relying on an internal pull-up, because Arduino boards do not all use the same microcontroller or electrical limits.

```cpp
const byte buttonPin = 2;
const byte ledPin = LED_BUILTIN;

void setup() {
  pinMode(buttonPin, INPUT_PULLUP);
  pinMode(ledPin, OUTPUT);
}

void loop() {
  const bool pressed = (digitalRead(buttonPin) == LOW);
  digitalWrite(ledPin, pressed ? HIGH : LOW);
}
```

This sketch turns the built-in LED on while the button is pressed. It assumes the selected board has a built-in LED and supports `INPUT_PULLUP`; use its board page and pinout to confirm. A different circuit, such as one with an external pull-down resistor, gives the opposite readings, so adapt the condition to match the wiring.

## One press can look like several

The contacts inside a mechanical button can briefly open and close several times as the button is pressed. A program that counts every transition may interpret one press as several. This is called **switch bounce**. If a button simply holds an LED on while pressed, the quick transitions are usually not important. If the program reacts once per press, add a debounce method and test it with the actual switch.

## Check the board’s limits

Keep input voltages within the limits for the exact board. Do not connect a pin to a voltage above its supply rail or below ground. A microcontroller input is for sensing a signal; it is not a power output for motors, lamps, or other loads. Check the board and component documentation before connecting a circuit.

## Further reading

- Arduino’s [INPUT, INPUT_PULLUP and OUTPUT reference](https://docs.arduino.cc/language-reference/en/variables/constants/inputOutputPullup/) explains floating inputs and pull-up behaviour.
- Arduino’s [button wiring example](https://docs.arduino.cc/built-in-examples/digital/InputPullupSerial/) and [pushbutton debounce example](https://docs.arduino.cc/built-in-examples/digital/Debounce/) show related circuits and code.

*This article uses the supplied DFRobot beginner tutorial as background, then rewrites the explanation for current Arduino documentation. Confirm the target board before publishing pin-specific instructions.*

# Arduino Mega — First External LED

My first physical computing project using an Arduino Mega 2560.

## Goal

Control an external LED using a digital output pin.

## Hardware

- Arduino Mega 2560
- Red LED
- 330Ω resistor
- Breadboard
- Jumper wires

## Circuit

Pin 9 → 330Ω resistor → LED → GND

## Code

```cpp
void setup() {
  pinMode(9, OUTPUT);
}

void loop() {
  digitalWrite(9, HIGH);
  delay(1000);
  digitalWrite(9, LOW);
  delay(1000);
}


# Arduino Mega — First External LED 10.8.26
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

## Goal
Using an LED and Arduino mega control board to control the LED with the digital output pin. 

## Workflow Pathway
Arduino pin 9 --> Yellow Jumper --> 330 Ohm resistor --> Red LED --> Black wire --> Adruino GND

## Breadboard Positions
-Yellow → 40d → Mega pin 9
-Resistor → 40e–40f
-LED long leg → 40g
-LED short leg → 41g
-Black → 41h → Mega GND

## Results
Red LED started to work; ~1 second per blink when digital pin 9 is being controlled. 

## Troubleshoot
I didn't properly seat the jumpers, resistor, and LED into the breadboard. I tested and isolated the wiring, LED, resistor, power connections and breadboard, took me hours but did not give up.

## What I Learned
-How to identify LED anode and cathode
-How to use a resistor to limit LED current
-How to use an Arduino digital output
-How to connect an LED to an Arduino GND pin
-How breadboard connections work
-The importance of checking physical connections when debugging
  hardware

## Lesson
CHECK PHYSICAL CONNECTIONS!!

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


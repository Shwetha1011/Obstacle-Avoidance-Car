# Obstacle Avoidance Car

This project involves an Arduino-based obstacle avoidance car that uses an ultrasonic sensor to navigate and avoid obstacles. The car can be controlled via Bluetooth with various commands.

## Features

- **Obstacle Detection:** Utilizes an ultrasonic sensor to detect obstacles and respond accordingly.
- **Bluetooth Control:** Allows remote control via Bluetooth with commands to move the car in different directions.
- **Motor Control:** Manages motor direction and speed for movement and stopping.

## Components

- Arduino (e.g., Arduino Uno)
- Ultrasonic Sensor (HC-SR04)
- Bluetooth Module (e.g., HC-05 or HC-06)
- DC Motors (4 motors for differential drive)
- Motor Driver (e.g., L298N)
- Servo Motor (optional)

## Wiring

- **Ultrasonic Sensor:**
  - `Trig` pin -> Arduino `pin 12`
  - `Echo` pin -> Arduino `pin 13`
- **Bluetooth Module:**
  - `TX` pin -> Arduino `RX` pin (e.g., `pin 0`)
  - `RX` pin -> Arduino `TX` pin (e.g., `pin 1`)
- **Motors:**
  - Right Motor 1 -> Arduino `pin 5`
  - Right Motor 2 -> Arduino `pin 4`
  - Left Motor 1 -> Arduino `pin 6`
  - Left Motor 2 -> Arduino `pin 7`
  - Left Motor Enable -> Arduino `pin 3`
  - Right Motor Enable -> Arduino `pin 9`

## How to Use

1. **Upload the Code:** Upload the Arduino code to your Arduino board using the Arduino IDE.
2. **Power the Car:** Connect the power supply and ensure all components are properly connected.
3. **Bluetooth Connection:** Pair the Bluetooth module with a compatible device (e.g., smartphone) and use a Bluetooth terminal app to send commands.
4. **Control Commands:** 
   - `b`: Move backward
   - `f`: Move forward
   - `r`: Turn right
   - `l`: Turn left
   - `h`: Hold (stop)

## Troubleshooting

- **Bluetooth Issues:** Verify the Bluetooth module is properly paired and connected.
- **Sensor Calibration:** Check the ultrasonic sensor wiring and calibration if obstacle detection is inaccurate.


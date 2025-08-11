

This project is a mobile robot controlled by an **Arduino Uno** and **two L293D motor driver ICs**.  
It operates autonomously, performing predefined movement patterns while avoiding obstacles using an **ultrasonic sensor** mounted on a **servo motor**.



## Components
- **Arduino Uno** – main controller
- **Breadboard** – wiring connections
- **L293D Motor Driver IC × 2** – controls 4 DC motors
- **DC Motors × 4** – drive the wheels
- **Tower Pro SG90 Servo Motor × 1** – rotates ultrasonic sensor
- **HC-SR04 Ultrasonic Sensor × 1** – measures distance to obstacles
- **9V Battery** – power supply
- **Jumper Wires** – for connections

## How It Works
1. The Arduino sends control signals to the L293D motor drivers to run the DC motors according to the programmed sequence.
2. The HC-SR04 ultrasonic sensor measures the distance to objects in front of the robot.
3. If the sensor detects an obstacle within 10 cm:
   - The motors stop
   - The servo motor sweeps the sensor left and right to check for a clear path
   - The robot moves backward briefly
   - The robot turns right before resuming its sequence



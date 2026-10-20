A Bluetooth-controlled Arduino robot car is a wireless robotic vehicle that uses an Arduino microcontroller as its "brain," an HC-05 or HC-06 Bluetooth module for remote communication, and a motor driver to steer DC motors. You drive it wirelessly using a smartphone app.


Core Components

• Arduino UNO / Nano: Processes incoming wireless data and sends movement commands to the motors.
• HC-05 or HC-06 Bluetooth Module: Receives serial commands (like forward, backward, left, right, stop) sent from your smartphone.
• L298N / L293D Motor Driver: Manages the electrical power and direction for the DC motors since the Arduino cannot power motors directly.
• Chassis & DC Motors: A 2WD or 4WD platform with wheels, BO motors, and caster wheels for mobility.
• Power Source: Rechargeable batteries (such as 18650 Li-ion cells or a 7.4V/9V pack).

How It Works

1. Pairing: You turn on the robot and pair your smartphone via Bluetooth to the HC-05 module (using default PIN 1234 or 0000).
2. Sending Commands: Using an Android app like Arduino Bluetooth RC Car, pressing directional buttons transmits single-character commands (e.g., 'F' for Forward, 'B' for Backward, 'L' for Left, 'R' for Right, 'S' for Stop).
3. Execution: The Arduino reads these characters through its serial port, interprets the command, and signals the L298N motor driver to turn the wheels accordingly.

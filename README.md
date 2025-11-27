# Photobioreactor_code
This firmware runs on an Arduino UNO R4 WiFi to automate a continuous culture photobioreactor. It utilizes a non-blocking state machine to manage sensors, actuators, and IoT connectivity simultaneously.

Key Features:

Turbidostat Control: Automatically performs dilution cycles (drain & refill) based on turbidity sensor readings to keep cells in the exponential growth phase.

Environmental Regulation: Maintains temperature via a hysteresis loop and controls LED intensity and aeration speed using PWM.

IoT Connectivity: Connects to Ubidots via MQTT for real-time data logging and remote setpoint adjustment.

Safety Protocols: Includes hardware interlocks for the heater (dry-run protection), valve safety checks, and operation timeouts to prevent overflows.

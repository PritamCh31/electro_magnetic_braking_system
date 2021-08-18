# electro_magnetic_braking_system
The braking system is activated on pressing the clutch. Pin number 8 of the arduino is assigned to check if the clutch is pressed or not. When the clutch is pressed, the ultrasonic sensors start sensing if there is any obstacle in close range to the vehicle and also measures the distance from it simultaneously. Pin numbers 6 and 11 have been assigned to control the trigger pins for left and right ultrasonic sensor respectively. These pins are programmed to emit ultrasonic pulses continuously in short time intervals (some microseconds). Pin number 6 and 10 of arduino monitors the echo pins of the ultrasonic sensors. If any of the emitted ultrasonic waves gets reflected from some obstacle it is received by the echo of the sensors, which is subsequently relayed to the arduino microcontroller via 6th and 10th pin as 1(HIGH) for further processing. If there is no obstacle in front of the vehicle, 0(LOW) will be relayed.
# LED-chaser-circuit-Sequential-LED-flasher-using-4017-IC-and-555-timer

LED chaser lights (or) sequential LED flasher circuit on a breadboard using 555 timer + 4017 IC and a few other components. The LED’s chasing rate can be adjusted using a potentiometer in place of 47K resistor. Watch the video above for detailed step by step instructions on how to build this circuit. Explanation of how the circuit works is also included in the video.

[Schematic for this LED chaser circuit is at the end of this Page]

Components Required:
555 Timer IC
CD 4017 IC
LED Lights x10
Resistors: 470R, 1K, 47K
Capacitor: 1uF
Breadboard
Lot of Breadboard Connectors
Power Supply: (5-15)V
[Note: If you are using this circuit with a power source of 9v or above, use a 1K resistor in place of 470R.]

Explanation of Circuit’s Working:
The 555 timer IC is configured to work in astable mode. Which means, the output from the 555 timer changes continuously between high (Supply Voltage) and low (0V). In other words, if you connect an LED between the output of 555 timer and ground, the LED flashes/blinks continuously.

This pulsing output from the 555 timer is connected to the clock input of 4017 IC (a decade counter). It has 10 output pins and we have connected an LED to each output. By default, the first output pin is on/high and the rest are off. Each time the clock input pin of 4017 IC detects a rise in voltage (from low to high), it turns off the current output and turns on the next sequential output. This swapping of outputs which looks like the LED’s are chasing each other, continues until the last LED and then the output resets back to the first LED.

For this LED chaser circuit, we have used all the 10 outputs of 4017 IC. But if you wish to make an LED chaser circuit with less than 10 LED’s, you can do the same by connecting the LED’s starting from U0. Let’s say you wish to build this circuit with 4 LED’s, you need to connect an LED to each of U0, U1, U2, U3 and leave the rest.

Circuit Diagram:

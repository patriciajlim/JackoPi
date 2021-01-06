# Jack-o-Pi

A pumpkin that scares you when you walk by. Powered by a Raspberry Pi, Unicorn Hat, tiny speaker, and some python.

# How it works

When you walk by the Jack-o-Pi, a sensor detects your motion and 'tells' Raspberry Pi that motion has been detected. Raspberry Pi then turns on its lights to light up the Pumpkin with a candlelight effect and scares you with a ghost scream! 

# How it really works (under the hood)

A unicorn hat and speaker are connected to the Raspberry Pi via GPIO pins, and a sensor is connected to the Arduino Uno. 


The Arduino is hooked up to the Raspberry Pi via USB and sends a signal via serial communication to Raspberry Pi whenever it detects motion. 


Raspberry Pi runs a python script that listens for serial messages from the Arduino, and when the Pi receives the signal, it lights up the LEDs on the Unicorn Hat in a red, orange, and yellow candlelight effect while playing a ghost scream sound effect through the connected speaker on the audio jack

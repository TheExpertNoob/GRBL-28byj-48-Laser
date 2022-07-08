# GRBL 28byj-48 + PWM Laser

This GRBL uses an ugly hack to control two motors unipolar steps as 28byj-48 and also supports a PWM Laser on pin 11

The motors (28byj-48) are connected to a controller card that uses the chip ULN2003. This board is connected to pins A0(IN4), A1(IN3), A2(IN2), A3(IN1) for the Y axis and 2(IN1),3(IN2),4(IN3),5(IN4) digital pins to the axis X. The Laser PWM signal connected to pin 11.

Credits to costycnc who modified grbl from bipolar to unipolar: https://github.com/costycnc/costycnc-costycnc-grbl-1.1-unipolar 

Credits to peppe-catena who did support the PWM Laser: https://create.arduino.cc/projecthub/tsaritsynskyyaa/mini-laser-engraver-on-28byj-48-motors-1d851f

I tested the code with 328p (Arduino Pro Mini), not with 2560 (Arduino Mega) because I do not have a 2560 to test the alterations in the file cpu_map_atmega2560.h

Possibly more alterations and tweaks to come.

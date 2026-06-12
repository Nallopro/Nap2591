# Nap2591
A low-cost, extremely low-light handheld sensor powered by 2x AAA batteries. Made up of a TSL2591 light sensor, a 0.96" OLED screen, an Esp32 super mini, and a few more electronic components.

--------------------------------------------------------------------------------------------------------

I made some night vision goggles and I wanted to test in how much darkness they could see and record it.

If I used my phone, you would rely on a “trust me bro, the night is dark”. I wanted real, kinda accurate data, so I got to searching and found out about the TSL2591. I had already been messing around with ESP32s, and I decided to build smt...

The ESP32 is overkill for this project, but I hope to add more functionality, like Bluetooth to check out the data, or maybe redesigning the UI on the screen.

I’m still a newbie, so suggestions/help are always appreciated!!

--------------------------------------------------------------------------------------------------------

Consumes 20 mAh @ 3 V. Powered with 2x AAA batteries, it should achieve nearly 50 h of runtime. Be aware that it will drain your batteries until the sum of them is under 0.7 V, which is the minimum voltage required in order to work.

It uses a boost converter that takes the battery voltage and gives a nice and stable 3.3 V for the ESP32.

Can measure between 88k and 188 µlux. To measure light under 0.1 lux, it’s recommended to switch to slow mode, which reduces reading speed but can achieve a reading in way darker places.

--------------------------------------------------------------------------------------------------------

What will you need:
Parts (20$):
1× ESP32-C3 Super Mini
1× TSL2591 PCB
1× SSD1306 0.96" OLED screen
1× 3.3 V boost converter
1× 2×AAA battery holder, in series
1× passive buzzer
1× 220 Ω through hole resistor, DIN0207 (this is the buzzer resistor)
1× 220 kΩ through hole resistor, DIN0207
1× 100 kΩ through hole resistor, DIN0207
1× 105 / 1 µF ceramic capacitor
1× 106 / 10 µF ceramic capacitor
1× SS54 Schottky diode, SMA package
1× button
2× SMD switches

1× PCB

2× AAA batteries

Tools:
Soldering equipment
Wire cutters
And if you are not feeling brave, some tweezers
3D printer (or buy a case)

--------------------------------------------------------------------------------------------------------

How to asemble:

Read the stuff printed on the PCB it should help clear out any doubts.
Solder the boost converter before the screen and the TSL2591 after the resistors/buzzer.




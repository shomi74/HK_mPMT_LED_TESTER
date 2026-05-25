# Lessons Learned

## USB Cable
A charge-only micro-USB cable will power the Pico but may not allow flashing or serial communication. Use a data-capable cable.

## Serial Line Ending
The serial monitor must use LF line ending.

## Channel Numbering
Firmware channels start from zero:
- ON 0 controls the first LED
- ON 1 controls the second LED

## Wiring
If an LED is connected to GND instead of its GPIO, it will stay on permanently.

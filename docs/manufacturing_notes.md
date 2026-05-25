# Manufacturing Notes

## PCB
- Two-layer PCB is sufficient.
- Pour GND on both top and bottom layers.
- Route signal lines on the bottom layer where practical.
- Route 3V3 and COMMON_ANODE as normal traces, not large power pours.
- Use 1206 20 kΩ resistor for easy hand soldering.

## Connector
- Verify 2x10 connector pin numbering.
- Mark pin 1 on silkscreen.
- Label CH0-CH18 and COMMON_ANODE.

## Assembly
- Inspect for solder bridges near the connector.
- Verify resistor value before assembly.
- Verify continuity from Pico pins to connector pins.

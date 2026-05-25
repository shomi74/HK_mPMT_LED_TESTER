# Interface Definition

## Pico to Carrier Board
The Raspberry Pi Pico plugs into the carrier board through standard Pico headers.

## Carrier Board to Cap
A 20-pin connector carries:
- CH0 to CH18
- COMMON_ANODE

## Connector Signals
CH0-CH18 are LED cathode control lines.
COMMON_ANODE is the shared LED anode supply after the 20 kΩ resistor.

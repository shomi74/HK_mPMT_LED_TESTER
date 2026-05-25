# System Architecture

## Block-Level Description
The system has three main blocks:

1. Raspberry Pi Pico controller
2. Pico carrier/interface board
3. LED cap harness assembly

## Electrical Flow
- Pico GP2-GP20 connect to 19 LED cathode channels.
- Pico 3V3 feeds a single 20 kΩ resistor.
- The resistor output becomes `COMMON_ANODE`.
- `COMMON_ANODE` is distributed to all LED anodes.

## Operating Mode
Only one LED channel is intended to be active at a time. This avoids current-sharing issues in the shared-anode architecture and supports unambiguous PMT mapping.

## Firmware Interface
The Pico accepts commands over USB serial:
- `TEST`
- `ON <channel> <duty>`
- `OFF`
- `GET`
- `SET`
- `HELP`

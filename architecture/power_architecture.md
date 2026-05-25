# Power Architecture

## Input Power
The Raspberry Pi Pico is powered from USB.

## LED Supply
The LED common anode rail is supplied by Pico `3V3_OUT` through a single 20 kΩ resistor.

## Final Connection
`3V3_OUT -> 20 kΩ -> COMMON_ANODE -> all LED anodes`

Each LED cathode is connected to a separate Pico GPIO through the carrier-board connector.

## Notes
Do not connect COMMON_ANODE directly to 3V3. The 20 kΩ resistor is required to limit LED current.

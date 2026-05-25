# Design Review Notes

## Reviewed Items
- Pico GPIO mapping
- 20-pin connector pinout
- shared-anode LED architecture
- single 20 kΩ resistor location
- active-low firmware behavior
- DRC status

## Key Design Assumption
The firmware drives one LED at a time. The shared resistor approach relies on this operating mode.

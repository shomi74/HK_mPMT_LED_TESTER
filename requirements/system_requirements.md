# System Requirements

## Purpose
The mPMT LED Mapping Tester shall provide controlled LED illumination for verifying mPMT channel mapping.

## Functional Requirements
- Drive 19 LED positions independently.
- Enable one LED channel at a time.
- Allow brightness adjustment using PWM duty command.
- Provide USB serial command control.
- Support simple firmware flashing using a UF2 file.
- Use red LEDs unless otherwise specified by the collaboration.

## Electrical Requirements
- Controller: Raspberry Pi Pico RP2040.
- LED drive: active-low GPIO drive.
- Final cap architecture: shared-anode LED wiring.
- Common anode resistor: nominal 20 kΩ.
- Channel pins: GP2 through GP20.

## Mechanical Requirements
- LEDs shall be mounted in 3D-printed holders.
- LED holders shall fit into the mPMT cap positions.
- Wiring shall be strain-relieved near the cap exit point.
- Connector pinout shall be clearly documented.

## Documentation Requirements
- Provide flashing guide.
- Provide serial command reference.
- Provide connector mapping.
- Provide BOM and procurement notes.
- Provide bringup and validation checklist.

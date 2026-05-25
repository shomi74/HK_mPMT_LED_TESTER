# Hyper-K mPMT LED Mapping Tester

## Overview
This repository documents the Hyper-Kamiokande mPMT LED Mapping Tester.

The tester uses a Raspberry Pi Pico RP2040 to sequentially drive red LEDs mounted in a 3D-printed cap. The cap is placed over an mPMT dome so each LED can illuminate a known PMT position. The detected signal is then used to verify PMT channel mapping.

## Main Features
- Raspberry Pi Pico RP2040 controller
- 19-channel LED mapping interface
- USB serial command interface
- PWM brightness control
- Active-low LED drive
- Shared-anode final LED wiring architecture
- 20-pin carrier-board connector for cap harness
- UF2 firmware workflow for simple flashing

## Quick Use
1. Flash `firmware/uf2/mpmtblink.uf2` to a Raspberry Pi Pico.
2. Open a serial monitor at 115200 baud.
3. Set line ending to LF.
4. Send `TEST`.
5. Use `ON <channel> <duty>` and `OFF` to control LEDs.

## Repository Sections
- `requirements/` — system-level requirements
- `architecture/` — electrical and software architecture
- `docs/` — setup, flashing, manufacturing, and deployment notes
- `firmware/` — firmware source, UF2 releases, and debug notes
- `hardware/` — public hardware notes and pointer to private engineering files
- `bringup/` — first-power-up and debug checklists
- `validation/` — channel-mapping and measurement records
- `images/` — diagrams, PCB screenshots, assembled photos, and validation images

## Status
Initial Pico prototype validated on breadboard. USB serial command interface works, and LED channels can be controlled individually.

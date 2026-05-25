# Firmware Flash Guide

## No-Build Method
Use this method when a UF2 file is already available.

1. Hold the BOOTSEL button on the Pico.
2. Plug the Pico into the computer using a micro-USB data cable.
3. A drive named `RPI-RP2` appears.
4. Copy `mpmtblink.uf2` to the drive.
5. The Pico reboots automatically.

## Build Method
Use this method only if firmware source has changed.

Required tools:
- VS Code
- Raspberry Pi Pico extension
- CMake Tools
- ARM GCC toolchain

Build the project using CMake and copy the generated UF2 to the Pico.

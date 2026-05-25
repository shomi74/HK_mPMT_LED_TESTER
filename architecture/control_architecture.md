# Control Architecture

## Active-Low Drive
The firmware drives LED channels as active-low outputs:
- GPIO high = LED off
- GPIO low/PWM low-time = LED on

## Channel Numbering
The firmware uses zero-based channel numbering:
- Channel 0 = GP2
- Channel 1 = GP3
- ...
- Channel 18 = GP20

## Single-Channel Behavior
The firmware is intended to keep only one active LED channel at a time. Sending a new `ON` command changes the active channel.

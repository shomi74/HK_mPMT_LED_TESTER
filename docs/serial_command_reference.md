# Serial Command Reference

## TEST
Checks communication.

Command:
`TEST`

Expected response:
`OK`

## ON
Turns on a channel with PWM duty.

Command:
`ON <channel> <duty>`

Example:
`ON 0 1000`

## OFF
Turns off the active channel.

Command:
`OFF`

## GET
Returns current channel/settings.

## HELP
Lists supported commands if implemented in the firmware.

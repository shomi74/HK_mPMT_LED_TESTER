# Bringup Checklist

- Inspect board visually.
- Verify no shorts between 3V3 and GND.
- Verify R101 is 20 kΩ.
- Verify 3V3 -> R101 -> COMMON_ANODE -> connector pin 20.
- Flash UF2.
- Open serial monitor at 115200 baud with LF line ending.
- Send `TEST`; expect `OK`.
- Test CH0 through CH18 individually.

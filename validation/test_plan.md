# Validation Test Plan

## Objective
Verify all 19 LED channels respond correctly and match the expected PMT positions.

## Tests
1. Serial communication test
2. Individual LED activation test
3. Channel mapping test
4. Brightness/duty response test
5. Cap harness continuity test

## Acceptance Criteria
- TEST command returns OK.
- All 19 channels activate the expected LED.
- No LED remains on after OFF.
- Connector mapping matches documentation.

---
author: sunrisesteel
date: 2025-07-07
revision: 1
---
# MG5 Camera Harness

This overview of a camera harness for the MG5, for connecting to the LKAS camera, car harness, and Comma 3X relay box.

## Electrical Checks

Before connecting, verify the following & check on the harness that goes to the LKAS camera with a multimeter:

- **LKAS Camera / FVCM *(Front Vechile Camera Module) (Manu Part No):** 11047791/01
- **Resistance (Pins 1-7):** ~125–135 Ω
- **Resistance (Pins 2-8):** ~60–65 Ω
- **Voltage (Pins 6-7):** 12V

## Connectors and Parts

### LKAS Camera Side

- **TE Connector/Cable Strain Relief:** `1-1534096-1`
- **TE Insert:** `1534100-1`
- **TE Pins:** `5-928999-1`

### Car Harness Side

- **TE Connector:** `1-1534840-1`
- **TE Pins:** `6-928918-1`

### Comma 3X Relay Box Side

- **Molex Connector:** `501646-1800`
- **Molex Pins:** `501648-1000`

## Wiring
|               |LKAS TE | RELAY MOLEX | HARNESS TE  |
| Function      |PIN     | PIN         | PIN         |
|---------------|--------|-------------|-------------|
| RADAR_CAN (L) |   1    |      9      |             |
| RADAR_CAN (H) |   7    |     11      |             |
| CHASIS_CAN (L)|   2    |     18      |             |
| CHASIS_CAN (H)|   8    |     16      |             |
| GND           |   5    |     17      |             |
| IGNITION (12V)|   6    |     14      |             |
| LOOP BACK     |        |     13      |             |
| LOOP BACK     |        |     15      |             |
| RADAR_CAN (L) |        |      7      |      1      |
| RADAR_CAN (H) |        |      8      |      7      |
| CHASIS_CAN (L)|        |      6      |      2      |
| CHASIS_CAN (H)|        |      4      |      8      |
| GND           |        |      1      |      5      |
| IGNITION (12V)|        |      2      |      6      |

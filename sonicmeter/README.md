# sonicmeter

A Flipper Zero app that measures distance using an **HC-SR04** ultrasonic sensor.

## Screenshot

> _Add a photo or screenshot here_

## Hardware

### Wiring

| HC-SR04 | Flipper Zero GPIO |
|---------|-------------------|
| VCC     | 5V (pin 1) — enable OTG in app |
| GND     | GND (pin 11 or 18) |
| TRIG    | A4, A6, or A7 (configurable) |
| ECHO    | B2 or B3 (configurable) |

> **Note:** The HC-SR04 requires 5V. The app enables the Flipper's OTG output automatically.

## Features

- Live distance readout in cm
- Configurable trigger and echo pins
- Debug mode showing raw tick count and pulse duration in microseconds

## Usage

1. Wire up the HC-SR04 as above
2. Open the app → **Config** to set your trigger and echo pins
3. Go to **Measure** — distance updates every 200ms
4. Toggle **Debug** in Config for raw timing data

## Building

```bash
cd sonicmeter
ufbt
```

Or place the folder in `applications_user` in your firmware tree and build with `fbt`.

## License

[GPL-3.0](../LICENSE)

# flipperzero-apps

A collection of external apps for the [Flipper Zero](https://flipperzero.one/), written in C using the official Flipper SDK.

Each app lives in its own subfolder and builds independently.

---

## Apps

### [sonicmeter](./sonicmeter)
Measures distance using an **HC-SR04** ultrasonic sensor wired to the Flipper Zero GPIO pins.

- Configurable trigger and echo pins (A4, A6, A7 / B2, B3)
- Live distance readout in cm
- Optional debug mode showing raw ticks and pulse duration
- 5V output via OTG to power the sensor

---

## Building

Requirements: [Flipper Zero firmware toolchain](https://github.com/flipperdevices/flipperzero-firmware)

```bash
# Clone this repo inside your firmware tree or use ufbt
git clone https://github.com/ChrisMavrommatis/flipperzero-apps

# Build a specific app with ufbt
cd flipperzero-apps/sonicmeter
ufbt
```

Or add the app folder to your firmware's `applications_user` directory and build with `fbt`.

---

## License

[GPL-3.0](./LICENSE)

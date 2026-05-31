# Crkbd - ZMK firmware configuration

<p align="center"><img src="https://github.com/user-attachments/assets/8ed7ae5e-146a-48ce-9c4d-cd8a6668f7bd"/></p>

This repository contains my custom [ZMK](https://zmk.dev/) firmware configuration for a **Crkbd / Corne** split keyboard.

The keyboard was hand-built from the original open-source Corne project by [foostan/crkbd](https://github.com/foostan/crkbd), with a Tenstar nRF52840 controller used as a nice!nano v2 equivalent.

## Hardware

- Split Corne layout with 6 columns per side
- 3 thumb keys on each side
- Tenstar nRF52840 controllers, built as `nice_nano_v2`
- Brown switches
- White uniform-profile keycaps
- OLED displays for layer/status output
- Firmware: ZMK

## Firmware Layout

```text
Crkbd/
├── .github/workflows/build.yml   # GitHub Actions firmware build
├── build.yaml                    # Build matrix for left/right halves
├── config/
│   ├── corne.conf                # Shared Corne ZMK config
│   ├── corne.keymap              # Shared keymap for both halves
│   └── west.yml                  # Pinned ZMK version
└── zephyr/module.yml             # ZMK module metadata
```

The build is pinned to ZMK `v0.3.0` for stability. The current matrix builds:

- `nice_nano_v2` + `corne_left`
- `nice_nano_v2` + `corne_right`

## Keymap

The keymap has three layers:

- `Base`: QWERTY-style typing layer
- `Lower`: numbers, arrows, Bluetooth profile selection, bootloader
- `Raise`: symbols and accent-friendly keys

Bluetooth profile keys are on `Lower`:

- `BT_SEL 0` through `BT_SEL 4`
- `BT_CLR`
- `BT_CLR_ALL`

The physical key next to `L` sends `SEMI`, which is the usual HID key used by the `ç` position when the host OS is set to a Brazilian/ABNT-style layout.

## Build and Flash

1. Push changes to GitHub.
2. Open the repository's Actions tab.
3. Run or wait for **Build ZMK firmware**.
4. Download the generated firmware artifacts.
5. Flash the left `.uf2` to the left half and the right `.uf2` to the right half.

To enter bootloader from the keyboard, hold the `Lower` layer and press the bootloader key on the lower layer.

## Local Notes

This repository is a ZMK user config, not a full ZMK checkout. Local builds require a ZMK/west toolchain setup. GitHub Actions is the intended build path for this repo.

## Photo

![photo_2025-07-04_16-46-52](https://github.com/user-attachments/assets/6ee9ff8e-bb90-44d3-8bf3-26939c76cf3a)

## Credits

- Original keyboard project: [foostan/crkbd](https://github.com/foostan/crkbd)
- Firmware: [ZMK Firmware](https://zmk.dev/)

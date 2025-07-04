# Crkbd - Custom Configuration for My Split Keyboard

<p align="center"><img src="https://github.com/user-attachments/assets/8ed7ae5e-146a-48ce-9c4d-cd8a6668f7bd"/></p>

This repository contains my custom [ZMK](https://zmk.dev/) firmware configuration for the **Crkbd (Corne Keyboard)** split keyboard.

I built this keyboard **entirely from scratch** — from soldering all components to setting up the firmware — using the original open-source project as a base:  
🔗 [foostan/crkbd](https://github.com/foostan/crkbd)

## 🛠️ Keyboard Specifications

- 🔹 Split layout with 6 columns per side
- 🔹 3 thumb keys on each side
- 🔹 Brown switches
- 🔹 White uniform-profile keycaps
- 🔹 OLEDs for layer/status display
- 🔹 Firmware: [ZMK Firmware](https://zmk.dev/)

## 📁 Repository Structure

```
Crkbd/
├── config/
│   ├── keymap.keymap         # Key mapping
│   ├── shields/              # Hardware-specific definitions
│   └── ...                  
├── zmk-config/               # ZMK environment configuration
└── README.md
```

> **Note:** This repo is currently tailored for ZMK, but can be adapted for QMK builds if needed.

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/ImLusca/Crkbd.git
   ```

2. Follow the official ZMK setup guide:
   👉 https://zmk.dev/docs

3. Compile and flash the firmware using the configuration files from this repo.

## 📸 My Build

![photo_2025-07-04_16-46-52](https://github.com/user-attachments/assets/6ee9ff8e-bb90-44d3-8bf3-26939c76cf3a)

Hand-assembled keyboard based on the original Crkbd project. Every part was soldered and put together by me, with special care given to ergonomics and portability for daily work and programming.

## 💡 Credits

- Original project: [foostan/crkbd](https://github.com/foostan/crkbd)
- Firmware: [ZMK Firmware](https://zmk.dev/)

## 📜 License

This repository is licensed under the [MIT License](LICENSE).

---

Feel free to clone and adapt it for your own split keyboard!

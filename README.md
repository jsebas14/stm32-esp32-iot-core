# stm32-esp32-iot-core

**stm32-esp32-iot-core** is a dual-MCU embedded system that integrates an STM32 microcontroller and an ESP32 module to create a flexible IoT-ready firmware platform. This project includes a bootloader and main application for the STM32, as well as Wi-Fi-enabled firmware for the ESP32, communicating via UART to coordinate data exchange, control, and connectivity.

---

## 📁 Project Structure

```text
stm32-esp32-iot-core/
├── stm32/
│   ├── bootloader/         # STM32 bootloader (firmware validation + handoff)
│   └── application/        # Main STM32 application (sensor/control logic)
├── esp32/
│   └── firmware/           # ESP32 firmware (Wi-Fi / communication bridge)
├── docs/                   # Diagrams, documentation, architecture specs
├── .gitignore
└── README.md
```

---

## 🚀 Features

- 🔒 **STM32 Bootloader**: Handles firmware validation and jump to main app; designed for OTA support.
- 🎛️ **STM32 Application**: Handles real-time operations, I/O control, or sensor logic.
- 📡 **ESP32 Firmware**: Acts as a network bridge (Wi-Fi / MQTT / Bluetooth) to the cloud or other systems.
- 🔄 **UART-based Communication**: Efficient and structured data exchange between STM32 and ESP32.
- 🧩 **Modular Codebase**: Easy to extend or adapt to other hardware or protocols.

---

## ⚙️ Technologies Used

- STM32CubeIDE (HAL Drivers, STM32F767 family)
- ESP-IDF (ESP32 development framework)
- C (firmware development)
- Git (version control)

---

📚 Documentation

docs/architecture.md — System architecture and module interaction

docs/serial-protocol.md — Message format and command list

docs/flash-guide.md — How to flash and test both MCUs

---

🎯 Project Goals

This project showcases the integration of two embedded platforms in a cooperative architecture, emphasizing clean structure, modularity, and real-world IoT applications such as remote control, data reporting, or OTA updates.

---

🧑‍💻 Author

Juan Sebastian Bermudez

Embedded Systems Engineer / Firmware Developer

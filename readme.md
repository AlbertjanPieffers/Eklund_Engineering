# Eklund Engineering Git Database

Welcome to the official repository for Eklund Engineering PLC programming. This project includes back-ups, examples and documentation.

## 📦 Project Overview

This repository contains:

- 🧠 Encoder configuration using Fast Mode
- 📏 Pulsfactor calculation based on real movement
- 🔄 Index pulse (Z-pulse) interpretation in Fast Mode
- 🧰 Git integration with TIA Portal for version control
- ⚙️ Practical solutions to common TIA V16 errors
- 🔎 Analysis of module address assignments
- 📚 Examples of structured FBD/SCL logic

---

## 🔧 Technologies Used

- **Siemens TIA Portal V16**
- **S7-1200 / S7-1500 PLCs**
- **High Speed Counter modules (1-count in Fast Mode)**
- **Git for Windows** (for project version control)

---

## ⚙️ Encoder Setup (Fast Mode)

This project includes examples of configuring a 1-count HSC module in **Fast Mode**, interpreting the encoder word from `%IW112`, and handling the 32-bit status word starting from `%ID110`.

> ✅ **Z-pulse detection** is done using **bit 27** of the status word (STS_DI), _not_ a traditional `%I110.4` digital input.

---

## 📐 Pulsfactor Calculation

We provide logic to calculate how many millimeters per encoder pulse the system moves:

Pulsfactor = Travelled Distance / Number of Pulses
This is essential for precise motion scaling and NC integration in custom positioning logic.

---

## 🙋 Contact

For questions, ideas or to report a security issue:

📧 **info@eklund-engineering.com**  
🔒 **security@eklund-engineering.com**

---

## 📄 License

This project is **proprietary and confidential**. All content is owned by **Eklund Engineering** and may not be reproduced, redistributed, or reused without explicit permission.


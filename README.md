
---

# VSD-IDF  
**VLSI System Design - IoT Development Framework**  

[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](LICENSE)  
[![Arduino Compatible](https://img.shields.io/badge/Arduino%20IDE-Compatible-brightgreen)](https://www.arduino.cc)  

A unified framework for developing IoT applications on **THEJAS32 RISC-V SoCs**, designed for VSD’s custom boards like **VSDSquadron Ultra** and **VSD32-S3**.  

---

## Overview 📌  
VSD-IDF is a flexible IoT framework optimized for **VSD RISC-V boards**, featuring:  
- **THEJAS32 RISC-V CPU** support (32-bit, 100+ MHz)  
- Preconfigured **WiFi/BLE** stacks (Ai-Thinker & ESP32-C3 modules)  
- Arduino IDE integration for rapid prototyping  
- Secure OTA updates, low-power modes, and sensor libraries  

**Current Testing**:  
- **VEGA ARIES Boards** (THEJAS32 reference designs)  

**Future Support**:  
- **VSDSquadron Ultra**: THEJAS32 + Ai-Thinker WiFi/BLE  
- **VSD32-S3**: THEJAS32 + ESP32-C3 WiFi/BLE  

---

## Key Features 🚀  
✅ **RISC-V First**: Leverage open-source RISC-V ISA for energy-efficient edge computing.  
✅ **Multi-Module Connectivity**:  
   - Ai-Thinker (VSDSquadron Ultra)  
   - ESP32-C3 (VSD32-S3)  
✅ **Arduino IDE Integration**: Install boards via `package_vega_index.json`.  
✅ **Hardware-Agnostic HAL**: Portable across THEJAS32-based boards.  
✅ **Production-Ready**: Secure boot, encrypted OTA, and BSP templates.  

---

## Getting Started 🛠️  

### 1. Install in Arduino IDE  
1. Add this URL to **File > Preferences > Additional Boards Manager URLs**:  
   ```  
   https://github.com/VSD-Systems/VSD_IDF/raw/main/package_vega_index.json  
   ```  
2. Install **"VEGA ARIES Boards"** via **Tools > Board > Boards Manager** (current test platform).  

### 2. Dependencies  
```bash
# Install Git LFS for large file support
sudo apt-get install git-lfs
git lfs install
```


---

## Supported Hardware 🖥️  
| Board               | SoC       | Connectivity Module | Status         |  
|---------------------|-----------|----------------------|----------------|  
| VSDSquadron Ultra   | THEJAS32  | Ai-Thinker WiFi/BLE  | Upcoming       |  
| VSD32-S3            | THEJAS32  | ESP32-C3 WiFi/BLE    | In Development |  
| VEGA ARIES Boards   | THEJAS32  | Custom               | Tested         |  

---

## Documentation 📚  
- [**THEJAS32 Datasheet**](docs/THEJAS32_DATASHEET.md) - CPU specs and peripherals  
- [**BSP Customization**](docs/BSP_GUIDE.md) - Adapting to VSDSquadron Ultra/VSD32-S3  
- [**WiFi/BLE Setup**](docs/CONNECTIVITY.md) - Configuring Ai-Thinker & ESP32-C3  

---

## Roadmap 🗺️  
- **Phase 1**: VSDSquadron Ultra BSP release  
- **Phase 2**: VSD32-S3 integration  



---

## Acknowledgments  
- Built on open-source tools from [C-DAC VEGA](https://vegaprocessors.in/).  
- Inspired by ESP-IDF and Arduino Core.  

---

**Developed by VSD Systems**  
[Report Issues](https://github.com/VSD-Systems/VSD_IDF/issues) | [Request Features](https://github.com/VSD-Systems/VSD_IDF/discussions)  

---

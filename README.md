# 🚀 Week 0: VLSI System Design (VSD) Program Foundation & Tool Setup

<div align="center">

![VLSI](https://img.shields.io/badge/VLSI-System%20Design-red?style=for-the-badge&logo=chip)
![Week](https://img.shields.io/badge/Week-0-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

</div>

Welcome to my **VLSI System Design (VSD) Program** repository! This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

---

## 🎯 System and Virtual Machine Configuration

To ensure optimal performance, I configured a **Virtual Machine (VM)** with the following specifications:

<div align="center">

| **Specification** 💻    | **Details** 📋        |
|-----------------------|-----------------------|
| **Operating System** 🐧 | Ubuntu 24.04          |
| **RAM** 💾            | 6GB                   |
| **Storage** 💿          | 50GB HDD              |
| **vCPUs** ⚡            | 4                     |

</div>

> 💡 **Pro Tip:** This setup guarantees sufficient resources for handling toolchain demands and running simulations smoothly.

---

## ⚙️ Tool Installation & Verification

The following open-source EDA tools were installed and verified. Click on each one to see the installation commands and verification screenshot.

<div align="center">

`🧠 Yosys → 📟 Iverilog → 📊 GTKWave`

</div>

---

### 🧠 1. Yosys – RTL Synthesis Tool

* **Purpose:** A framework for Verilog RTL synthesis, used to convert digital circuit designs into gate-level representations.

<details>
<summary><b>Click to view Yosys Installation & Verification</b></summary>

#### Installation Commands
```bash
# Install dependencies
sudo apt-get update
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Clone, build, and install Yosys
git clone [https://github.com/YosysHQ/yosys.git](https://github.com/YosysHQ/yosys.git)
cd yosys
make
sudo make install
```
## 📷 **Installation Verification**
<p align="center">
  <img src="https://github.com/suryarandhi/RTL2GDS_surya_randhi/blob/assets/yosys.jpg?raw=true" 
       alt="Yosys Installed" width="600"/>
</p>

<div align="center">

✅ **Yosys Successfully Installed**

</div>
### 📟 **2. Iverilog – Verilog Simulator**

<details>
<summary><b>Purpose:</b> Compiles and simulates Verilog designs for functional verification.</summary>

Icarus Verilog is a Verilog simulation and synthesis tool that supports the IEEE-1364 Verilog HDL standard.

</details>

## **Iverilog Installation**
```bash
$ sudo apt-get install iverilog
```

## 📷 **Installation Verification**
<p align="center">
  <img src="https://github.com/suryarandhi/RTL2GDS_surya_randhi/blob/main/iverilog.png" 
       alt="Iverilog Installed" width="600"/>
</p>

<div align="center">

✅ **Iverilog Successfully Installed**

</div>

---

### 📊 **3. GTKWave – Waveform Viewer**

<details>
<summary><b>Purpose:</b> Analyzes and visualizes simulation waveforms for debugging.</summary>

GTKWave is a fully featured GTK+ based wave viewer for Unix, Win32, and Mac OSX.

</details>

## **GTKWave Installation**
```bash
$ sudo apt update
$ sudo apt install gtkwave
```

## 📷 **Installation Verification**
<p align="center">
  <img src="https://github.com/suryarandhi/RTL2GDS_surya_randhi/blob/main/gtkwave.jpg" 
       alt="GTKWave Installed" width="600"/>
</p>

<div align="center">

✅ **GTKWave Successfully Installed**

---

<div align="center">

## 🎉 Installation Summary

| Tool | Status | Primary Use |
|------|--------|-------------|
| 🧠 **Yosys** | ✅ Complete | RTL Synthesis |
| 📟 **Iverilog** | ✅ Complete | Verilog Simulation |
| 📊 **GTKWave** | ✅ Complete | Waveform Analysis |

### 🚀 Environment Ready for VLSI Design Journey!

</div>

---

<div align="center">

**📂 Repository:** [RTL2GDS_surya_randhi](https://github.com/suryarandhi/RTL2GDS_surya_randhi)  
**👨‍💻 Author:** [Surya Randhi](https://github.com/suryarandhi)  
**📚 Program:** VLSI System Design (VSD)

</div>

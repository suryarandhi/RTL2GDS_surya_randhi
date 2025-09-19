# Week 0: VLSI System Design Program Foundation & Tool Setup

![Status](https://img.shields.io/badge/STATUS-COMPLETE-green)
![Category](https://img.shields.io/badge/CATEGORY-VLSI-blue)
![Type](https://img.shields.io/badge/TYPE-System%20Design-informational)

Welcome to my VLSI System Design (VSD) Program repository! This week focused on setting up the development environment and installing the essential open-source tools that will be used throughout the program. The goal was to create a reliable and efficient workspace for synthesis, simulation, and design tasks.

---

## 🚀 System and Virtual Machine Configuration

To ensure optimal performance, I configured a Virtual Machine (VM) with the following specifications:

| Specification         | Details         |
| --------------------- | --------------- |
| 🖥️ **Operating System** | Ubuntu 24.04    |
| 🧠 **RAM** | 6GB             |
| 💾 **Storage** | 50GB HDD        |
| ⚙️ **vCPUs** | 4               |



---

## 🛠️ Tool Installation & Verification

The following tools were installed for RTL synthesis, simulation, and circuit analysis.

**Yosys → Iverilog → GTKWave**

### 1. Yosys - RTL Synthesis Tool

* **Purpose:** Converts RTL code (Verilog) into gate-level representations for chip design and FPGAs.

#### Yosys Installation

```bash
# Install dependencies
sudo apt-get update
sudo apt-get install build-essential clang bison flex \
	libreadline-dev gawk tcl-dev libffi-dev git \
	graphviz xdot pkg-config python3 libboost-system-dev \
	libboost-python-dev libboost-filesystem-dev zlib1g-dev

# Clone the repository and build from source
git clone [https://github.com/YosysHQ/yosys.git](https://github.com/YosysHQ/yosys.git)
cd yosys
make config-gcc
git submodule update --init --recursive
make
sudo make install

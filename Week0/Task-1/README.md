# 🌟 Week 0 / Task 1 — VSD Program Foundation & Tool Setup

Welcome to the beginning of my **RISC-V SoC Tapeout (VSD Program)** journey.  
This week was all about **building the environment** and **setting up essential tools** that will power my RTL-to-GDS design flow.

---

## 🖥️ Virtual Machine Configuration

A dedicated VM was configured to ensure smooth performance for synthesis, simulation, and waveform analysis.

| Resource | Configuration |
|----------|---------------|
| 🐧 **OS** | Ubuntu 20.04 LTS |
| 💾 **RAM** | 6 GB |
| 💿 **Storage** | 50 GB HDD |
| ⚡ **vCPUs** | 4 |

 **Why this setup?** → All are open source resources .Balanced resources for handling synthesis, running simulations, and debugging waveforms.

---

## ⚙️ Tools Installed & Verified

The following open-source tools were installed successfully:

| Tool | Purpose | Status |
|------|----------|--------|
| 🧠 **Yosys** | RTL synthesis (Verilog → Gate-level netlist) | ✔ Installed |
| 📟 **Icarus Verilog** | Compile & simulate Verilog designs | ✔ Installed |
| 📊 **GTKWave** | Waveform viewer for simulation results | ✔ Installed |

---

## 🔧 Installation Steps in Ubuntu




### 🧠 Yosys (RTL Synthesis Tool)

- `sudo apt-get update`  
- `git clone https://github.com/YosysHQ/yosys.git`  
- `cd yosys`  
- `sudo apt install make` 
- `sudo apt-get install build-essential clang bison flex \`  
  `libreadline-dev gawk tcl-dev libffi-dev git \`  
  `graphviz xdot pkg-config python3 libboost-system-dev \`  
  `libboost-python-dev libboost-filesystem-dev zlib1g-dev`  
- `make config-gcc`  
- `make`  
- `sudo make install`  

Verify: `yosys -V`


### 📟 Icarus Verilog (Tool to Compile & simulate Verilog designs )

- `sudo apt-get update`  
- `sudo apt-get install iverilog`  

✅ Verify: `iverilog -V`

###  📊 GTKWave (Waveform viewer for simulation results)


- `sudo apt-get update`  
- `sudo apt install gtkwave`  

✅ Verify: `gtkwave --version`



Summary

🖥️ Configured a Virtual Machine with Ubuntu  6 GB RAM, 50 GB storage, 4 vCPUs

⚙️ Installed and verified three key tools:

🧠 Yosys 

📟 Icarus Verilog 

📊 GTKWave 

 Environment is fully set up for upcoming VSD program tasks

A solid foundation is now in place — ready to design, simulate, and take the next step toward silicon.


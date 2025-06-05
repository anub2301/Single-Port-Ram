# Single Port RAM (Verilog) - Xilinx Vivado

This project implements a **Single Port RAM** using Verilog HDL and simulates/synthesizes it using **Xilinx Vivado**.

## 📁 Project Structure

single_port_ram/
├── src/
│ └── single_port_ram.v # Verilog code for single port RAM
├── sim/
│ └── tb_single_port_ram.v # Testbench for simulation
├── vivado_project/ # Vivado project files
├── README.md


## 🧠 Functionality

A single port RAM allows **read and write operations through a single address and data port**, controlled by enable and write enable signals.

### ✅ Features:
- Parameterized memory depth and data width
- Synchronous write and read operations
- Clock-based operation

## 📦 Usage

### 1. Open in Vivado
- Launch Vivado
- Create a new project and add `single_port_ram.v` and `tb_single_port_ram.v`
- Set simulation and synthesis constraints as needed

### 2. Run Simulation
- Use Vivado's **Behavioral Simulation** to verify the functionality
- Check waveform to validate correct read/write behavior

### 3. Synthesis
- Click **Run Synthesis** to generate the netlist
- Review utilization and timing reports

## 🔧 Parameters

You can customize the RAM by modifying the following parameters in `single_port_ram.v`:

```verilog
parameter DATA_WIDTH = 8;
parameter ADDR_WIDTH = 4;

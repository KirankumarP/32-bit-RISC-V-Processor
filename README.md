# 32-bit RISC-V Processor

## Overview
This project implements a basic 32-bit RISC-V Processor using Verilog HDL. The processor supports instruction fetch, decode, execution, memory access, and write-back operations through a datapath and control unit architecture.

## Features
- 32-bit RISC-V architecture
- ALU operations
- Control Unit
- Datapath implementation
- Instruction Memory and Data Memory interface
- Verilog-based design
- Testbench for simulation

## Project Structure

├── alu_mem.v          # ALU and memory operations
├── control_unit.v     # Control signal generation
├── datapath_units.v   # Datapath components
├── riscv_top.v        # Top-level processor module
├── tb_riscv.v         # Testbench
├── program.hex        # Program memory contents

## Tools Used
- Verilog HDL
- ModelSim / Vivado / Xilinx ISE
- GitHub

## Working
1. Instruction is fetched from memory.
2. Control unit decodes the instruction.
3. Datapath executes required operations.
4. ALU performs arithmetic/logic functions.
5. Results are written back to registers.

## Simulation
Compile all Verilog files and run the testbench:

```bash
iverilog *.v -o riscv
vvp riscv

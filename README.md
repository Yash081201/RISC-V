# 🚀 RISC-V Based 32-bit Processor with Custom 13-bit Addressing

This project features a fully functional 32-bit RISC-V processor implemented in HDL (Hardware Description Language), designed to operate with a custom 13-bit address bus and 19-bit little-endian internal data path. It was developed as part of a computer architecture course project at The University of Texas at Dallas during Fall 2023.

---

## 📌 Project Highlights

- ✅ RISC-V Compliant Core: Implements a subset of the RISC-V instruction set architecture (ISA) to support basic arithmetic, logical, load/store, and control instructions.
- 📐 13-bit Address Bus: Supports up to 8192 memory locations (2¹³), customized to meet architectural constraints. The processor uses a Harvard-like structure with instruction and data sharing the same address space.
- 🧠 Internal 19-bit Data Path: Data operations are executed using a non-standard 19-bit datapath in little-endian format, aligning with architectural customization.
- 🏁 Program Entry at 0x1000: As per system architecture constraints, all program execution begins at memory address `0x1000`, which is the midpoint of the memory map.
- 🔄 Instruction/Data Co-location: Instructions and data are stored in the same memory block, with branching logic and load/store operations coordinated accordingly.
- 🧪 SystemVerilog Testbench + UVM Environment: Full simulation and verification environment created to test the processor against various instruction sequences including loops, conditionals, and arithmetic operations.
- ⚙️ RTL Optimizations: Branching logic, address decoding, and ALU operation paths were carefully designed to meet functionality within the limited address range and memory layout.

---

## 🧰 Technologies Used

- HDL/RTL Design: SystemVerilog
- Verification: SystemVerilog Testbench with UVM methodology
- Simulation: Icarus Verilog (`iverilog`), GTKWave for waveform analysis
- Toolchain Compatibility: Project is structured for use with both open-source and proprietary tools

---

## 📂 Directory Structure




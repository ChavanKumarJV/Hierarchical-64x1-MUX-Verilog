# 📐 Hierarchical 64:1 Multiplexer Design in Verilog

### 📌 Project Overview
Designed and simulated a complex **64:1 Multiplexer** in **Verilog HDL** using a modular, hierarchical design approach. By instantiating multiple lower-order **16:1 Multiplexer** primitives and a final decoding stage, the architecture optimizes combinational logic flow, improves readability, and streamlines testbench verification.

---

### 🧩 Hierarchical Architecture
* **Stage 1 (Input Multiplexing):** Instantiates four parallel `16:1 MUX` modules to process the 64-bit data input bus (`in[63:0]`), controlled by the lower 4 selection lines (`sel[3:0]`).
* **Stage 2 (Output Routing):** Routes the 4 intermediate outputs from the 16:1 modules into a top-level `4:1 MUX` stage controlled by the upper 2 selection lines (`sel[5:4]`) to drive the final output.
* **Functional Verification:** Verified across all 64 selection states using a self-checking Verilog testbench and waveform analysis on **EDA Playground**.

---

### 🛠️ Tools & Technologies
* **Hardware Description Language:** Verilog HDL
* **Simulation & Verification:** EDA Playground, Waveform Viewer
* **Core Concepts:** Modular RTL Instantiation, Combinational Logic Optimization, Hierarchical Digital Design

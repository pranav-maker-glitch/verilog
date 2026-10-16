
# Digital Circuits Using Verilog HDL

## 📌 Project Overview

This repository contains the design and implementation
of Combinational and Sequential Digital Circuits
using Verilog HDL.

The circuits can be simulated and synthesized
using Xilinx Vivado.

## 🛠️ Tools and Technologies

- **Language:** Verilog HDL
- **Software:** Xilinx Vivado
- **Combinational Design:** Dataflow Modeling
- **Sequential Design:** Behavioral Modeling
- **Platform:** FPGA

---

## 🔹 1. Combinational Circuits

Combinational circuits produce outputs based only
on the present input values.

These circuits are implemented using `assign` statements.

### Implemented Circuits

| S.No | Circuit |
|------|---------|
| 1 | AND Gate |
| 2 | OR Gate |
| 3 | NAND Gate |
| 4 | NOR Gate |
| 5 | XOR Gate |
| 6 | XNOR Gate |
| 7 | Half Adder |
| 8 | Full Adder |
| 9 | 4-bit Adder |
| 10 | 4-bit Comparator |
| 11 | 4:1 Multiplexer |
| 12 | 8:1 Multiplexer |

### Example: AND Gate

```verilog
module and_gate(
    input a, b,
    output y
);

assign y = a & b;

endmodule
```

---

## 🔹 2. Sequential Circuits

Sequential circuits depend on present inputs
and previously stored states.

Flip-flops are implemented using clock-triggered
`always` blocks.

### Implemented Flip-Flops

| S.No | Circuit |
|------|---------|
| 1 | SR Flip-Flop |
| 2 | JK Flip-Flop |
| 3 | D Flip-Flop |
| 4 | T Flip-Flop |

### Example: D Flip-Flop

```verilog
module d_ff(
    input clk, rst, d,
    output reg q
);

always @(posedge clk) begin
    if (rst)
        q <= 0;
    else
        q <= d;
end

endmodule
```

---

## 📊 Combinational vs Sequential Circuits

| Combinational | Sequential |
|---------------|------------|
| No memory | Has memory |
| No clock required | Usually clock-based |
| Uses `assign` | Uses clocked `always` |
| Gates, Adders, MUX | Flip-Flops, Counters |

---

## 🚀 How to Run in Vivado

1. Open Xilinx Vivado.
2. Create a new RTL project.
3. Add the Verilog source files.
4. Select the required top module.
5. Run Behavioral Simulation using a testbench.
6. Run Synthesis.
7. View the RTL schematic.

---

## 🎯 Applications

- Digital Logic Design
- FPGA Development
- Computer Architecture
- Arithmetic Logic Unit (ALU)
- Digital Data Storage
- Microprocessor Design

---

## 📚 Learning Outcomes

- Understanding combinational logic circuits
- Understanding sequential logic circuits
- Implementing circuits using Verilog HDL
- Learning dataflow and behavioral modeling
- Understanding FPGA design using Vivado

---

## 📝 Conclusion

This repository demonstrates the fundamentals
of digital circuit design using Verilog HDL.

The project provides a foundation for developing
advanced digital systems and FPGA-based applications.

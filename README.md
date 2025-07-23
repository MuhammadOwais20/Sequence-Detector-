
##  Objective

Design and implement a digital logic circuit that detects the specific 8-bit binary sequence `01111110`. The detector should output a high signal (`z = 1`) when the sequence is fully matched on the positive edge of the clock.

---

##  Features

- **Single-bit input (w)** and **single-bit output (z)**
- Uses **Finite State Machine (FSM)** with 9 states (S0 to S8)
- Implemented with **D flip-flops** and **basic logic gates**
- Fully synchronous design based on **positive clock edges**
- Simulated and tested using **Verilog**

---

##  How It Works

- The circuit transitions through a sequence of states as it detects each correct bit.
- Any mismatch resets the FSM to an earlier state (or to S0).
- When the complete sequence `01111110` is detected, the FSM enters state S8 and sets `z = 1`.

---

##  Tools Used

- Verilog HDL
- Digital Simulator (e.g., ModelSim, GTKWave, Vivado)
- Logic design with flip-flops and gates

---

##  Output Condition

The output `z` becomes high (`1`) **only** when the system detects the exact 8-bit sequence `01111110`. Otherwise, it remains `0`.

---

##  Conclusion

This project demonstrates the design of a synchronous FSM-based sequence detector using flip-flops and logic gates. The Verilog implementation ensures accurate state transitions and reliable detection of the target binary pattern.

---


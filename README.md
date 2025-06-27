# 🧠 6-Bit Arithmetic Logic Unit (ALU)

## 📌 Abstract

This project presents the design and implementation of a `6-bit Arithmetic Logic Unit (ALU)` entirely built using **Logisim**. It replicates core CPU computation logic at the gate level and supports `16 unique operations`, including arithmetic, logical, shifting, and comparison-based functions. The design is modular, hierarchical, and instruction-driven.

---

## 🎯 Objectives

### ✔ Functional Goals

* Perform arithmetic operations: `Addition`, `Subtraction`, `Multiplication`, `Division`
* Implement logical operations: `AND`, `OR`, `NOT`, `XOR`
* Execute bit shifting: `Left Shift`, `Right Shift`
* Include control and utility ops: `Increment`, `Decrement`, `Equality`, `Less Than`, `Greater Than`, `Parity Check`

### ✔ Educational Goals

* Understand how primitive gates lead to complex computation
* Practice hierarchical modular circuit design
* Simulate control via `D Flip-Flop`-based opcode instruction selection

---

## 🔍 Background

The `ALU (Arithmetic Logic Unit)` is the computational backbone of any processor. This project demonstrates how such a system can be **designed from scratch** using only built-in logic gates and circuits within Logisim — no libraries, no black boxes, just raw logic.

---

## 🧰 Tools Used

* Software: `Logisim-win v2.7.1`
* Components: All standard built-in gates
* Design: Modular, top-down development with reusable subcircuits

---

## 🧩 Design Methodology

### 🔝 Top-Down Modular Flow

1. Build basic gates → `AND`, `OR`, `NOT`
2. Construct core logic units:
   * `Half Adder`, `Full Adder`
   * `2's Complement Subtractor`
   * `Bitwise Logic Units`
3. Integrate into functional blocks:
   * `Arithmetic Unit`
   * `Logic Unit`
   * `Shift Unit`
   * `Compare Unit`
   * `Utility Functions`
4. Control via:
   * `D Flip-Flop instruction latching`
   * `MUX-controlled Output Routing`

---

## ⚙️ Core Modules & Features

### 🔢 Arithmetic Unit
* `6-bit Adder` using Full Adders
* `Subtractor` using 2's complement
* `Multiplier` via iterative addition
* `Divider` via repeated subtraction

### 🧪 Logical Unit
* Bitwise `AND`, `OR`, `XOR`, `NOT` across 6-bit buses

### 🔁 Shift Unit
* `Left Logical Shift` with zero fill
* `Right Logical Shift` with zero fill

### ⚖ Comparison Unit
* Outputs for `Equal`, `Less Than`, `Greater Than`

### ➕ Utility Ops
* `Increment`: `X + 1`
* `Decrement`: `X - 1`
* `Parity Check`: Even/Odd 1’s in X
* `Zero Flag`: True if X == 0

---

## 🛰️ Control Mechanism

* Each operation is selected via `D Flip-Flops`, triggered by clock edges
* Only **one operation** can stay active at any time
* Removes glitching and toggling issues from traditional switches

---
## 👥 Team Contributions

| 👨‍💻 **Team Member**         | 🛠️ **Contribution Highlights**                                                                                                 |
|----------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| **Abdur Rehman Khan**      | - Designed `Zero Detection` and `Parity Check` flags <br> - Engineered `D Flip-Flop` based opcode control mechanism <br> - Ensured `signal exclusivity` and safe operation execution <br> - Validated module integrity and performed edge-case debugging <br> - Handled structural modularity and final documentation |
| **Syed Muhammad Sufyan**   | - Assembled and integrated the entire `Main ALU Circuit` <br> - Designed the `6-bit Divider Circuit` using repeated subtraction logic <br> - Controlled signal routing, output indicators, and simulation workflow <br> - Handled instruction latching and reset-safe input architecture |
| **Faizan Basheer**         | - Developed core arithmetic blocks: `Adder`, `Subtractor`, `Multiplier` <br> - Built the `Comparator Unit` for `==`, `<`, and `>` operations <br> - Implemented logical grouping of arithmetic modules <br> - Aided in design consistency across logic units and ensured arithmetic correctness |

---

## ✅ Results & Achievements

* Fully functional 6-bit ALU with 16 operations
* Built using over 120+ gates
* Modular, hierarchical, and visually debuggable design
* Stable and CPU-like instruction selection via Flip-Flops

---

## 📊 Future Scope

* Extend ALU to 8-bit or 16-bit architecture
* Add signed number support
* Integrate with memory and program counters for full CPU emulation

---
## 📫 Contact

- 📧 Gmail: [_abdurrehmankhan0909@gmail.com_](mailto:abdurrehmankhan0909@gmail.com)  
- 🔗 LinkedIn: [_Abdur Rehman Khan_](https://www.linkedin.com/in/abdur-rehman-khan-999198320?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

---

## 💬 Final Words

> **What began as wires became wisdom.**  
> This 6-bit ALU wasn’t just built | it was forged through bugs, logic, and late nights.  
> **Behold the beast:** so dense it defies screenshots, so stable it echoes real CPUs.  
> Built one gate at a time | and every gate taught us growth.

---

## 📜 License

This project is licensed for **educational purposes only**.  
Commercial reuse or redistribution is not allowed without prior permission.

---


# 22-bit-mini-computer
# 🖥️ 22-bit Mini Computer in Logisim

This is a **22-bit Mini Computer** designed and implemented in **Logisim** as part of the **CSE 2114: Computer Architecture** course in **Semester 2-1** at **KUET**.  
It features a custom datapath, control unit, and an instruction set architecture (ISA) supporting key arithmetic, logic, memory, and control operations.

## 📌 Project Overview

This mini computer mimics the architecture of a basic CPU, designed from scratch using logic gates, multiplexers, registers, memory units, and a control unit.  
It executes instructions via the **fetch-decode-execute** cycle and supports both arithmetic/logical and control flow operations.

---

## 🧠 Instruction Set Architecture (ISA)

The CPU supports the following operations:

| Opcode | Instruction     | Description                        |
|--------|------------------|------------------------------------|
| 0000   | AND              | Bitwise AND between AC and memory |
| 0001   | ADD              | Add memory content to AC          |
| 0010   | STORE            | Store AC to memory                |
| 0011   | ISZ              | Increment memory; skip if zero    |
| 0100   | BSB              | Branch to subroutine              |
| 0101   | BUN              | Unconditional jump                |
| 0110   | LOAD             | Load memory into AC               |
| 0111   | HALT             | Stop execution                    |
| 1000   | OR               | Bitwise OR between AC and memory |
| 1001   | SUB              | Subtract memory from AC           |
| 1010   | INC              | Increment AC                      |
| 1011   | DEC              | Decrement AC                      |

---

## ⚙️ Components

- **Program Counter (PC)** – Holds the address of the next instruction
- **Instruction Register (IR)** – Stores the current instruction
- **Memory Address Register (MAR)** – Points to the memory location being accessed
- **Accumulator (AC)** – Main register for ALU operations
- **Data Register (DR)** – Temporarily stores data
- **ALU (Arithmetic Logic Unit)** – Performs arithmetic and logic operations
- **Control Unit** – Generates control signals based on opcodes
- **Main Memory** – Stores instructions and data

---

## 🔄 Instruction Cycle

1. **Fetch** – PC sends address to MAR; memory fetches instruction into IR
2. **Decode** – Control unit decodes opcode and sets up control signals
3. **Execute** – Operation is performed by ALU or control logic

---

## 🧾 How to Run

1. Open the `.circ` file using [Logisim](http://www.cburch.com/logisim/)
2. Set the clock input to automatic or manually trigger it
3. Load instructions and data into memory
4. Run the circuit and observe the execution cycle

---

## 🗃️ File Structure



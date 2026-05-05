# Lab 02: Arithmetic Circuits (Adders)
**Student Name:** Rayene rahal and Ahmed guerrah  
**Group:** 03

## 1. Introduction
In this laboratory, I designed and implemented binary adder circuits: the Half Adder and the Full Adder. These circuits are the fundamental building blocks for arithmetic operations in digital systems.

---

## 2. Half Adder
The Half Adder adds two 1-bit binary numbers ($A$ and $B$). It produces two outputs: **Sum (S)** and **Carry (C)**.

### Logic Equations:
- $S = A \oplus B$ (XOR Gate)
- $C = A \cdot B$ (AND Gate)

### Truth Table:
| A | B | Sum (S) | Carry (C) |
|---|---|---------|-----------|
| 0 | 0 |    0    |     0     |
| 0 | 1 |    1    |     0     |
| 1 | 0 |    1    |     0     |
| 1 | 1 |    0    |     1     |

---

## 3. Full Adder
The Full Adder adds three 1-bit binary numbers: $A$, $B$, and an input carry $C_{in}$. It is implemented using two Half Adders and an OR gate.

### Logic Equations:
- $S = (A \oplus B) \oplus C_{in}$
- $C_{out} = (A \cdot B) + (C_{in} \cdot (A \oplus B))$

### Truth Table:
| A | B | Cin | Sum (S) | Cout |
|---|---|-----|---------|------|
| 0 | 0 |  0  |    0    |  0   |
| 0 | 0 |  1  |    1    |  0   |
| 1 | 1 |  0  |    0    |  1   |
| 1 | 1 |  1  |    1    |  1   |

---

## 4. Implementation Screenshots
Below are the screenshots of the circuits designed in Logisim:

### Half Adder Circuit:
![Half Adder](./screenshots/half_adder_case.png)

### Full Adder Circuit:
![Full Adder](./screenshots/full_adder_case.png)

---

## 5. Conclusion
Through this lab, I successfully learned how to build a 1-bit adder and how to chain logic gates to handle carry-over bits in binary addition. All circuits were tested and verified using Logisim.
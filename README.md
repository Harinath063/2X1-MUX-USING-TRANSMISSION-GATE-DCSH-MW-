 # 2x1 Multiplexer using Transmission Gates (DSCH + Microwind)

## 📌 Project Overview

This project demonstrates the design and implementation of a 2×1 Multiplexer (MUX) using transmission gates. The design is created using DSCH for schematic-level simulation and implemented in Microwind for CMOS layout and physical-level simulation.

---

## 🎯 Objective

* To design a 2×1 MUX using transmission gates
* To understand CMOS-based switching using PMOS and NMOS
* To simulate and verify the functionality at both schematic and layout levels

---

## 🧠 Theory

A 2×1 Multiplexer selects one of two input signals based on a select line.

### Logic:

* Output = A when S = 0
* Output = B when S = 1

Transmission gates are used instead of simple pass transistors to ensure full voltage transfer (both logic ‘0’ and ‘1’).

Each transmission gate consists of:

* One NMOS transistor
* One PMOS transistor
* Complementary control signals (S and S̅)

---

## 🛠 Tools Used

* DSCH (Digital Schematic Design)
* Microwind (CMOS Layout Design and Simulation)

---

## ⚙️ Implementation Steps

### Step 1: Design in DSCH

* Create inputs: A, B, Select (S)
* Generate inverted signal S̅ using NOT gate
* Use two transmission gates:

  * TG1 passes A when S = 0
  * TG2 passes B when S = 1
* Connect outputs of both transmission gates to final output

### Step 2: Simulation in DSCH

* Apply different input combinations
* Verify correct output switching based on select line

### Step 3: Layout in Microwind

* Implement CMOS layout using PMOS and NMOS
* Ensure correct connections for transmission gates
* Maintain proper routing using metal and poly layers

### Step 4: Simulation in Microwind

* Run simulation
* Verify output behavior and switching delay

---

## 📊 Truth Table

| S | Output |
| - | ------ |
| 0 | A      |
| 1 | B      |

---

## 📸 Results

* DSCH schematic simulation verified correct logic
* Microwind layout successfully implemented
* Output waveform matches expected multiplexer behavior

---

## ✅ Advantages

* Provides full voltage swing using transmission gates
* Efficient CMOS implementation
* Reduces signal degradation compared to pass transistor logic

---

## ⚠️ Limitations

* Requires complementary control signal (S̅)
* Slightly more complex than basic gate-level MUX
* Layout design requires careful transistor placement

---

## 🚀 Applications

* Data selection circuits
* Digital communication systems
* Arithmetic and logic units (ALU)
* Signal routing in VLSI systems

---

## 📌 Conclusion

The project successfully demonstrates the design of a 2×1 MUX using transmission gates. It highlights the importance of CMOS design techniques and provides practical exposure to both schematic and layout-level implementation using DSCH and Microwind.


Done by:
V.Venkata Harinath
ECE Diploma 
SVGP TIRUPATI

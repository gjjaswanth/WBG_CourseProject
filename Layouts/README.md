# WBG_CourseProject

## CMOS Logic Gate Layout Design using Magic VLSI

This repository contains custom CMOS layout designs for fundamental digital logic gates created using Magic VLSI as part of a course project.

The project demonstrates the complete physical design flow:

- CMOS layout creation
- Design Rule Checking (DRC)
- Layout extraction
- SPICE netlist generation
- Circuit simulation

---

## Repository Structure

- WBG_CourseProject
  - Layouts
    - Inverter
    - NAND
    - NOR
  - LICENSE
  - README.md
Each gate folder contains:

- .mag file  → Magic layout file  
- .ext file  → Extracted layout file  
- .spice file → SPICE netlist for simulation  

---

## Implemented Gates

### 1. CMOS Inverter (NOT Gate)

- One PMOS (pull-up) and one NMOS (pull-down)
- DRC verified
- Extracted and converted to SPICE

Function:
Y = A'

---

### 2. 2-Input NAND Gate

- Parallel PMOS in pull-up network
- Series NMOS in pull-down network
- DRC clean layout
- Extracted SPICE netlist generated

Function:
Y = (A · B)'

---

### 3. 2-Input NOR Gate

- Series PMOS in pull-up network
- Parallel NMOS in pull-down network
- Layout verified using DRC
- SPICE netlist generated for simulation

Function:
Y = (A + B)'

---

## Tools Used

- Magic VLSI for layout design and DRC
- extract command in Magic for layout extraction
- ext2spice for SPICE netlist generation
- SPICE simulator for verification

---

## How to Use

1. Navigate to the required gate folder.
2. Open the layout in Magic:

   magic filename.mag

3. Run DRC:

   drc check

4. Extract layout:

   extract all
   ext2spice

5. Simulate the generated .spice file in any SPICE simulator.

---

## Learning Objectives

- Understanding CMOS pull-up and pull-down networks
- Physical layout design concepts
- Design Rule Checking (DRC)
- Layout extraction process
- SPICE simulation workflow

---

## License

This project is licensed under the MIT License.
See the LICENSE file for details.

---

## Author

Jaswanth  
B.Tech – Electrical and Computer Engineering  
VLSI Layout Design Course Project

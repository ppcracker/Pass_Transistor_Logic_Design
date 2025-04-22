#Pass Transistor Project
This project is a Pass Transistor implementation and simulation using LTspice.

It includes:

Schematic file (Pass_Transistor.asc)

Netlist file (Pass_Transistor.net)

Simulation setup

README and License files

Project Description
A Pass Transistor is a basic MOSFET-based switch used in digital logic design.
In this project, a PMOS transistor is used to realize a pass gate mechanism.

This simulation demonstrates the behavior of a pass transistor under different input conditions, verifying its switching characteristics using LTspice XVII.

Files Included
Pass_Transistor.asc — Schematic file for LTspice

Pass_Transistor.net — Auto-generated netlist from LTspice

README.md — Documentation

LICENSE — Open source under MIT License

How to Run the Simulation
Open LTspice XVII (or newer).

Open Pass_Transistor.asc schematic file.

(Optional) Regenerate the netlist if needed:

Click on Netlist > Create Netlist.

Run the simulation by clicking the Run button (running man icon).

Probe waveforms by clicking on nodes or nets.

How to Generate Netlist in LTspice
Open your .asc schematic file.

Go to the top menu: View ➔ SPICE Netlist.

Save it manually if you want, or simulate once — LTspice auto-generates the .net file.

Choosing W/L Ratio for PMOS
Typically, for CMOS design, PMOS is made wider than NMOS to balance drive strengths.

Common thumb rule:

𝑊
𝐿
𝑃
𝑀
𝑂
𝑆
≈
2
×
𝑊
𝐿
𝑁
𝑀
𝑂
𝑆
L
W
​
  
PMOS
​
 ≈2× 
L
W
​
  
NMOS
​
 
If your NMOS is, say, W/L = 1 μm/0.18 μm →
Then for PMOS: W/L ≈ 2 μm/0.18 μm.

Exact W/L depends on:

Technology node (e.g., 180 nm, 90 nm, etc.)

Required performance (speed, leakage, power)

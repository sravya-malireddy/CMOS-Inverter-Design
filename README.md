# CMOS Inverter Design using Cadence Virtuoso

A transistor-level CMOS inverter designed and analyzed using Cadence Virtuoso, covering schematic design, circuit simulation, physical layout, and layout verification.

This project was developed to understand the practical flow of custom CMOS digital circuit design and the relationship between transistor-level behavior and physical implementation.

---

## Project Overview

A CMOS inverter is one of the fundamental building blocks of digital integrated circuits.

The project focuses on designing a CMOS inverter using complementary PMOS and NMOS transistors and studying its electrical behavior through simulation and physical implementation.

The design flow covered:

- CMOS inverter schematic design
- DC analysis
- Voltage Transfer Characteristic (VTC)
- Transient analysis
- Physical layout
- Design Rule Check (DRC)
- Layout Versus Schematic (LVS)

The design was implemented using Cadence Virtuoso with a 90 nm technology PDK and a 1.8 V supply.

---

## Design Flow


CMOS Inverter Schematic
          |
          v
      DC Analysis
          |
          v
     VTC Analysis
          |
          v
   Transient Analysis
          |
          v
      Layout Design
          |
          v
         DRC
          |
          v
         LVS
          |
          v
   Verified Layout

   
## Design Specifications
| Parameter      | Details               |
| -------------- | --------------------- |
| Circuit        | CMOS Inverter         |
| Technology     | 90 nm UMC PDK         |
| Supply Voltage | 1.8 V                 |
| PMOS Width     | 1.5 µm                |
| PMOS Length    | 0.18 µm               |
| NMOS Width     | 0.75 µm               |
| NMOS Length    | 0.18 µm               |
| EDA Tool       | Cadence Virtuoso      |
| Simulation     | Spectre / ADE         |
| Layout Tool    | Virtuoso Layout Suite |
| Verification   | DRC, LVS              |

## CMOS Inverter
The inverter consists of a PMOS transistor connected to the supply and an NMOS transistor connected to ground.

The gates of both transistors are connected to the input, while their drains are connected to the output.

              VDD
               |
              PMOS
               |
               +-------- VOUT
               |
              NMOS
               |
              GND

               ^
               |
              VIN
## Logic Operation
| Input | PMOS | NMOS | Output |
| ----- | ---- | ---- | ------ |
| LOW   | ON   | OFF  | HIGH   |
| HIGH  | OFF  | ON   | LOW    |


The complementary operation of the two transistors produces the required logical inversion.

## Schematic Design

The CMOS inverter schematic was created using the Virtuoso Schematic Editor.

The PMOS and NMOS devices were sized to obtain the required inverter characteristics and balanced switching behavior.

## DC Analysis

DC analysis was performed by sweeping the input voltage and observing the corresponding output voltage.

The resulting Voltage Transfer Characteristic (VTC) was used to study the switching behavior of the inverter.

The VTC provides information about:

Logic-high output
Logic-low output
Switching region
Switching threshold
Voltage gain
Noise-margin behavior

## Transient Analysis

Transient analysis was performed using a pulsed input signal to observe the inverter's switching response.

The output waveform was analyzed to understand the dynamic behavior of the CMOS inverter.

<img width="300" height="300" alt="transient-response" src="https://github.com/user-attachments/assets/4d5c3942-86bc-4103-9dcc-c4be9a07830a" />

Important timing characteristics include:

Rise time
Fall time
Propagation delay

## Physical Layout

After schematic-level verification, the physical layout of the CMOS inverter was created using the Virtuoso Layout Suite.

<img width="300" height="500" alt="layout" src="https://github.com/user-attachments/assets/2072b900-658e-4761-98a3-780ea36588bf" />

The layout incorporates the required CMOS layers and physical connections, including:

PMOS region
NMOS region
Polysilicon
Diffusion
Metal interconnects
Contacts
Well connections

## Design Rule Check

Design Rule Check (DRC) was performed to verify that the physical layout satisfies the technology design rules.

DRC checks physical constraints such as:

Minimum spacing
Minimum width
Layer overlaps
Enclosures
Contact placement

A clean DRC indicates that the layout follows the required geometric design rules.

## Layout Versus Schematic

LVS verification was performed to compare the extracted layout connectivity with the original schematic.

The purpose of LVS is to ensure that the physical layout represents the intended schematic circuit.

The verification checks:

Device correspondence
Pin connectivity
Device connections
Overall circuit topology

## Tools Used
Cadence Virtuoso
Virtuoso Schematic Editor
Virtuoso Layout Suite
Analog Design Environment (ADE)
Spectre
90 nm UMC PDK

## Key Learning

This project helped me understand the complete basic flow of custom CMOS digital circuit design.

The main areas of learning were:

CMOS transistor operation
PMOS/NMOS sizing
Voltage Transfer Characteristics
Transient circuit behavior
Custom IC layout
CMOS layout layers
Design-rule verification
Schematic-to-layout verification
Hardware-aware circuit design

One of the most useful aspects of the project was understanding that circuit functionality is only one part of VLSI design. The physical layout must also satisfy technology design rules and maintain the connectivity represented by the schematic.

## Project Structure
CMOS-Inverter-Design/
│
├── README.md
│
├── docs/
│   ├── Project-Report.pdf
│   ├── Presentation.pdf
│   └── IEEE-Paper.pdf
│
├── images/
│   ├── schematic.png
│   ├── testbench.png
│   ├── vtc-curve.png
│   ├── transient-response.png
│   |__ layout.png
│
└── LICENSE

## Future Scope

The project can be extended toward more advanced custom digital IC design by:

Optimizing transistor sizing
Studying power-delay trade-offs
Designing CMOS NAND and NOR gates
Building larger combinational logic blocks
Exploring standard-cell design
Comparing different technology nodes
Designing and analyzing larger CMOS digital circuits
Project Information
Category	Details
Project	CMOS Inverter Design
Domain	VLSI / Custom IC Design
Circuit	CMOS Inverter
Technology	90 nm
Supply	1.8 V
EDA Tool	Cadence Virtuoso
Simulation	Spectre / ADE
Verification	DRC, LVS
Project Type	Academic VLSI Project
Documentation

Detailed project documentation is available in the docs/ directory.

Project Report
Presentation

## Author

Malireddy Sravya Sri

Electronics and Communication Engineering

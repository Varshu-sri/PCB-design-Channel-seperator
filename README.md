**Custom PCB design - Channel separator**

Overview

This project is a beginner-friendly custom PCB designed in Altium Designer for signal separator and distribution applications. The board provides a protected interface between external signal sources and downstream devices such as FPGA development boards, microcontrollers, and test equipment.

The design incorporates a fuse for basic protection, a linear voltage regulator for power conditioning, and a quad AND gate IC used as a signal buffer/distribution stage. Rather than routing signals directly to sensitive hardware, the PCB provides an intermediate interface layer that helps isolate and organize signal connections.

The project includes complete design documentation, including schematic files, PCB layout files, Gerber manufacturing outputs, and photographs of the assembled hardware.

**The board includes:**

DC power input
Fuse protection
Linear voltage regulator
Filter capacitors for power stability

The regulator generates a stable logic supply voltage used by the signal processing circuitry.

**Signal Processing Section**

A quad 2-input AND gate IC is used as the signal routing stage.

One input of every AND gate is permanently connected to the regulated supply voltage.

The second input receives the external signal.

Because one AND gate input remains HIGH, the output follows the incoming signal:

Output = Signal × Logic High
Output = Signal

This configuration allows the logic device to act as an intermediary stage between external equipment and downstream electronics.

**Applications**

The PCB can be used for:

FPGA GPIO interfacing
Signal distribution
Test bench signal routing
Prototype hardware development
Educational digital electronics experiments
Logic-level signal conditioning

**PCB Design Highlights**
Schematic Capture

The schematic was developed in Altium Designer and includes:

Power input stage
Fuse protection
Linear regulator circuit
Quad AND gate interface
Input connectors
Output connectors
PCB Layout

The PCB layout was created with attention to:

Component placement
Signal routing
Manufacturability
Through-hole assembly
Ease of debugging and testing
Assembly

After fabrication, the board was manually assembled using through-hole components.

Images of the populated board are included in the repository.

**Results**

The fabricated PCB was successfully assembled and verified.

Testing confirmed:

Proper voltage regulation
Correct signal propagation through all channels
Stable operation of the logic circuitry
Reliable signal routing between input and output headers
Learning Outcomes

This project provided hands-on experience with:

Electronic schematic design
Component selection
PCB layout techniques
Gerber generation
PCB manufacturing workflow
Through-hole soldering and assembly
Hardware validation and debugging
Repository Contents

**This repository contains:**

Altium schematic files
PCB layout files
Gerber manufacturing files
Assembly images
Design documentation
Author

Varsha Sri
FPGA Engineer | Embedded Systems Engineer | PCB Design Enthusiast

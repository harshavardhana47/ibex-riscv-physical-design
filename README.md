# ibex-riscv-physical-design
Open-source physical design implementation of the Ibex RISC-V core using OpenROAD-flow-scripts and the SKY130HD technology, covering synthesis, floorplanning, power planning, placement, CTS, routing, timing analysis, signoff, and GDSII generation.

## Technology

- PDK: SKY130
- Standard Cell Library: SKY130HD
- Technology Node: 130 nm
- Target Design: Ibex RISC-V Core

## Tools

- OpenROAD
- OpenROAD-flow-scripts
- Yosys
- KLayout
- Docker
- WSL2 / Ubuntu

## Physical Design Flow

RTL
 ↓
Synthesis
 ↓
Floorplanning
 ↓
Power Planning
 ↓
Placement
 ↓
CTS
 ↓
Routing
 ↓
Signoff
 ↓
GDSII

## Key Inputs

- RTL/SystemVerilog
- SDC
- Liberty (.lib)
- LEF
- Technology LEF (.tlef)

## Key Outputs

- Synthesized netlist
- Floorplan
- Placement database
- CTS results
- Routed design
- Timing reports
- DRC/LVS results
- GDSII

## Results

Project in progress, results will be eventually added.

# 8×1 Multiplexer using Verilog

## Overview

This project implements an **8×1 Multiplexer (MUX)** in Verilog HDL. An 8×1 multiplexer selects one of eight input signals based on a 3-bit select line and forwards the selected input to the output.

## Truth Table

| Select (S2 S1 S0) | Output (Y) |
|-------------------|------------|
| 000 | I0 |
| 001 | I1 |
| 010 | I2 |
| 011 | I3 |
| 100 | I4 |
| 101 | I5 |
| 110 | I6 |
| 111 | I7 |

## Inputs

- `I[7:0]` – Eight data inputs
- `S[2:0]` – 3-bit select signal

## Output

- `Y` – Selected output

## Project Structure

```
8x1-multiplexer-verilog/
├── src/
├── tb/
├── sim/
├── images/
└── README.md
```

## Simulation

Compile:

```bash
iverilog -o mux src/mux8x1.v tb/mux8x1_tb.v
```

Run:

```bash
vvp mux
```

Open waveform:

```bash
gtkwave mux8x1.vcd
```

## Applications

- Data routing
- Bus switching
- Processor datapaths
- Communication systems
- FPGA and ASIC designs

## License

MIT Licenses
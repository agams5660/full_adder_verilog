# 1-bit Full Adder in Verilog

## Overview

This project implements a 1-bit Full Adder using Verilog HDL.

A Full Adder adds three 1-bit inputs (`A`, `B`, and `Cin`) and produces two outputs:
- `Sum`
- `Carry Out (Cout)`

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
|0|0|0|0|0|
|0|0|1|1|0|
|0|1|0|1|0|
|0|1|1|0|1|
|1|0|0|1|0|
|1|0|1|0|1|
|1|1|0|0|1|
|1|1|1|1|1|

## Files

- `full_adder.v` – RTL design
- `tb_full_adder.v` – Testbench

## How to Run

```bash
iverilog -o sim full_adder.v tb_full_adder.v
vvp sim
gtkwave full_adder.vcd
```

## Tools Used

- Icarus Verilog
- GTKWave
- VS Code
- Ubuntu (WSL)

## Author

Agam Sharma
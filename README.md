# 4-bit ALU in Verilog HDL

A 4-bit Arithmetic Logic Unit (ALU) designed using **Verilog HDL** with a hierarchical and modular approach. 

## Features

- Structural Half Adder and Full Adder
- 4-bit Ripple Carry Adder/Subtractor
- Arithmetic Operations
  - Addition
  - Subtraction
- Logical Operations
  - AND
  - OR
  - XOR
  - NOT
- Shift Operations
  - Left Shift
  - Right Shift
- Multiplication
- Division (with divide-by-zero handling)
- Status Flags: Carry (C), Overflow (V), Zero (Z), Negative (N)


Flag Behavior
- C (Carry) — Set on unsigned overflow for addition, or borrow for subtraction (inverted carry-out).
- Z (Zero) — Set when the result is all zeros.
- N (Negative) — Reflects the sign bit (MSB) of the result.
- V (Overflow) — Set on signed overflow, detected via XOR of carry-in and carry-out of the MSB stage.

Flags are only meaningful for **addition and subtraction**; logical, shift, multiply, and divide operations do not currently update them.

## Supported Operations

| Opcode | Operation |
|--------|-----------|
| 0000 | Addition |
| 0001 | Subtraction |
| 0010 | AND |
| 0011 | OR |
| 0100 | XOR |
| 0101 | NOT |
| 0110 | Left Shift |
| 0111 | Right Shift |
| 1000 | Multiplication |
| 1001 | Division |


## Simulation

- Directed Verilog testbench
- 11 Test Cases
- All tests passed successfully


## Tools Used

- Verilog HDL
- Xilinx Vivado 2025.2
- Git
- GitHub

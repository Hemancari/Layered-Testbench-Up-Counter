# Layered-Testbench-Up-Counter
# SystemVerilog Layered Testbench for a 4-Bit Synchronous Up Counter

## NAME
Heman Cariappa

## SRN
PES2UG24EC039

## Project Overview

This project implements a modular, layered verification environment using SystemVerilog to verify the functionality of a 4-bit synchronous up counter.

The testbench follows a layered architecture, separating stimulus generation, DUT interaction, signal monitoring, and output checking to achieve structured and reusable verification.

## Design Under Test (DUT)

The DUT is a 4-bit synchronous up counter with the following specifications:

- 4-bit output (`Q[3:0]`)
- Active-high synchronous reset
- Increments by 1 on every active clock edge
- Counts from 0 to 15
- Automatically wraps around to 0 after reaching 15

## Testbench Architecture

The verification environment consists of the following components:

1. **Transaction:** Defines the input stimulus and transaction data.
2. **Generator:** Generates randomized or directed test transactions.
3. **Driver:** Drives the generated stimulus to the DUT.
4. **Monitor:** Observes DUT signals and captures output transactions.
5. **Scoreboard:** Compares the DUT output against the expected counter value.
6. **Environment:** Instantiates and connects the testbench components.
7. **Top-Level Testbench:** Instantiates the DUT and verification environment.

## Verification Features

- Counter increment verification
- Synchronous reset verification
- Overflow and rollover verification (15 → 0)
- Expected versus actual output comparison
- Modular and reusable testbench architecture

## Language and Tools

- **Language:** SystemVerilog
- **Simulation:** [Add your simulator name, e.g., QuestaSim / ModelSim / Vivado]

## Objective

To verify the functional correctness of a 4-bit synchronous up counter using a modular layered SystemVerilog testbench, demonstrating fundamental concepts of functional verification and testbench architecture.

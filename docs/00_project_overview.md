# Project Overview

This project is a single-phase shunt active power filter (SAPF) for a 48 V AC bus.

## System Architecture

- The mains grid (e.g. 230 V, 50 Hz) is stepped down to 48 V AC using a transformer.
- A nonlinear load (single-phase diode bridge + DC capacitor + DC resistor) is connected to the 48 V bus.
- A shunt active power filter is connected in parallel with the load at the 48 V bus.
- The SAPF consists of:
  - H-bridge voltage-source inverter
  - DC-link capacitor
  - Filter inductor between inverter and point of common coupling (PCC)
- The controller measures currents and voltages and generates gating signals for the H-bridge to compensate harmonics.

## Goals

- Compensate up to 2 A of nonlinear/harmonic current drawn by the load.
- Make the source current approximately sinusoidal and in phase with the grid voltage.
- Reduce source current THD to a specified target (e.g. below 5–8%) and improve power factor.
- Implement the same controller structure later on an STM32 microcontroller.

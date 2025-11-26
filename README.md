# Single-Phase Shunt Active Power Filter (48 V)

This project implements a single-phase shunt active power filter (SAPF) for a 48 V AC system (derived from the mains using a transformer).

- Compensates up to 2 A of harmonic/reactive current from a nonlinear load (diode bridge + C + R).
- Uses an H-bridge voltage-source inverter, DC-link capacitor, and filter inductor.
- Control strategy: DC-link voltage PID control + hysteresis current control.
- Target platform: STM32 microcontroller (controller logic first developed in Simulink, then ported to firmware).

The repository is organized to be easy to follow step-by-step from simulation to implementation.

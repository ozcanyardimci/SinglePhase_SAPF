# Requirements and Specifications

## Electrical Specifications (Initial)

| Item                              | Symbol | Value (initial)            | Notes                       |
|-----------------------------------|--------|----------------------------|-----------------------------|
| Grid primary voltage              | Vpri   | 230 V RMS, 50 Hz (example) | mains side                  |
| Secondary / test bus voltage      | Vsec   | 48 V RMS                   | after transformer           |
| Max compensation current (RMS)    | Icomp  | 2 A                        | APF rating                  |
| Nonlinear load type               | –      | Diode bridge + C + R       | single-phase rectifier load |
| Target source current THD (after) | THD_s  | e.g. 5–8 %                 | to be refined               |
| Target power factor (after)       | PF_s   | e.g. > 0.95                | near unity                  |
| DC-link nominal voltage (sim)     | Vdc    | 80–100 V (initial guess)   | refine in later phases      |
| Control method                    | –      | PID (Vdc) + hysteresis     | STM32 implementation later  |

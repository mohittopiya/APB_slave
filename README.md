# APB Slave Design and Verification

This repository contains the complete RTL design and verification setup for an **APB Slave** module compliant with the **AMBA APB 2.0** protocol. The design includes a built-in watchdog timer that raises an error (`PSLVERR`) if the protocol is not followed correctly, such as when `PENABLE` is not asserted within 10 clock cycles.

> The RTL is parameterized for both address and data widths, making it easy to scale and reuse across different APB-based systems.

## Project Structure

- `RTL/` – Contains the Verilog source file for the APB Slave design  
- `TB/` – Contains the testbench for protocol verification and error handling  
- `SIM/` – Stores simulation outputs, logs, and result files  
- `SIM/makefile` – Automation for compilation, simulation, and coverage  
- `SIM/APB_SLAVE_code_coverage/` – Code coverage report directory  
- `SIM/terminal_output.txt` – Simulation output for testbench run  
- `SIM/wave.do` – Waveform configuration file  
- `SIM/APB_slave_schematic.sch` – Graphical schematic of the RTL design  

## Tools Used

- **Mentor Graphics QuestaSim** – Used for simulation, waveform viewing, and functional coverage analysis

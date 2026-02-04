# Traffic Light Controller (FPGA)

## Overview
This repository contains a Verilog-based digital design for a Traffic Light Controller. The project is implemented using Xilinx Vivado and targets the Zynq UltraScale+ MPSoC architecture. It features a Finite State Machine (FSM) to control traffic signal timing and includes a testbench for verification.

## Project Details
- **Project Name:** Traffic_Light
- **Language:** Verilog
- **IDE:** Xilinx Vivado 2025.1
- **Target Device:** Zynq UltraScale+ (`xczu3eg-sbva484-2-e`)

## File Structure
The project directory is organized as follows:

- **`sources_1/new/traffic_light.v`**: The main top-level module containing the traffic light control logic and state machine.
- **`sim_1/new/Test.v`**: The testbench file used to simulate and verify the signal timing and state transitions.
- **`Traffic_Light.xpr`**: The main Vivado project file.

## Getting Started

### Prerequisites
- **Software:** Xilinx Vivado 2025.1 or later.
- **Hardware (Optional):** Xilinx Zynq UltraScale+ Evaluation Board (or compatible hardware using the `xczu3eg` part).

### How to Open
1. Clone this repository to your local machine.
2. Open **Vivado 2025.1**.
3. Select **Open Project** and navigate to `Traffic_Light.xpr`.
4. Allow Vivado to refresh the IP and block design if requested.

## Simulation
To verify the traffic sequences:
1. Open the project in Vivado.
2. In the **Flow Navigator**, click on **Simulation** > **Run Simulation**.
3. Select **Run Behavioral Simulation**.
4. Observe the waveforms for the Red, Yellow, and Green signals defined in `Test.v`.

## Synthesis & Implementation
To generate the bitstream for the FPGA:
1. Click **Run Synthesis** in the Flow Navigator.
2. Upon success, click **Run Implementation**.
3. Finally, click **Generate Bitstream** to create the `.bit` file for programming.

## License
This project is open-source and available for educational and personal use.

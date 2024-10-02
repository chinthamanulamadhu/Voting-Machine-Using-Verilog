# Verilog Voting Machine Project
https://www.edaplayground.com/x/Qxvc

## Overview
This project implements a simple **Voting Machine** using **Verilog**. The design tracks votes for three candidates and allows votes to be reset. The machine counts the number of votes for each candidate based on user input and outputs the current count for each.

The project includes:
- `voting_machine.v`: The Verilog module for the voting machine logic.
- `tb_voting_machine.v`: The testbench to simulate and verify the functionality of the voting machine.

## Features
- Supports voting for three candidates.
- Keeps track of votes using a simple counter.
- Votes can be reset using the reset signal (`rst`).
- Verilog testbench provided for simulation.

## Files
- **voting_machine.v**: The main Verilog module for the voting machine.
- **tb_voting_machine.v**: The testbench module to test the voting machine.

## How to Run the Project

### 1. Simulate using EDA Playground:
1. Visit [EDA Playground](https://www.edaplayground.com/).
2. Copy and paste the `voting_machine.v` and `tb_voting_machine.v` into the respective sections.
3. Select **Icarus Verilog** as the simulator.
4. Run the simulation to verify the functionality.

### 2. Simulate Locally:
If you prefer to run the simulation locally, you can use tools like **Xilinx Vivado**, **ModelSim**, or **Icarus Verilog**:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/verilog-voting-machine.git

Use your preferred simulation tool to load voting_machine.v and tb_voting_machine.v.
Run the simulation to observe the vote counting process.
3. Generate Waveform:
To visualize the waveforms using GTKWave or any other VCD viewer:

Ensure the $dumpfile and $dumpvars commands are included in your testbench.
Run the simulation to generate a .vcd file.
Open the .vcd file in GTKWave to analyze the waveforms.
Example Output
You should see the following key events in the waveform:

![Screenshot 2024-10-02 191019](https://github.com/user-attachments/assets/7230471f-9568-4ae3-99a9-1f1419baa1e0)


Clock (clk): Continuous clock signal.
Reset (rst): Resets the vote counts to zero.
Vote Inputs (vote_C1, vote_C2, vote_C3): Pulses when a vote is cast.



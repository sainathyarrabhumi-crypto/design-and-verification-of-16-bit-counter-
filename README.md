16-bit Counter Design and Verification
📌 Project Overview

This project implements and verifies a 16-bit synchronous counter in SystemVerilog. The goal is to ensure functional correctness of the design through directed and random stimulus.

🛠️ Features

16-bit counter (0 to 65535)

Supports:

Reset

.Enable control

.Up-counting mode

.Verification environment built in SystemVerilog
├── rtl/
│   └── counter16.v           # 16-bit Counter RTL
├── tb/
│   ├── counter_tb.sv         # Testbench top
│   ├── stimulus_gen.sv       # Random/directed stimulus generator
│   ├── monitor.sv            # Output monitor
│   ├── scoreboard.sv         # Self-checking scoreboard
├── waves/
│   └── simulation.vcd        # Sample waveform dump
├── docs/
└── README.md                 # Project description
📊 Verification Methodology

Stimulus: Random and directed testcases

Scoreboard: Compares DUT output against reference model

Coverage:

Reset behavior

Enable functionality

Counter wrapping at max value (65535 → 0)

✅ Results

Counter functionality verified for:

Reset (proper initialization)

Enable/disable behavior

Correct counting sequence including rollover



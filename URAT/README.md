markdown# Synthesizable UART Design Core (Verilog HDL)

A robust, modular **Universal Asynchronous Receiver-Transmitter (UART)** communication interface module tailored for FPGA and ASIC design pipelines.

## 📁 Repository Overview
* `rtl/uart_tx.v` - Serial Transmit hardware engine
* `rtl/uart_rx.v` - Serial Receive data reconstructor
* `tb/uart_tb.v` - Automated validation testbench script

## 🚀 Execution Guide
Compile, emulate, and analyze hardware state routing directly from your command line:

```bash
# 1. Hardware compilation via EDA tools
iverilog -o build_target.out rtl/*.v tb/*.v

# 2. Run simulation engine 
vvp build_target.out

# 3. Open behavioral waveforms 
gtkwave uart_simulation.vcd
```


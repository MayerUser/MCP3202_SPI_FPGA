# CMODA7_Demo_MCP3202_SPI_Verilog

This is FPGA SPI ADC demo project for DSL, which using CMOD A7 as the development board. The MCP3202 Dual Channel FPGA was selected as ADC in this application which provide the demo Verilog Code to drive MCP3202

## Getting Started

- MCP3202 Protocol Detail:
* Inputs:
1. - rstn: Active low reset signal.
2. - clk: Clock signal.
3. - ap_ready: Signal indicating the host is ready for data processing.
4. - mode: 2-bit input to select the ADC channel and configuration.
5. - port_din: Serial data input from the ADC.

* Outputs:
1. - ap_vaild: Signal that indicates valid data is available.
2. - data: 12-bit output holding the ADC conversion result.
3. - port_dout: Serial data output to the ADC.
4. - port_clk: Clock signal for the ADC.
5. - port_cs: Chip select signal for the ADC, active low.

### MCP3202 Operation Mode
* SINGLE_CHAN0  = 2'b10; - CHANNEL 0;
* SINGLE_CHAN1  = 2'b11; - CHANNEL 1;
* DIFFER_CHAN01 = 2'b00;  - DIFFERENTIAL CHANNEL 01
* DIFFER_CHAN10 = 2'b01;  - DIFFERENTIAL CHANNEL 10

## Prerequisites

* Vivado 2023.1;
* CMOD A7-35T Board File;

## MCP3202 Simulation Result
The following figure is the simulation result of MCP3202 SPI protocol.
![MCP3202 SPI protocol Simulation Result](./Figure/SPI_Simulation.jpg)

## Reference

MCP3202 Dataset:
https://www.farnell.com/datasheets/1669376.pdf

CMOD A7 Reference Page:
https://digilent.com/reference/programmable-logic/cmod-a7/start
 
## License
This project is licensed under the MIT License
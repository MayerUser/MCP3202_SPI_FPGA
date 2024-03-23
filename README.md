# MCP3202_SPI_FPGA
This is FPGA SPI ADC demo project for DSL, which using CMOD A7 as the development board. The MCP3202 Dual Channel FPGA was selected as ADC in this application which provide the demo Verilog Code to drive MCP3202

# Environement
* Vivado 2023.1;
* CMOD A7-35T;

# MCP3202 Operation Mode
* SINGLE_CHAN0  = 2'b10; - CHANNEL 0;
* SINGLE_CHAN1  = 2'b11; - CHANNEL 1;
* DIFFER_CHAN01 = 2'b00;  - DIFFERENTIAL CHANNEL 01
* DIFFER_CHAN10 = 2'b01;  - DIFFERENTIAL CHANNEL 10
 
# Reference
https://www.farnell.com/datasheets/1669376.pdf


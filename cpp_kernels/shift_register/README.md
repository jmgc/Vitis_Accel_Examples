Shift Register (C)
======================

This example demonstrates how to shift values in registers in each clock cycle

***KEY CONCEPTS:*** Kernel Optimization, Shift Register, FIR

***KEYWORDS:*** #pragma HLS ARRAY_PARTITION

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_u200_qdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u200_xdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u250_qdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u250_xdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u280_xdma|Xilinx Alveo U280|VITIS 2019.2
xilinx_u50_xdma|Xilinx Alveo U50|VITIS 2019.2
zc702_base|Xilinx Zynq-7000 SoC ZC702|VITIS 2019.2
zc706_base|Xilinx Zynq-7000 SoC ZC706|VITIS 2019.2
zcu102_base|Xilinx UltraScale+ MPSoC ZCU102|VITIS 2019.2
zcu104_base|Xilinx UltraScale+ MPSoC ZCU104|VITIS 2019.2


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/fir_naive.cpp
src/fir_shift_register.cpp
src/host.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./host <fir XCLBIN>
```


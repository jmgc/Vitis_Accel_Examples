Vadd 2 Kernels (RTL)
======================

This example has two RTL Kernels. Both Kernel_0 and Kernel_1 perform vector addition. The Kernel_1 reads the output from Kernel_0 as one of two inputs.

***KEY CONCEPTS:*** Multiple RTL Kernels

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
src/host.cpp
src/ip_0/hdl/krnl_vadd_rtl_0.v
src/ip_0/hdl/krnl_vadd_rtl_adder.sv
src/ip_0/hdl/krnl_vadd_rtl_axi_read_master.sv
src/ip_0/hdl/krnl_vadd_rtl_axi_write_master.sv
src/ip_0/hdl/krnl_vadd_rtl_control_s_axi.v
src/ip_0/hdl/krnl_vadd_rtl_counter.sv
src/ip_0/hdl/krnl_vadd_rtl_int.sv
src/ip_1/hdl/krnl_vadd_rtl_1.v
src/ip_1/hdl/krnl_vadd_rtl_adder.sv
src/ip_1/hdl/krnl_vadd_rtl_axi_read_master.sv
src/ip_1/hdl/krnl_vadd_rtl_axi_write_master.sv
src/ip_1/hdl/krnl_vadd_rtl_control_s_axi.v
src/ip_1/hdl/krnl_vadd_rtl_counter.sv
src/ip_1/hdl/krnl_vadd_rtl_int.sv
src/kernel_0.xml
src/kernel_1.xml
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./host <vadd XCLBIN>
```


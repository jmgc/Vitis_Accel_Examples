Kernel Chain Matrix Multiplication (C)
======================

This is a kernel containing the cascaded Matrix Multiplication using dataflow. ap_ctrl_chain is enabled for this kernel to showcase how multiple enqueue of Kernel calls can be overlapped to give higher performance. ap_ctrl_chain allow kernel to start processing of next kernel operation before completing the current kernel operation.

***KEY CONCEPTS:*** ap_ctrl_chain, PLRAM

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_u200_qdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u200_xdma|Xilinx Alveo U200|VITIS 2019.2
xilinx_u250_qdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u250_xdma|Xilinx Alveo U250|VITIS 2019.2
xilinx_u280_xdma|Xilinx Alveo U280|VITIS 2019.2


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/host.cpp
src/krnl_chain_mmult.cpp
src/krnl_mmult.hpp
src/krnl_simple_mmult.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./vadd_mmult <krnl_mmult XCLBIN>
```


# FPGA hardware emulation using Layer-specific architecture and tiled pooling

# Introduction

# Build Setup
```
git clone https://github.com/aws/aws-fpga.git $AWS_FPGA_REPO_DIR
```
![image](https://user-images.githubusercontent.com/75317393/147209223-7721f322-4cbc-4df4-9a30-1d08d6a542f4.png)
```
cd $AWS_FPGA_REPO_DIR
source vitis_setup.sh
source /opt/Xilinx/Vitis_HLS/2021.1/settings64.sh
cd $VITIS_DIR/examples/xilinx/hello_world
```
Put Code(ccn.h, ccn.cpp, host.cpp) in src folder

# Branches

# FPGA Evaluation
```
make clean (or cleanall)
make run TARGET=sw_emu DEVICE=$AWS_PLATFORM all
make run TARGET=hw_emu DEVICE=$AWS_PLATFORM all
make run TARGET=hw DEVICE=$AWS_PLATFORM all
```

# Varying the Number of Convolvers

# Kown Issues and Bugs

# FPGA hardware emulation using Layer-specific architecture and tiled pooling

# Introduction

# Build Setup
This build takes place in the hello_world folder.
So, the name of the folder is hello_world.   
If you want to build in a different folder, create a new folder and edit the contents of the Makefile.
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

# FPGA Evaluation 
## (sw_emu)
```
make clean (or cleanall)
make run TARGET=sw_emu DEVICE=$AWS_PLATFORM all
```

## (hw_emu)
```
make clean (or cleanall)
make run TARGET=hw_emu DEVICE=$AWS_PLATFORM all
```

## (hw)
```
make clean (or cleanall)
make run TARGET=hw DEVICE=$AWS_PLATFORM all
```

# Results
> without zeropadding
**1. Layer 1**   
**2. Layer 2**   
**3. Layer 3**   
**4. Layer 4**   
**5. Layer 5**   

> with zeropadding
**1. Layer 1**   
**2. Layer 2**   
**3. Layer 3**   
**4. Layer 4**   
**5. Layer 5**   

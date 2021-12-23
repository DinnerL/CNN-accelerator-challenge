# FPGA hardware emulation using Layer-specific architecture and tiled pooling

# Introduction
![image](https://user-images.githubusercontent.com/75317393/147212779-f24964b7-eff8-4abb-9941-a2b030708a42.png)

![image](https://user-images.githubusercontent.com/75317393/147212751-b8c23d66-5977-4312-a23f-921462a439c2.png)

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
## sw_emu
```
make clean (or cleanall)
make run TARGET=sw_emu DEVICE=$AWS_PLATFORM all
```

## hw_emu
```
make clean (or cleanall)
make run TARGET=hw_emu DEVICE=$AWS_PLATFORM all
```

## hw
```
make clean (or cleanall)
make run TARGET=hw DEVICE=$AWS_PLATFORM all
```

# Results
**without zeropadding**   
+ Layer 1      

+ Layer 2

+ Layer 3   
![(without zeropadding) layer3 hw_emu](https://user-images.githubusercontent.com/75317393/147213590-9568f8ae-7681-40f3-a469-8d0248ad7043.png)   

+ Layer 4   
![(without zeropadding) layer4 sw_emu](https://user-images.githubusercontent.com/75317393/147213559-fad5a619-1acb-4c76-a5c8-a93ad7a6003c.png)   


+ Layer 5    
![(without zeropadding) layer5 hw_emu](https://user-images.githubusercontent.com/75317393/147213544-d97d0a3d-c213-4850-9c49-ca37d313c931.png)   


**with zeropadding**   
+ Layer 1      

+ Layer 2

+ Layer 3

+ Layer 4

+ Layer 5   
![(with zeropadding) layer5 hw_emu](https://user-images.githubusercontent.com/75317393/147213624-a6de096b-b2c3-475e-8083-afccaad8d407.png)



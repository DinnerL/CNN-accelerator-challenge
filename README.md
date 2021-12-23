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
![(without zeropadding) layer1 hw_emu](https://user-images.githubusercontent.com/75317393/147214144-d34c132c-5431-4d45-8668-5538711305d5.png)   

+ Layer 2

+ Layer 3   
![(without zeropadding) layer3 hw_emu](https://user-images.githubusercontent.com/75317393/147214157-e8a13cdf-02ec-4865-8189-9c09ba4d8be9.png)   

+ Layer 4   
 ![(without zeropadding) layer4 hw_emu](https://user-images.githubusercontent.com/75317393/147214182-d6d7b342-5ca5-4533-8bb8-cf85c4eb155f.png)   

+ Layer 5    
![(without zeropadding) layer5 hw_emu](https://user-images.githubusercontent.com/75317393/147214089-2ac8a026-df14-4b90-a9df-8a40fa343cd0.png)   

**with zeropadding**   
+ Layer 1      

+ Layer 2

+ Layer 3

+ Layer 4

+ Layer 5   
![(with zeropadding) layer5 hw_emu](https://user-images.githubusercontent.com/75317393/147214330-090e878e-4795-4e08-a87c-7db54f2cca5b.png)   




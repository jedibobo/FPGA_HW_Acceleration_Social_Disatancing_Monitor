# FPGA_HW_Acceleration_Social_Disatancing_Monitor
 Social Disatancing Monitor using yolov3 and DPU HW acceleration for Xilinx adaptive computing challenge 2020

Hardware layout：

![layout](https://github.com/jedibobo/FPGA_HW_Acceleration_Social_Disatancing_Monitor/blob/main/img/layout.jpg)

Image test for functionality：

<img src="https://github.com/jedibobo/FPGA_HW_Acceleration_Social_Disatancing_Monitor/blob/main/img/image-20201129111317248.png" width="800" align="center">

# How to reproduce this project

You should follow the steps below to reproduce it.

1. Download PYNQ image v2.5 from https://github.com/Avnet/Ultra96-PYNQ/releases .
2. Image the SD card and boot the device, with USB camera attached, USB to Ethernet adapter to connect to Internet and a mini-DP to DP cable connecting to a Monitor.
3. Follow the instructions on DPU-PYNQ page to set up the examples([Xilinx/DPU-PYNQ: DPU on PYNQ (github.com)](https://github.com/Xilinx/DPU-PYNQ)) by getting all the notebooks, go to this page([DPU-PYNQ/README.md at master · Xilinx/DPU-PYNQ (github.com)](https://github.com/Xilinx/DPU-PYNQ/blob/master/host/README.md)) , and download the .hwh file for Ultra96v2 to employ DPU acceleration.
4. Run the dpu_yolo_v3.ipynb example project and make sure there is no warnings or errors when executing this ipynb file.
5. Shift to this project, run one by one and you will get the right results. 

If there is one python package missing, please install it on your own. (for I almost forget when I install the other used packages that are not installed when installing dpu-pynq)

# TO DO

1. improve performance from Hardward(utilize more hardware resources like resize and more powerful DPU) and Software(reading USB camera is I/O block job).
2. 

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=jedibobo/FPGA_HW_Acceleration_Social_Disatancing_Monitor&type=Date)](https://star-history.com/#jedibobo/FPGA_HW_Acceleration_Social_Disatancing_Monitor&Date)

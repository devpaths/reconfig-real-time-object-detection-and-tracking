# Reconfigurable real-time object detection and tracking

Object tracking and detection is a prominent area of research in Computer Vision and Image Processing. Traditionally, Object tracking and detection methods rely more on fixed algorithms and hardware architecture, which are limited in their ability to adapt to changing scenarios and real time requirements. To address these limitations, we propose a system which is designed to detect objects in real-time and can be customized to detect different types of objects. The system is implemented on the Xilinx ZynQ Ultrascale+ board, which provides both FPGA and ARM-based processing units. The FPGA is used to accelerate the computationally intensive tasks, while the ARM processor is used for system control and communication. The system uses a pre-trained CNN model for object detection, which is loaded onto the FPGA at runtime. The FPGA-based implementation of the CNN provides high throughput and low latency compared to traditional software-based implementations. The proposed system is evaluated using a dataset of images and achieves high accuracy in object detection. The results demonstrate that the proposed system is an effective and efficient solution for real-time object detection applications.

## PYNQ-Z2 Setup Guide

### Prerequisites :

- PYNQ-Z2 board

- Computer with compatible browser (Supported Browsers)

- Ethernet cable

- Micro USB cable

- Micro-SD card with preloaded image, or blank card (Minimum 8GB recommended)

### PYNQ Z2 BOARD FEATURES :

PYNQ-Z2 board integrates USB and Ethernet to connect to internet, HDMI Input/Output, MIC
Input, Audio Output, Arduino interface, Raspberry Pi interface, 2 Pmod, user LED, pushbuttons, switches, MicroSD Slot, Power In port for direct power connection, a Jumper for power
source selection and another jumper to select Boot Mode.
It is intended to be easily extensible with Pmod, Arduino, and peripherals, along with generalpurpose GPIO pins.

### MicroSD CARD SETUP :

You can download the pre-compiled PYNQ-Z2 image using the link
http://www.pynq.io/board.html. Connect the microSD card to a PC/Laptop. Open Win32Disk
Imager application, select the downloaded pynq image, and click on the write button. This will
transfer the pynq image to SD card.

### BOARD SETUP :

- Set the boot jumper to SD card.
- Set the power jumper to power the board from USB.
- Insert the SD card loaded with pynq image.
- Connect MicroUSB cable to PROG-UART port of the board and USB port to your PC/Laptop.
- Connect Ethernet cable to a PC or to a Router.
- Turn ON the board which will immediately glow the Red LED to indicate that the board has power and then the Done LED will turn ON to confirm that the device is working. Finally, 2 Blue LEDs and four Green LEDs will light up to show that the device is booted and ready to use.

### NETWORK CONNECTION :

Set the IP address of your PC in the same range as the board by following the below steps :

- Open Control Panel -> Select Network and Internet -> Network and Sharing Center and then click on Ethernet (highlighted below)
- Select Internet Protocol Version 4 and click on properties
- Set the IP Address to 192.168.2.1 and Subnet mask to 255.255.255.0 and click ok.

### CONNECTING TO JUPYTER NOTEBOOK :

Open a web browser and navigate to http://192.168.2.99 to connect to jupyter notebook. You
will be navigated to a login screen if the board setup is completed successfully. Enter Username
xilinx and password xilinx.

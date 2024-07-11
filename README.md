# Arty Z7 Root Repository

## Arty Z7-10 HDMI Input Demo

### Description

This branch contains sources for the Arty Z7-10 HDMI Input Demo.

This project demonstrates how to use the USB-UART Bridge, HDMI Sink, and HDMI Source with the ZYNQ processor. Vivado is used to build the demo's hardware platform, and Vitis is used to program the bitstream onto the board and to build and deploy a C application. Video data streams in through the HDMI in port and out through the HDMI out port. A UART interface is available to configure the platform. There are 3 display frame buffers that the user can choose to display from or write to. The configuration options are shown in the table below.

As the usb-uart bridge is used, the Arty Z7-10 must be connected to a computer over MicroUSB, which must be running a serial terminal (such as Tera Term or PuTTY).

| Option | Function |
| ------ | -------- |
| 1 | Change the resolution of the HDMI output to the monitor. |
| 2 | Change the frame buffer to display on the HDMI monitor. |
| 3/4 | Store a test pattern in the chosen video frame buffer - color bar or blended. |
| 5 | Start/Stop streaming video data from HDMI to the chosen video frame buffer. |
| 6 | Change the video frame buffer that HDMI data is streamed into. |
| 7 | Invert and store the current video frame into the next video frame buffer and display it. |
| 8 | Scale the current video frame to the display resolution, store it into the next video frame buffer, and then display it. |

**Note:** *1080p is not supported.*

For more information on the Arty Z7-10 HDMI Input Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/arty-z7/demos/hdmi-input) on the Digilent Wiki.

For more information on the Arty Z7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/arty-z7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Arty-Z7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes               |
| OS        | No                |
| SW        | Yes               |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Arty-Z7-10-HDMI-In

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Arty Z7-10
* Vivado and Vitis Classic Installations
* Serial Terminal
* HDMI-capable Monitor
* HDMI-capable Source
* 2 HDMI Cables
* MicroUSB Cable for Programming and Communication
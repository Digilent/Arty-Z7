# Arty Z7 Root Repository

## Arty Z7-10 HDMI Output Demo

### Description

This branch contains sources for the Arty Z7-10 HDMI Output Demo.

This project demonstrates how to use the USB-UART Bridge, HDMI Sink and HDMI Source with the ZYNQ processor. Vivado is used to build the demo's hardware platform, and Vitis is used to program the bitstream onto the board and to build and deploy a C application. Video data streams in through the HDMI in port and out through the HDMI out port. A UART interface is available to configure what is output through HDMI.

There are 3 display frame buffers that the user can choose to display or write to. The configuration options are shown in the table below.

The demo uses the usb-uart bridge to configure the HDMI Display , the Arty Z7-10 must be connected to a computer over MicroUSB, which must be running a serial terminal (such as Tera Term or PuTTY).

| Option    | Function                                                                  |
| --------- | ------------------------------------------------------------------------- |
| 1         | Change the resolution of the HDMI output to the monitor.                  |
| 2         | Changes the frame buffer index.                                           |
| 3/4       | Prints a test pattern in the chosen frame buffer: blended or color bar.   |
| 5         | Inverts current frame colors.                                             |
| 6         | Inverts current frame colors seamlessly.                                  |

For more information on the Arty Z7-10 HDMI Output Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/arty-z7/demos/hdmi-output) on the Digilent Wiki.

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
* https://github.com/Digilent/Arty-Z7-10-HDMI-Out

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Arty Z7-10
* Vivado and Vitis 2021.1 Installations
* Serial Terminal
* MicroUSB Cable for Programming and Communication
* HDMI Cable
* HDMI-capable Monitor
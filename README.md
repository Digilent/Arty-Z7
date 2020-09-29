# Arty Z7 Root Repository

## Arty Z7-10 XADC Demo

### Description

This branch contains sources for the Arty Z7-10 XADC Demo.

This project instantiates the XADC IP Core and measures an analog voltage, this simple XADC demo is a Verilog project made to demonstrate the ADC functionality of the Arty Z7.

The LED associated with a specific channel brightens when the read voltage goes up.
The two user switches enable two XADC channels to be read from.

Voltages are read off of the chipKIT Analog connector, which has differential ports 1, 2, and 3 connected to the XADC pins 12, 0, and 8, respectively.

For more information on the Arty Z7-10 XADC Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/arty-z7/demos/xadc) on the Digilent Wiki.

For more information on the Arty Z7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/arty-z7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Arty-Z7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes               |
| OS        | No                |
| SW        | No                |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Arty-Z7-10-XADC

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Arty Z7-10
* Vivado 2020.1 Installation
* MicroUSB Programming Cable
* Wires and a Circuit to Measure
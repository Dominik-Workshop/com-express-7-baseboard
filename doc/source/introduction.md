# Introduction

The Baseboard supports COM Express Type 7 modules. The board breaks out major communications and peripheral interfaces as defined by the COM Express standard. It features front panel connectors for cable interfaces and a backplane edge connector designed for integrating the board into larger systems.

One of the supported COM Express Type 7 modules is the SolidRun LX2160A. It features 16 Arm Cortex-A72 processors, 4 x 10GbE and 18x PCIe Gen 3.0 lanes and is fully supported by Linux.

The board design files were created in KiCad 7.x.
You can find out more about the COM Express 7 baseboard by visiting Antmicro's portals listed below:

* [Open Hardware Portal](https://openhardware.antmicro.com/boards/com-express-7-baseboard/)
* [System Designer](https://designer.antmicro.com/hardware/devices/com_express_7_baseboard_with_lx2160a)
* [Open Source Portal](https://opensource.antmicro.com/projects/com-express-7-baseboard/)
 
They provide 3D renders and the board [stackup definition](https://openhardware.antmicro.com/boards/com-express-7-baseboard/?view=top-ortho&tab=stackup), as well as [an interactive preview](https://openhardware.antmicro.com/boards/com-express-7-baseboard/?view=top-ortho&amp%3Btab=stackup&tab=preview) of the board schematic.
A [PDF schematic](../com-express-7-baseboard-schematic.pdf) of the board is also available.

## Block diagram

<iframe src="_static/COM_Express_baseboard_VSD_graph.html" style="border:0px" height="800px" width="100%" title="COM Express 7 baseboard graph"></iframe>

## IO map 

A map of on-board connectors, status LEDs, control buttons and I/O interfaces is provided below.

:::{figure-md}
![](img/io_map.png)

COM Express 7 baseboard interface map
:::


## Power
 
COM Express 7 baseboard can be powered with a DC voltage via the on-board locking DC connector ([`J6`](#J6)) with Molex Nano-Fit plug, or backplane PCB-edge connector ([`J16`](#J16)).
More details in [Power supply](./power_supply.md) section.

## Available interfaces and features

- Gigabit Ethernet RJ45 connector ([`J1A`](#J1))
- 2x SFP+ 10 Gigabit Ethernet port ([`J2`](#J2))
- OCuLink PCIe x4 connector ([`J4`](#J4)) 
- USB 3.0 - two type A ports: ([`J1B`](#J1)) and ([`J1C`](#J1))
- USB-C console ([`J3`](#J3))
- 2x M.2 2280 key M connector with PCIe x4 ([`J5`](#J5)) and ([`J8`](#J8))
- M.2 2230 key E connector with PCIe x1 and USB([`J100`](#J100))
- SD card connector ([`J15`](#J15))
- Backplane PCB edge connector with PCIe x2, USB 2.0 and UART console ([`J16`](#J16))
- 2x RGB LED for status indication
- Board EEPROM and support for carrier MAFS BIOS

## Mechanics

The COM Express 7 baseboard PCB is 225x104 millimeters (WxL) which translates into 10.04x4.09 inch.
The overall height of the set depends on the cooling module attached.

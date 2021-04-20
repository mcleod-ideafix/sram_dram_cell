# Model for a SRAM and a DRAM memory cell.
A schematic for a SRAM and a DRAM memory cell. Made just for didactic purposes.
Uses MOSFET transistors and the same traditional 6T configuration for SRAM. For DRAM, the circuit is not exactly the same as in standard DRAM cells.
Project made using EasyEDA, ready for JLCPCB.

# 3D model and actual pictures
![3D model](/pictures/placa_3d.png)

# How to use it
To operate the SRAM cell, press and release the button for the value you want to store (0 or 1) and then, press and release the WE (write enable) button to accept the new value into the cell.
The value will stay at the SRAM OUT led as long as power supply is applied, just as in an actual SRAM memory.

To operate the DRAM cell, press and release the button for the value you want to store (0 or 1).
The value will stay at the DRAM OUT for several seconds, then it will fade to 0.
If you want to keep the value, you need to periodically press the RFSH button.
Obviously, this operation is only "visible" to the user if the value stored is 1 (led on).

# Current issues
(not fixed) the circuit draws too much current even while in static operation (not changing values). This makes the battery to drain quickly. If the voltage is lower than, aprox, 2V, the cells cease to operate correctly.

Isolate the battery from the holder with a piece of paper in between when not in use.

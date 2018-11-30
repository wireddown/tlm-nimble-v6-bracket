# LIS3DH Extension

## Tools and environment

* FreeCAD 0.17 (released August 2018)
* Autodesk EAGLE 9.2.2
* Windows 10

## Approach

Convert Adafruit's [LIS3DH Breakout PCB](https://github.com/adafruit/Adafruit-LIS3DH-Breakout-PCB) layout to metric units. In FreeCAD, use measurements from the layout to create the base body from two sketches: one for the footprint on the XY plane and the other for the profile on the YZ plane. Complete the base body by extruding both sketches and taking their intersection. Finish the bracket by fusing simple cylinder posts that force alignment of the PCB to the bracket.

Use Cinpro's upstream model [Tevo Little Monster Effector](https://www.thingiverse.com/thing:2750830) to square the bracket with the X axis and place it between the Y-tower bearing posts. Add a simple extrusion between the Nimble's base plate and the LIS3DH bracket to fuse them into a single part.

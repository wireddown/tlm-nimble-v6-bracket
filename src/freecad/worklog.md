# Work log

## Tools and environment

* FreeCAD 0.17 (released August 2018)
* Windows 10

## Approach

Because Zesty provided a solid shape in a STEP-file, I used the Part Workbench and cut into the shape with boolean operations. I chose against both Part Design and Sketcher because there weren't any drawings of any of the faces. I'm curious about the Reverse Engineering Workbench and using it to extract dimensions and constraints, but I chose the naïve brute-force approach to minimize surprises.

### Add the base Part

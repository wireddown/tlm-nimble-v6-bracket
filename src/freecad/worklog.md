# Work log

## Tools and environment

* FreeCAD 0.17 (released August 2018)
* Windows 10

## Approach

Because Zesty provided a solid shape in a STEP-file, I used the Part Workbench and cut into the shape with boolean operations. I chose against both Part Design and Sketcher because there weren't any drawings of any of the faces. I'm curious about the Reverse Engineering Workbench and using it to extract dimensions and constraints, but I chose the naïve brute-force approach to minimize surprises.

### Add the base parts

From the Part menu, I selected "Import CAD..."

### Enlarge the through-hole to allow the PTFE feed tube to pass
Otherwise, the filament can bend/kink in the 10 mm gap between bottom of the Nimble and the top of the V6.

One shape to cut:

* a cylinder: 2.3 mm r x 2.8 mm

Use this shape on the both the mount base and position plate to widen the PTFE tube hole.

### Remove material that blocks the tube collet and collet clip
Otherwise, the bracket does not sit flush on the effector.

Two shapes to cut:

* a cube: 6.5 mm x 5.5 mm x 1.5 mm
* a cylinder: 3.9 mm r x 1.5 mm

Place them flush to the same plane on their flat sides. Align their center axes and move them until they join. When their combined length is 11 mm, fuse them into one shape. Center the circle with the center of the through-hole and with the cube pointing towards the wide opening on the side of the base bracket. Finally, move the object Z-wise so that cube is flush with inner tier and cut the shape from the bracket.

### Deepen the Nimble bolt countersinks
Otherwise, the bolts strike the bottom and split the bracket in two during installation.

One shape to cut, twice:

* a cylinder: 1.75 mm r x 10 mm

Position these so that they are centered over the Nimble mounting bolt counter sinks. Lower them into the base bracket until the top of the cylinders are flush with the top face and cut them from the bracket.

### Lower the surface for the effector mounting holes
Purely cosmetic, and allows for shorter mounting bolts when attaching the bracket to the effector.

Many shapes to cut:

* a cube: 40 mm x 40 mm x 5 mm
* a cylinder, twice: 4.8 mm r x 5 mm
* a cylinder: 16.5 mm r x 5 mm
* a cylinder: 8.3 mm r x 5 mm
* a cube: 18.1 mm x 15 mm x 5 mm
* a cylinder: 4.2 mm r x 5 mm

The first cube is the main shape used to cut the mount. To quickly make the cutting shape, center the large cube over the base bracket's filament hole and lower it 2 mm below the top face of the bracket. To keep the core of the mount, the bolt stops, and gear housing, place the remaining pieces, except for the last cylinder, so that they are flush with the top face of the bracket and arrange them so they overlap those critical regions. Then, fuse them together before cutting the resulting shape from large cube. Finally, place the last cylinder so that it cuts the mounting face for the bolt beneath the Nimble flush and fuse it with the remainder of the large cube. Cut this final shape from the Nimble base shape to complete the updates.

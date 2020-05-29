## 02 Modify the (flat) shape

The flat shape of a glider defines the cells-widths, ribs-lengths and rib-positions. This is done by a 2D draft. The shape is defined by a leading-edge-curve a trailing-edge-curve and a distribution which maps a constant spaced distribution via a spline on a 90 degrees rotated distribution.
For all the splines (le, te, dist) it's possible to set the number of controlpoints. The distribution has the additional functionality to compute a constant aspect-ratio for each cell. Pressing the corresponding button will fit the controlpoints of the distribution-spline to a curve which represent a constant aspect ratio for each cell.  
![modify-shape](gifs/modify-shape.gif)  
  
  
[03 modify arc](03_modify-arc.md)
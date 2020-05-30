## 05 Modify airfoil (Deprecated, better use airfoil-workbench -> full nurbs)

A parametric airfoil is defined by a upper and a lower spline (order 2 bspline). The tangentiallity of the leading-edge is guaranteed by constraining the fron points of the spline to x=0, y=0 and the next controlpoint to x=0. The controlpoints at the trailing-edge is constrained to x=1, y=0. The airfoil represent a normalised (chord=1) rib. Using multiple airfoils allows to distribute airfoils on the glider. Again the distribution-curve is defined by a spline which assigns every rib to an merged airfoil.  
The airfoil-workbench gives better control for creating the airfoils. Here nurbs objects (bsplines of degree 3 with weights) can be modified. Weights allow to create smoother shapes.
The airfoil workbench creates "Airfoil-Features" which can be added to the glider with the properties-panel. Once this is done, the airfoiltool from the glider-workbench becomes disabled for the glider-object.

![modify airfoil](gifs/modify-airfoil.gif)  
  
  
[06 modify lines](06_modify-lines.md)
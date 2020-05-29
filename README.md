# glider tutorial with freecad

A simple tutorial on how to use openglider with freecad-gui.

## Openglider design-principles:

On the highest level openglider provides two classes which represent abstractions of a paraglider-model. The `ParametricGlider` is a parametric representation of a glider. Most propoerties of this object are defined by parametric geometries like nurbs and bezier-splines.
The `Glider` class itself is an direct representation of the paraglider. This object includes all the necessary subobject like ribs, cells, lines and all there properties. These properties are directly defined by numerical values.

The connection between a `ParametricGlider` and a `Glider` is given by the functions:
`glider = parametric_glider.get_glider_3d()`

The visual implementation of openglider in FreeCAD is done by using the mesh-functionalities available from openglider. The base-feature available in the glider-workbench is a `GliderFeature` which contains both a `ParametricGlider` and a `Glider`. There is a toolbox available to modify the parametric glider. These functions are all applied on the `GliderFeature` and therefore are not parametric (if you modify the glider it's not directly revertable -> still TODO).
On the other hand there is a toolbox available which adds functions to set parametric modifiers on top of the `GliderFeature`. These features allow to modify the `Glider`-object directly by copiing the `Glider` and modifiing some properties of the copy.
  
  
  
[00 installation](00_installation.md)
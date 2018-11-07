# c4dnotes

General notes, tip and techniques for working in Cinema 4D.


  * spin edge
  * two / four triangles can be disolved into a quad.
  * use bevel in solid mode to add cut edges
  * isoline editing in view options for sub-d
    * https://www.youtube.com/watch?v=wlEpzROs9CA


Tutorials
----------------------------------------
https://www.pluralsight.com/courses/intro-cinema-4d-r14-841


Functionality
----------------------------------------

### Quick Menu Modifiers

K - cut commands
M
U

### Commands
#### Spin Edge

M -> V
Basically rotates and edge to help change loop flow in topology.

If you experience shading anomalies after spinning edges (see image below), switch to polygon mode, select the affected polygons and call up the Change Point Order command, which should solve the problem


#### Bevel

#### Inner Extrude

#### Slide Tool

#### Loop Cut

#### Isoline Editing

#### Set Point Value

####  Disolve
M -> N
Deleted selected edges. Similar to Melt command but also removes uncessecary points.

#### Melt

#### Weld

### Selection

### Tips and Tricks

#### Create a Circle inside a quads
If you have a 2 x 2 quad, you can create a circle (udner sub-d) if you select the center point, and then belel out with the following bevel settings:

Offsetmode : Fixed Distance
Subdivision : 1
Depth : -100%

Basically, this will create a 6 sided polygon. You may need to clean up points depending on quad by using Points to Circle script  / plugin.


####  Isolating Section for Higher Resolution Detail

1. Select faces you want to isolate
2. Split faces (U -> P).
3. Deleted faces from original mesh

At this point, you can now work on isolated mesh. Just make sure that outside points / edges are not changed, and the pieces should match up.


#### Extruding relative to object faces

If you want to extrude a face out and have the extrusion angle be relative to the face, then make sure that the orientation is set to "Normal" in the move modelling axis tab / setting.

# Road Tiles Assembly {#dt-ops-tiles status=ready}

<div class='requirements' markdown="1">

Requires: Knowledge of the [Duckietown appearance specifications](#dt-ops-appearance-specifications).

Requires: Materials: tiles, white, yellow and red road markings;

Requires: Tools: scissors (or a sharp cutter) and a ruler;  

Results: Duckietown road tiles.

Next Steps: [Assembly of other components](#dt-ops-assembly).

</div>


## Before we start {#dt-ops-tiles-templates status=ready}

If you have access to a laser cutter, you can find templates to build straight and curved tiles [here](https://github.com/hosnerm/docs-opmanual_duckietown/book/opmanual_duckietown/tile_templates). If you do not have a laser cutter, it is helpful to build own templates for example from cardboard to ensure that all tiles will be the same. Pictures and descriptions of the tiles and their measurements which can be used as sample are found below.

Note: Before you attach the tape to the tiles, make sure they are free of any debris or dust. This will ensure that your roads are built to last. Use a cleaning cloth to clean the tiles before you continue.

Tip: instead of measuring and cutting each yellow segment individually, tape several parallel lines of yellow tape on the back of a tile, take a ruler and a sharp cutter, and proceed to cut them in batch.


## Straight roads {#dt-ops-tiles-straight status=ready}

Each straight road segment has:

* Solid white markings on the outer sides of the lanes (right of direction of travel);
* Dashed yellow markings at the center;
* Each lane is 22 cm wide (from end of white to beginning of yellow);
* The spacing between the yellow tapes is 2.5cm (1 inch).

<div figure-id="fig:straight_tile_real">
<img src="images/tiles/straight_tile_real.png" style="width: 70%"/>
<figcaption>
Straight tile used in Duckietown.
</figcaption>
</div>


## Curved roads {#dt-ops-tiles-curves status=ready}

Each curved road segment has:

* Solid white markings on the outer sides of the lanes (right of direction of travel);
* Dashed yellow markings at the center;
* Each lane is 22 cm wide (from end of white to beginning of yellow).

Note: As we approximate the curve with five straight pieces of tape, the radii of the lanes will slightly differ. The lane width will be between 21cm and 23cm which is good enough for the Duckiebot to find its way through the curve. If you do not have a template available for the construction, we suggest you draw two radii with the measurements shown in the picture below and fit the lines such that they have the least error with respect to the desired radii.

<div figure-id="fig:curved_tile_real">
<img src="images/tiles/curved_tile_real.png" style="width: 70%"/>
<figcaption>
Curved tile used in Duckietown.
</figcaption>
</div>


## Intersections {#dt-ops-tiles-intersections status=ready}

Each intersection road segment (3- or 4- way) has:

* Solid white markings on the outer sides of the lanes (right of direction of travel);
* Dashed yellow markings at the center;
* Each lane is 22 cm wide (from end of white to beginning of yellow);
* Solid red markings as stop signs.

Start by placing the red markings. You can then cover them with the white and yellow ones. A picture of a 4-way intersection can be found in the image below ([](#fig:4way_real)). If you want to have a 3-way intersection, simply replace one of the sides by a solid white tape.

<div figure-id="fig:4way_real">
<img src="images/tiles/4way_tile_real.png" style="width: 70%"/>
<figcaption>
4 way tile used in Duckietown.
</figcaption>
</div>

## Assembly with templates {#dt-ops-tiles-assembly status=ready}
Once you have laser cut your templates you need to screw them together. Use wood screws to ensure that everything stays in place. The templates are symmetrical, therefore it does not matter from which side you screw them in.

To build the tiles, simply align the frame of the template with the outer border of the tile and you are set to attach the tapes. the pictures in the next two subchapters show how it should look like.

### Straight roads

<div figure-id="fig:straight_tile_assembly">
<img src="images/tiles/straight_tile_assembly.png" style="width: 100%"/>
<figcaption>
Assembly of a straight tile using the laser cut template.
</figcaption>
</div>

### Curved roads

<div figure-id="fig:curved_tile_assembly_outside">
<img src="images/tiles/curved_tile_assembly_outside.png" style="width: 100%"/>
<figcaption>
Assembly of the outer line of a curved tile using the laser cut template.
</figcaption>
</div>

<div figure-id="fig:curved_tile_assembly_cut">
<img src="images/tiles/curved_tile_assembly_cut.jpg" style="width: 70%"/>
<figcaption>
Align the scissors with the slits of the template when cutting. This ensures a nice appearance of the curved tile.
</figcaption>
</div>

<div figure-id="fig:curved_tile_assembly_inside">
<img src="images/tiles/curved_tile_assembly_inside.png" style="width: 100%"/>
<figcaption>
Assembly of the middle line of a curved tile using the laser cut template.
</figcaption>
</div>

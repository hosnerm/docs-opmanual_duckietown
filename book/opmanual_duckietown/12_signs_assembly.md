# Traffic Signs Assembly {#dt-ops-city-traffic-signs status=ready}

<div class='requirements' markdown="1">

Requires: Traffic Sign Stands Pack

Results: A set of signs to be used for assembling your Duckietown.

</div>

## Build a Map {build_a_map}

Before beginning with sign assembly you should design a map that adheres to [the specification](#dt-ops-appearance-specifications).

An example that was used for the 2017 version of the class is here: [](+fall2017_info#fall2017-map)

The full set of currently existing signs is available here: [pdf](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/Signs_and_tags_V3.pdf) [docx](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/Signs_and_tags_V3.docx)

The set of tags used for the 2017 map are available here: [pdf](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/Signs_and_tags_2017.pdf) [docx](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/Signs_and_tags_2017.docx)


## Making New Signage {#making-new-signage}

If you find that what is available in the database in insufficient for your needs, then you will need to add to the existing database.


To do so you will have to load the original AprilTags file available here: [pdf](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/tag36h11.pdf) [ps](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/tag36h11.ps)


Which tag you should use depends on what type of sign you are trying add. The ranges of tags are specified in [](#tab:tag-ranges).

<col4 figure-id="tab:tag-ranges" figure-caption="April tag ID ranges">
    <span>Purpose</span><span>Size</span><span>Family</span><span>ID Range</span>
    <span>Traffic signs</span><span>6.5cm x 6.5cm</span><span>36h11</span><span>1-199</span>
    <span>Traffic lights</span><span>6.5cm x 6.5cm</span><span>36h11</span><span>200-299</span>
    <span>Localization</span><span>6.5cm x 6.5cm</span><span>36h11</span><span>300-399</span>
    <span>Street Name Signs</span><span>6.5cm x 6.5cm</span><span>36h11</span><span>400-587</span>

</col4>

First, find the last sign of the type that you are trying to make in the [signs and tags doc](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/Signs_and_tags_V3.docx). You will use the next available ID after this one.

Construct the new sign by first copying and pasting an existing sign of similar type, and then replacing/adding the new AprilTag. To add the new april tag, use a screen capture mathod to crop precisely around the tag at the top and sides and include the sign id at the bottom. Then paste the tag into your word file under your desired and resize it exactly 6.5cm (2.56inches).

If you make a new road name sign, you may need to change the font size of the name so that it appears on one line (this is why we like people with names like "ROY" and "RUS").

Important: You must also add your new sign to the [April Tags DB](https://github.com/duckietown/Software/blob/master18/catkin_ws/src/20-indefinite-navigation/apriltags_ros/signs_and_tags/apriltagsDB.yaml) in the software repo.

Add a new block like the ones that already exists or modify the one with the appropriate tag id:
```
- tag_id: ![NEW_TAG_ID]
  tag_type: in {TrafficSign, Light, Localization, StreetName}
  street_name: either ![NEW_STREET_NAME] or blank
  vehicle_name: currently not used
  traffic_sign_type: either ![TRAFFIC_SIGN_TYPE] or blank
```

The value of `![NEW_STREET_NAME]` is up to you to decide (have fun with it!). The value of `![TRAFFIC_SIGN_TYPE]` should be one of the signs in [](#fig:traffic-signs)

When finished, regenerate the PDF version of the Word file, and commit everything to the repo (via a pull request of course).

Note: It is also possible of course to start you own completely different signs and tags database, but make sure that you specify in the `april_tags` code which database to load from.

TODO: Update the way that the april tags code loads the database

## Traffic Signs Assembly

### Print the signals

First, you should print out the pdf version of the signs and tags file on the thickest card stock available. Templates can be found in the above chapter [Build a Map](#making-new-signage). Cut the signs out with a straight edge and a very sharp knife, leaving a small border of white around the sign.

### Assemble the stands


The picture below shows the parts needed for the assembly of a traffic sign stand ([](#fig:trafficsign_stand_kit)). There is one base plate, one plate to attach the traffic sign and two mounting parts.

<div figure-id="fig:trafficsign_stand_kit">
<img src="images/traffic_stand/trafficsign_stand_kit.png" style="width: 30%"/>
<figcaption>
Hardware included in a Traffic Sign Stands Pack.
</figcaption>
</div>

The four parts can be stacked together as in the following picture ([](#fig:trafficsign_stand_assembly)). Attach a piece of double sided tape on the stand to mount the traffic sign. Make sure the parts are stacked together rigidly and therefore the plate where the traffic sign will be attached is standing vertically. This is necessary to ensure that the Duckiebot will recognize the traffic sign properly.

<div figure-id="fig:trafficsign_stand_assembly">
<img src="images/traffic_stand/trafficsign_stand_assembly.png" style="width: 15%"/>
<figcaption>
Assembled Traffic Sign Stand.
</figcaption>
</div>

Now you only need to mount your traffic sign to the stand and you are already done. The finished traffic sign stand looks as in the next picture ([](#fig:trafficsign_stand_assembled)).

<div figure-id="fig:trafficsign_stand_assembled">
<img src="images/traffic_stand/trafficsign_stand_assembled.png" style="width: 15%"/>
<figcaption>
Complete Traffic Sign Stand.
</figcaption>
</div>

## Placement

For placement of signs see [](#traffic-signs-placement).

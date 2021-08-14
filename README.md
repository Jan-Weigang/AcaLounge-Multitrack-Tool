# AcaLounge-Multitrack-Tool
A MAGIX Vegas Extension able to create and modify "video walls" made for multitrack music videos

## Status
This extension is in the "WIP" stage. To test it out follow the Instructions in the beta release



### Instructions (temporary)

#### How to install:

Open the "Installing Folders" folder structure.

Copy the Extension (dll-file) and the presets (xml-files) to their respective Folders on your PC.


#### How to open: 

Open MAGIX VEGAS Pro and choose "View" / "Extensions" / "AcaLounge Multitrack Tool".



#### How it works

##### Track Creator:
Set your parameters (columns, rows, border) and press "Create Tracks" to add a Trackgroup to your project.

All Trackgroups will have a naming scheme applied and a "VEGAS Solid Color" plugin added to preview the grid.

You can create "doubles" and "triples". 
These tracks will overlap, as they are double or triple the size of the base grid.
you can use them to create a custom grid of different sized videos with perfectly matching borders.
Delete or mute unnecessary tracks of doubles and triples.

You can select a track and use the "Move Tracks" feature to move the track around on the currently set grid.
This works for singles, doubles, triples, features, and any kind. 
Pick a mode that fits your grid, as some Novelty grids use "in-between" positions.

You can create "Novelty Patterns" that use "Bezier Masking" plugins to create special layouts.
Be mindful that this can come at a performance cost, especially for large grids.

##### Track Assigner: 

Select the Videoclips that you would like to copy to a Layout.
Usually, one would have all synced videos in a seperate Trackgroup for this purpose.
Choose where you want the clips to be copied to, by selecting a Trackgroup and
placing the cursor in a region, between two markers or creating a loop-selection on the timeline.
Choose the appropriate mode and press "Assign Tracks".

This feature will create copies, any applied colorgrading or other effects will be kept.
If you want to change effects for all clips in a layout, select one clip and adjust the effects.
Then use the Buttons "Motion to all" and "...effects for all" to copy the positioning or effects to the other clips.

You can create "Extended Displays" i.e. splitting a video over multiple slots in a grid.
Assign the tracks to the Trackgroup / layout. Select one (or more) of the instances.
Press "Start Process". A Temporary Track will be added with the compositing mode "Screen".
Seeing both the large Track and the grid behing it, adjust the positioning (or movement) of the extended display.
Select the adjusted video and press "Calculate Motion". Mute the temporary track and check the extended display.
When satisfied press "Clean up" to remove and such temporary tracks in the project.
This process can be done with multiple sources at the same time.


#### THINGS THAT DONT WORK YET
The "rounded corners" feature needs the plugin "Soft Contrast" to be added. 
This plugin is no "OFX" plugin and thus the presets are not easily found on a hard drive. 


To replicate you manually can create the following presets:
Add FX "Soft Contrast" to a video.
In the tab "Effect" set all values to 0.

In the Tab "Vignette" set the following:

Exterior effect: "Transparent"

Strength: "100"

Vignette Shape: "Rectangle"

----

Softness: "0"

Width: "100"

Height: "100"

Corner radius: "15"

X position "50"

Y position "50"




Type "AMT_roundedEdgesSmall" into the Preset field and press save.

Change Corner radius to "30"

Type "AMT_roundedEdgesMedium" into the Preset field and press save.

Change Corner radius to "60"

Type "AMT_roundedEdgesLarge" into the Preset field and press save.


Done.

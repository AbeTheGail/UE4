Roads n Streets Readme

Requires the Substance Plugin in order to function.

Requires the Substance Plugin in order to function.

No, really, if you do not install the substance plugin the asset pack will appear empty and not work. 

To generate textures at 4k you will need to open your project settings, scroll down to Substance under plugins and under the cooking tap, change the Substance Engine from CPU to GPU. Then restart UE4 for the change to take effect.

Substance instance controls are located in the Textures folder.

Tiling control and tessellation control are located in the material instances located in the materials folder. 

Reccomended workflow is to drop in down to a low resolution and then bring it back up to the resolution that you want.

Material instances come with Tessellation control.


----------------------------------------------------------------------------
STREET MATERIAL
----------------------------------------------------------------------------

TOP LEVEL
-----------------------------------------------------------------------------
Asphalt_Scale_Presets: 3 scale presets for how much the apsphalt pattern repeats.

Shoulder_Mask_Control: Masks away the top bitumen from the sides inward to reveal the larger base asphalt underneath (saw road like this so I included the option into this)

--------------------------------------------------------------------------------
Color
--------------------------------------------------------------------------------

Color saturation and lightness controls for Bare Asphalt, Bitumen1 and 2.

Color saturation and lightness controls for the 2 asphalt patches groups.

Color pickers for the dirt and rocks that show up with the deep potholes.

--------------------------------------------------------------------------------
Bitumen (top asphalt layer that sits on top of the bare asphalt)
--------------------------------------------------------------------------------
There are 2 bitument layers. 

Bitumen_Layers_Flip controls wich bitumen layer is on top of the other.

Bitmen1&2_Mask_Scale: controls the scale of the mask that the bitumen1&2_Coverage control uses.
---------------------------------------------------------------------------------
Bitumen Layers 1 & 2 (both groups have the same controls so I'll just list them once)
---------------------------------------------------------------------------------
Bitumen1&2_Coverage: Increasing the value from 0 breaks away the bitumen showing the 2 bitument layer and the bare asphalt underneath.

Bitumen1&2_Tar_Coverage: Controls the amount of tar that covers everything. A new street would have the rocks in the asphalt completly covered while an older street would see rocks in the asphalt with the tar worn off the top.

Bitumen1&2_Road_Chips_Normal_Intensity: Turning on this normal effect by increasing the value gives the bitumen layer a chipped look.

Bitumen1&2_Road_Chips_Darken: Darkens the part of the bitumen layer thats  cipped off.

--------------------------------------------------------------------------------
Bitumen Layers 1 & 2 Cracks
--------------------------------------------------------------------------------

Tar_Cracks_Sealant_Coverage: Controls how much of the cracks that appear on the street are covered in tar.

Cracks_Coverage: Controls how much of the street are covered in cracks.

Cracks_Coverage_Mask_Scale: Controls how much the coverage mask repteats. The covage mask blends 2 different cracks groups together. The two cracks groups are scaled independantly with Large_cracks_scale and Small_cracks_scale.

Cracks_Strength: Controls the normal strength for the cracks.

Cracks_Random_Seed: randomizes of the crack patterns.


------------------------------------------------------------------------------
Patches(asphalt patches)
------------------------------------------------------------------------------

there are two asphalt patches groups.

Group1 and Group 2 shape_switch: switches between rectangular and oval shape for the patches.

Mirror_On_Off: When turned on will mirror the patches on from one side to the other.

Tar_Sealant_On_Off: toggles the appearans of a tar sealant border on the patches.

Square_Patches_Tar_Sealant_Switch: when turned on, masks off the top and bottom of the tar sealant border so only the sides are visible on the patches.

-------------------------------------------------------------------------------
Patches Group 1 and 2
-------------------------------------------------------------------------------

Patches x and y amount: Controls the number of patches.

Patches_Mask_Random: Randomly masks of the patches.

Patches_Position_Random: Ranomizes the position of the patches.

Patches_Global_Offset: moves the patches by x and y axis.

Patches_Warp: warps the shape of the patches.

Patches_Warp_Scale: controls the scale of the noise node used for warping the patches shape.

Patches_Scale: Controls the overal size of the patches.

Patches_Scale_Random: Randomizes the scale of the patches.

Patches_Size: Controls the length and width of the patches.

Patches_Size_Random: Randomizes the length and width of the patches.

---------------------------------------------------------------------------------
Potholes
---------------------------------------------------------------------------------

Pothole_Warp_Intensity: Warps the shapes of the potholes.

Pothole_Warp_Angle: changes the angle that the potholes shape is warped by.

---------------------------------------------------------------------------------
Potholes Deep and Shallow groups have the same controls except for 1 extra control in the deep potholes group. 
--------------------------------------------------------------------------------
Potholes_xy_amaount: Controls the number of potholes.

Potholes_Mask_Random: Randomly masks off the potholes.

Deep_Potholes_Depth_Variation: Adds variation to the depth of the deep potholes group.

Potholes_Size: Controls the legnth and width of the potholes.

Potholes_Size_Random: Randomizes the length and width of the potholes.

Potholes_Scale: Controls the overall size of the potholes.

Pothoels_Scale_Random: Randomizes the scale of the potholes.

Position_Random: Randomizes the position of the potholes.

Potholes_Rotation_Random: Randomizes the rotation of the potholes.

------------------------------------------------------------------------------
Road Grime. (the dark spot you see in the middle of the lanes on roads from all the cars that drive on the road. I don't have a better name so I'm calling them grime ruts.)
-------------------------------------------------------------------------------

Road_Grime_Opacity: Controls the opacity of the road grime.

Grime_Mask_Invert: Invert toggle for the road grime mask.

Road_Grime_Ruts_Double_or_Quad: 2 lanes or 4 lanes worth of grime ruts.

Road_Grime_Color: Color picker

Road_Grime_Level/ Road_Grime_Grunge_Amount: Controls for controlling the amound of grime on the road.

Road_Grunge_Width: Controls the width of the road grime rut.

Road_Grime_Rut_Spacing/Road_Grime_Rut_Quad_Spacing: Controls the spacing of the grime ruts.

--------------------------------------------------------------------------------
Oil Spots
--------------------------------------------------------------------------------

Oil_Spots_xy_Amount: Controls the amount of oil spots.

Oil_Spots_Scale: Controls the overall scale of the oil spots.

Oil_Spots_Scale_Random: Randomizes the scale of the oil spots.

Oil_Spots_Position_Random: Randomizes the position of the oil spots.

Oil_Spots_Opacity: Controls the opacity of the oil spots.

---------------------------------------------------------------------------------
---------------------------------------------------------------------------------
---------------------------------------------------------------------------------

STREET LINES MATERIAL
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Color group contains color pickers for the center and shoulder lines.

---------------------------------------------------------------------------------
Center Lines
---------------------------------------------------------------------------------

1_2_3_Center_Lines: Switches between 1,2, and 3 groups of center lines, depending on how many lanes you want for your road.

Center_Line_Cracks_On_Off: Toggles cracks appearing on the center lines.

Center_Lines_Cracks_Random_Seed: Randomizes the cracks pattern.

Center_Lines_Spacing: When you have it set to have 2 or 3 groups of center lines, this will control the spacing between them so you have control of lane width.

Center_Lines_Switch: This will switch between 4 common center line patterns that you would see on a road.

Nb_of_Segments: When you have Center_Lines_Switch set to the dash line pattern, this control will change the number of dash lines are in the pattern.

Dash_Lines_Gap_Length: Controls the length of the dash lines.

---------------------------------------------------------------------------------
Shape Control
---------------------------------------------------------------------------------
Street_Lines_Width: Controls the width of the lines.

Street_Lines_Breakup: Roughs up the edges of the street lines.

Street_Lines_Breakup_Scale: Changes the scale of the noise node that is used for Street_Lines_Breakup.

---------------------------------------------------------------------------------
Shoulder Lines
---------------------------------------------------------------------------------

Shoulder_Lines_Spacing: Controls the spacing of the shoulder lines. Moving them in close or pushing them out to the edges.

Shoulder_Lines_On_Off: Toggle for turning off the shoulder lines.

---------------------------------------------------------------------------------
Rumble Strip
---------------------------------------------------------------------------------

Shoulder_Rumble_Strip_On_Off: Toggle for turning on or off rumble strips for the shoulder of your road.

Center_Rumble_Strip_On_Off: Toggle for turning on or off rumble strips for the center lines.

Rumble_Strip_Bump_Amount: Sets the number of bumps in the rumble strips.

Rumble_Strip_Width: Controls the width of the rumble strips.

Shoulder_Rumble_Strip_Spacing Controls the spacing of the shoulder rumble strips. Moving them in close or pushing them out to the edges.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
COBBLESTONE ROAD
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Color
---------------------------------------------------------------------------------

3 color pickers for the cobblestones for color variation.

1 color picker used for circular and fishscale patterns.

1 color picker for the dirt between the cobblestones.

1 color picker for the dirt on top of the cobblestones.

Cobblestone_Highlight_Lightness: Controls the lightness of the highlight on the cobblestones.

Cobblestone_Highlight_Range: Controls how much the highlight color covers the cobblestones.

Cobblestone_Highlight_Contrast: Contrast control for the cobblestone highlight.

Cobblestone_Secondary_Highlight_Opacity: Controls the opacity of a secondary highlight for the cobblestones that's layered under the primary highlight.

---------------------------------------------------------------------------------
Pattern
---------------------------------------------------------------------------------
Pattern_Switch: Switches between 3 cobblestone patterns. Strait brick pattern, circular pattern, and a fishscale pattern.

Cobblestone_Shape_Switch: Switch between 3 base shapes for the cobblestones. 

---------------------------------------------------------------------------------
Circular (circular pattern and fishscale pattern)
---------------------------------------------------------------------------------

Circular_Pattern_Stone_Scale: Controls the size of the cobblestones for the circular and fishscale patterns. 

Circular/Fishscale_Pattern_scale:Toggle that changes between two versions for the ciruclar and fan patterns. The 2nd version of both contains more cobblestones in the patterns.

Ring_Color_Pattern_Switch: Switch that switches between color patterns for the circular and fishscale cobblestone patterns.

---------------------------------------------------------------------------------
Straight Pattern
---------------------------------------------------------------------------------

Number_X and Number_Y: Sets the number of cobblestones for the pattern.

Edge_Soften: Softens the edge of the cobblestones.

Middle_Size: Sqishes-pulls every other cobblestone.

Cobblestone_Scale: Controls the overal size of the cobblestones.

Slope_Variation: Adds random sloping to the cobblestones.

Cobblestone_Scale_Variation: Gives some variation to the size of all of the cobblestones.

Interstice: sets the gap size between the cobblestones.

---------------------------------------------------------------------------------
Dirt
---------------------------------------------------------------------------------

Dirt_Height: increasing the value will bring the dirt almost flush with the tops of the cobblestones, decreasing the value will push it back.

Dirt_Level: Controls how much dirt covers the cobble stones.

Dirt_Contrast: Contrast control for the Dirt_Level control

---------------------------------------------------------------------------------
Moss
---------------------------------------------------------------------------------
Color Picker for the moss.

Moss_Level: controls how much of the material the moss covers. Lower values keep it in the gaps between the cobblestones. Higher values will have it cover more and more of the cobblestones.

Moss_Contrast: Contrast control for the Moss_Level control.

Moss_Coverage_Mask: Controls a mask that gives variation to where the moss covers the material.

Coverage_Mask_Contrast: Contrast control for the Moss_Coverage_Mask control.

Moss_Coverage_Mask_Scale: Controls the scale of the Moss_Coverage_Mask.

Coverage_Mask_Random_Seed: Randomizes the Moss_Coverage_Mask.

Moss_Edge_Mask_Control: values lower than 1 will start to mask off the moss from the sides of the material.

Moss_Edge_Mask_Contrast: Contrast control for the Moss_Edge_Mask_Control.

Moss_Edge_Mask_Invert: Inverts the mask used in Moss_Edge_Mask_Control.













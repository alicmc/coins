# Coin Making Instructions

## Video Tutorial

I recommend following the video and then using the text guide as a reference afterwards

- [url](https://www.youtube.com/watch?v=YPCayoD0kpw)

## I. Prepare the coin depth maps

1.  Download the items from the Lisanby museum site.
2.  Use an image processing software to convert the images to black and white and increase the contrast.
    - In Krita apply a desaturate filter
    - Apply a auto-contrast filter and then adjust levels.
3.  Upload images to generate depth maps, download the grayscale version
    - [url](https://huggingface.co/spaces/depth-anything/Depth-Anything-V2)

## II. Prepare the coin faces

1. Add a plane mesh in blender
   - press Shift+A in object mode
   - look under Mesh dropdown
2. Subdivide the plane to create more geometry
   - Tab then right click on plane after it's selected
   - Increase number of cuts in bottom left corner menu to 30
   - Tab again to switch back to object mode
3. Add a displace modifier from menu on the right
   - Hit new then click icon with switches (far right) to add the depth map to the plane
   - Set strength to about 0.5
4. Right click the mesh and shade auto smooth
5. Add a subdivision surface modifier and place it above the displace
   - up the levels to at least 3
6. (Optional): Add a smooth corrective modifier
   - select only smooth and bump repeat up to 10
   - I personally think this makes the model less defined

Make another plane, press G then X to move it, and then repeat these steps.

## III. Turning it 3D

1. Select one face and press R X 180 to flip it over and R Z 180 to rotate it the right way
2. Align the plane by pressing G and then an axis (X Y or Z)
   - this allows you to move the plane over and make sure that they're aligned

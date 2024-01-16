# Useful link
- Keys Cheat Sheet
  http://www.blender.hu/tutor/kdoc/Blender_Cheat_Sheet.
- Textures
  https://www.poliigon.com/textures 

# Keys
- F9
  Open action ![Alt text](image.png)
- Tab
  Switch between Object mode <-> Edit mode
- /
  See only selected sections

# Add-ons
- https://andreasaust.gumroad.com/l/drop_it
- https://blendermarket.com/products/sanctus-library-addon---procedural-shaders-collection-for-blender
- https://blendermarket.com/products/realtime-materials-for-blender
- https://blendermarket.com/products/the-plant-library
- https://www.graswald3d.com/gscatter
- https://github.com/shteeve3d/blender-wiggle-2/releases/tag/v2.1.0
- https://gitlab.com/marcopavanello/real-sky
- https://blendermarket.com/products/alt-tab-water
- https://ninodefoq.gumroad.com/l/mossify?layout=profile
- https://blendermarket.com/products/blenrig
- https://n0451.gumroad.com/l/PgyXc
- https://github.com/sketchfab/blender-plugin
## Install Add-Ons
- #1
  ![Alt text](image-28.png)
- #2
  ![Alt text](image-29.png)
- #3
  ![Alt text](image-30.png)
- #4 Refresh, search for it then enable it
  ![Alt text](image-31.png)
- #5 Enjoy ~ Right click object -> drop it
  ![Alt text](image-32.png)

# Tips
- No need for high resolution:
  - Make it difficult to edit
  - Can smooth it out easily later: Right click ![Alt text](image-1.png) 
  - And add modifier to smoth out the edges ![Alt text](image-2.png)
  - Can clearly see the differences on Shade Flat
  
- Can combine Rotating, Moving with X Y Z to make it easier
  
- Proportional Editing: A game changer
  ![Alt text](image.png)

- Choose all the edges + points all around:
  - 1. Choose a point
  - 2. Press `Alt` while choose the edge
  - ![Alt text](image-1.png) 

- Making the icing:
  - 1. Doublicate the donut with Shift+D 
  - 2. Rename them well ![Alt text](image-2.png) 
  - 3. Choose the bottom half and Delete -> Verticels
  - 4. Then add modifier Solidify 
  - ![Alt text](image-3.png)

- Use Toggle X-ray to avoid skipping anything
  ![Alt text](image-4.png) ![Alt text](image-5.png)

- Uncheck in Modifier ![Alt text](image-6.png) if it's hiding our Edit mode

- To keep the icing still sticking to the donut, use `Snap` with `Face Porject` mode
  ![Alt text](image-7.png)
  - And also ![Alt text](image-8.png) so that the donut has more squares to make it realistic + can drag it down withoout making the sink in the donut
  ![Alt text](image-9.png)

- To avoid theinner part of the icing being dragged too
  - Use choose point then Alt + choose verticel to choose the very bottom part
  - Then `Ctrl`+`+` or ![Alt text](image-11.png) to get the upper part one by one
  - ![Alt text](image-10.png)
  - Then hide it with `H`
  - If wanna unhide it later ![Alt text](image-12.png)

- Making the icing edge go from this ![Alt text](image-13.png) to ![Alt text](image-15.png)
  - ![Alt text](image-14.png)  

- Make the drip by choosing 2 points + `E`
  - ![Alt text](image-17.png)
  - ![Alt text](image-16.png)

- Add another modifier `Shrinkwrap` to snap perfectly the icing `remember to put it on top of every modifier`
  ![Alt text](image-19.png)
  ![Alt text](image-18.png) 

- Make the drop of icing fatter:  
  - 1. `Sculpt Mode` with `Inflate` mode
  - 2. Just Left click to apply or Shift + Left Click to do the opposite
  - P/S: The radius should be big enough or wont see it change
  - 3. Apply subdivision modifier with 2 - 2 so that there is enough infos to sculpt
  - 4. Use the `Grab` mode to edit drop details : Make the beginning of the drop thinner, make the icing look more real with gravity
  - 5. To make the upper part kinda fatter: 
    - Use  `Mask` with `Brush-> Front Face Only` on to darken the parts that wont be affected by
      ![Alt text](image-20.png)
    - Hit `Ctrl + I` to invert the black mark
      ![Alt text](image-21.png)
    - Choose `Mesh Filter` with `Inflate` mode, Strength around 0.1, drag a bit out.
      ![Alt text](image-22.png)
    - Smooth it out with `Smooth Mask`
      ![Alt text](image-23.png)
    - Smooth again using `Smooth` sculpt
  
- Add new material + color
  ![Alt text](image-24.png) 

- Make the donut the icing's paaent by hold `Shift` then click icinf first then the donut then `Ctrl+P` -> `Object (Keep Transform)` ---> When we move our donut, the icing will move together (remember to turn off Snap though lol)

- Shading
  - Shift+A to add Image Texture 
  - Remember to choose `Non-color` as `Color Space` for everything other than the original pic
  - ![Alt text](image-26.png)
  - Can do manually like that or add add-on

- Find Auto-Saves UwU
  ![Alt text](image-27.png)

- Change the colors in a mesh:
  - Click on `Texture Paint` mode
  - Go to isolate mode with `/` for Donut
  - Change the Base Color to `Image Texture`
  ![Alt text](image-33.png) 
  - New Image -> Choose the base color and name it
  ![Alt text](image-34.png)
  - Choose the newly created image in the Texture Paint Window
  ![Alt text](image-35.png)
  - Draw other colors then save the image anywhere 
    ![Alt text](image-36.png)

- Add prinkles -> Use Geometry Nodes
  - Click on `New` to begin 
    ![Alt text](image-37.png)
  - `Shift + A` to add stuff as usual
    ![Alt text](image-38.png) 
    `Distributed Point` is to creating point
    `Join Geometry` is to keep the original icing, or else it would be replaced with the points
  - Pin the Geometry Node of icing, then drag&drop a newly created sphere in (aka the `Object Info`)
  - ![Alt text](image-40.png)
    ![Alt text](image-39.png) 
    ![Alt text](image-41.png)
  - To avoid point colappsing each other -> use `Poisson Disk` option for `Distribute Points`
    ![Alt text](image-42.png)
  - To avoid having points also on the bottom -> switch to `Weighted Paint` mode
    ![Alt text](image-43.png)
    - 1. Add new `Vertex Group` then add a `Named Attribute (attribute)` with it in the `Density` of `Distribute Points`
      ![Alt text](image-44.png)
    - 2. Use `Weighted Paint` 
      `Click` to paint
      `Alt + Click` to delete paint
      ![Alt text](image-54.png)
      ![Alt text](image-55.png)
    - 3. Multiply the value of density (or else we would see no effect of Weighted Paint)
      ![Alt text](image-52.png)
    - 4. Apply Scale `Ctrl + A` then choose Scale
      ![Alt text](image-53.png)
  - To make the diferent density if doublicate the donuts
    - 1. Drag&Drop `Density Max` onto `Group Input` -> The field would appear in `Modify` tab on every duplicated donuts
      ![Alt text](image-48.png)
    - 2. Modify its value each time
      ![Alt text](image-49.png)
      ![Alt text](image-50.png)
- We can define unit of mesurement and resize the donuts to the correct size
  ![Alt text](image-51.png)
  Then choose scaled ones then `Shift + A` -> choose Scale to apply 



      
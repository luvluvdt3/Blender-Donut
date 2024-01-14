# Useful link
- Keys Cheat Sheet
  http://www.blender.hu/tutor/kdoc/Blender_Cheat_Sheet.

# Keys
- F9
  Open action ![Alt text](image.png)
- Tab
  Switch between Object mode <-> Edit mode
- /
  See only selected sections
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
-  
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
- https://www.vfxmed.com/2023/07/blender-3-2-cloudscapes-v2-pro-2023-update-crack-download/
- https://www.vfxmed.com/2023/06/blender-2-7-auto-rig-pro-v-3-68-24-free-2023-download/
  
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

- Adding long sprinkles
  - `Shift + A` add cylinder 
  - ![Alt text](image-62.png)
  - To make the rounded edge:
    - 1. Go to `Edit mode` then choose the top and bottom rounds
    - 2. `Ctrl+B` then stretch out
    - 3. Add more layers to that when scroll up 
     ![Alt text](image-56.png)
  - Make other spinkles:
    - 1. `Shift D` to doublicate
    - 2. Choose the top part `G` then `Z` to lengthen it up (remember to turn off the Proportional Editing)
    ![Alt text](image-57.png)  
  - Make spinkles bend
    - 1. Edit mode then `Ctrl + R` to create the inner circle then scroll to create some more
      ![Alt text](image-58.png)
    - 2. Then add modifier `Simple Deform`
      ![Alt text](image-59.png)
      ![Alt text](image-60.png)
      - If doesnt work
        - `Ctrl + A` -> All transforms
        - Right click -> Set Origin -> Origin to Geometry 
    - 3. Apply it
- Apply different sprinkles
  - Doublicate the donut
  - Click on the button `2` there so that the variables are separated for each donut
    ![Alt text](image-61.png) 
  - Drag&Drop the collection of different spinkles into Geometry Node and check the 3 checkboxes
    ![Alt text](image-63.png)
    ![Alt text](image-64.png)
  - Also connect the Rotation of the 2 greens class so that the sprinkles can rotates based on the object's surface
  - Adding Rotate Euler
    ![Alt text](image-66.png)
  - Also rotates the prinkles to 90 degree
  - To ajust size of the spinkles:
    ![Alt text](image-65.png)
  - To randomize the rotation of the sprinkles while keeping them reasonable
    ![Alt text](image-67.png)

- Make sprinkles colorful and randomized colors 
  - Apply the same material for many objects
    - Create a new material within a sprinkle
    - Then `Shift` choosing every sprinkles with the target spinkles last with yellow outline
    - Then `Ctrl + L` choose
      ![Alt text](image-68.png) 
  - Go to Shadow
    - Create `Shift + A` a `Object info` and connect it with `Base Color`
      ![Alt text](image-69.png) 
    - Adding the `Color Ramp` in between to get randomized colors
      ![Alt text](image-70.png)
    - Make certain colors have metalic:
      - `Ctrl + Shift + D` to doublicate but still keep the connection of Color Ramp
      - For the one with metalic property, make it white, the normal ones black
       ![Alt text](image-71.png)
       ![Alt text](image-72.png) 
       ![Alt text](image-73.png)
      - `Ctrl+Shift+D` then connect to Rougness for some shinniness
      ![Alt text](image-74.png)

- Rendering:
  - Click the icon ![Alt text](image-75.png) to see the camera viewport
  - ` Shift + ` ` to move the camera with WASD
  - Improve rendering quality
    - ![Alt text](image-77.png) 
    - ![Alt text](image-78.png)
    - Switch to GPU for faster render & Choose `Cycle` for better quality but longer render
      ![Alt text](image-83.png)
      ![Alt text](image-84.png)
    - Also with `Denoise` checked
      ![Alt text](image-80.png)

- Improve the material of the icing for better feeling? idk
![Alt text](image-81.png)

- Also with the icing
  ![Alt text](image-82.png)

- Adding a plate :
  - Can split screen with
    ![Alt text](image-85.png) 
    ![Alt text](image-86.png)
  - `Shift + A` create a new `Round`
  - Then with `E` and `S` to create each layer together with Proportional Editing
  - To create the face surface at the bottom, choose the bottom round and hit `F`
    ![Alt text](image-87.png)
    ![Alt text](image-88.png)
  - Switch to `Edge` mode to select the round edges without choosing also the connection parts with `Alt + Shift`
    ![Alt text](image-89.png)
  - Then `Ctrl + B`
    ![Alt text](image-90.png)
  - Thicken it with `Solidify` modifier then apply
    ![Alt text](image-91.png)
  - Then choose the 2 outer edges
    ![Alt text](image-92.png)
  - `Ctrl + B`then `C`to avoid overlap
    ![Alt text](image-93.png)
  - `A` to choose everything then
    ![Alt text](image-94.png)
- Can make the camera smaller too edit easier
  ![Alt text](image-95.png)

- Different icings:
  - Rename each then click the number next to each to separate from others
  ![Alt text](image-96.png)
  ![Alt text](image-97.png)

- Adding skylight
  - Choose `Sky Texture` as color is `World` section
    ![Alt text](image-98.png)
  - Can modify the light explosure in `Render` section
    ![Alt text](image-99.png) 
  - Can also modify the sun's time and rotation
    ![Alt text](image-100.png)
- Create the counter
  - Create a new cube and go to   `Wildframe` mode
  -  Then `G` then `B`
  -  Choose the corner
    ![Alt text](image-101.png)
  - Then drag it to the corner that we want it to be aligned wiht
    ![Alt text](image-102.png)
  - Got to `Edit` mode with `Face` mode
  - Choose a face then hit `G` then `B` to make the cube perfectly cover everything
  ![Alt text](image-103.png)

- Make window
  - Choose a face
  - Hit `I` the drag it in a bit
  ![Alt text](image-104.png) 
  - Then delate that small part
    ![Alt text](image-105.png)
  - Rotate the whole stuff well for the best sun lighting
    ![Alt text](image-106.png)
  
- Walls
  - Create materials
  - Choose the wall behind then `Assign` it to the black-colored material to control lighting
    ![Alt text](image-107.png)
  - But can also add `Light->Aria` instead
  
- Download Models
  - Download & unzip it
    ![Alt text](image-108.png)
  - Click `File->Append` (remember to be in Object Mode, or else it wont work)
    ![Alt text](image-109.png)   
  - ![Alt text](image-110.png)
  - Tadahh 
    ![Alt text](image-111.png)
  - Add also Poligon's addon stuff
    ![Alt text](image-112.png)

- Compose
  - Check `Use Node`
    ![Alt text](image-113.png)
  - Hit `F12` or `Render` button to render
  - Then `Ctrl + Shift + click` on `Render Layer` to create `Viewer` node + image
    ![Alt text](image-114.png)
  - Can modify colors with `Shift + A` -> Color -> Ajust -> Color Balance
    ![Alt text](image-115.png)
  - Can also do it here (more recommended)
    ![Alt text](image-116.png)
  - Adding shiny glares
    - ![Alt text](image-117.png)
    - ![Alt text](image-118.png)
  - Make the glare foggier
    - ![Alt text](image-120.png) 
    - ![Alt text](image-119.png) 
  -  Edit the `Fac`, which control the second Image aka the second Glare
    ![Alt text](image-121.png) 
  - Final step (doesnt change any effect but kinda avoid errors in the future?)
    ![Alt text](image-124.png)
  - Apply it to `Always`
    ![Alt text](image-123.png)
  - If wanna render without `Compose`'s effects -> Uncheck `Compositing`
    ![Alt text](image-125.png)

- Camera animation
  - Add an empty axe
    ![Alt text](image-126.png)
  - Choose `Sphere` as display
    ![Alt text](image-127.png)
  - `Ctrl + P` set sphere as parent
    ![Alt text](image-128.png)
  - Click on end frame -> Choose the empty sphere -> Hit `I` - Rotation
    ![Alt text](image-129.png)
  - So the last frame would be our original Render
  - Go to the frist frame and edit the rotation and location
    ![Alt text](image-131.png)
    ![Alt text](image-130.png)
  - Go to `Animation` mode and choose `Graph Editor`
    ![Alt text](image-132.png)
  - We are gonna edit mostly X & Y Rotation
    ![Alt text](image-133.png)
    ![Alt text](image-134.png)
    With `R` and `G` to these black points
  - Fast at the start and slower a the ending 
    ![Alt text](image-135.png)
  - To zoom in at the start -> Scale down the Sphere
    - `I` then
      ![Alt text](image-136.png)
    - Then `S` make it smaller
      ![Alt text](image-137.png)

- Rendering
  - Kinda put it to 400 to make rendering faster
    ![Alt text](image-138.png)
    ![Alt text](image-139.png)
  - Hide sprinkles from camera
    ![Alt text](image-140.png)
  - Set camera's focus
    ![Alt text](image-141.png)
  - Active Motion Blur
    ![Alt text](image-142.png)
  - ![Alt text](image-143.png)
  - Now we wait
    ![Alt text](image-144.png)
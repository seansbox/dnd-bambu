# dnd-bambu
Workflow for printing miniatures for D&amp;D, Daggerheart, etc. on Bambu Labs A1 and P1S

## Workflow

1. Load the STL into Bambu Labs!
2. Set the Profile to **0.08mm High Quality**.
3. From the **Strength** menu, change **Wall loops** to **3**. *(Provides a slightly stronger outer shell to prevent damage from support material and reinforce tricky spots.)*
4. If the STL is **"unsupported"** or otherwise *not* **"supportless"** (not designed for FDM) then:
    1. Rotate the mini back **45 degrees**. *(This will help avoid support materials attaching to the front of the mini, getting caught between the legs, being generated both on the front and back of weapons, etc.)*
    2. From the **Support** menu, check **Enable support**, change **Type** to **tree(auto)**, and check **On build plate only**. *(We'll generate our own support. Tree is easier to break off than the default and less disruptive to the mini.)*
    3. Turn on **Advanced** and set the **Style** of Support to **Tree Slim**. *(This setting minimizes the touch-points on the mini. If your printer can't handle these "smaller noodles" then don't do this step.)*
    4. From the **Support** menu, turn on **Advanced** and set the **Initial layer expansion** to 5mm. *(Because the mini is small, adding some more brim to the trees helps it stay on the plate.)*
5. Create a **Cooling Tower**.
    1. Click on the mini and in the lower-right popup, make note of the third **Size** value. *(This is the height of the mini.)*
    2. Right-click next to the mini, select **Add Primitive**, and select **Cube**.
    3. Select the new cube, then click the **Scale** tool button. *(Or just press the **s** key.)*
    4. Uncheck **unform scale**, set the Z to **match the mini**, and set the X and Y to **10mm**.
    5. Press the **a** key to auto-arrange the objects. Use the arrow keys to move the tower behind the mini. *(We don't want a tower right in front of our mini!)*

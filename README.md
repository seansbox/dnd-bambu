# dnd-bambu
Workflow for printing miniatures for D&amp;D, Daggerheart, etc. on Bambu Labs A1 and P1S

## Recommended Equipment

- Sprue Cutters, such as https://a.co/d/dZU9VoP. Tiny ones are best for chopping up support materials around their tiny little legs and weapons.
- Isopropyl Alcohol (IPA, 90%+), such as https://a.co/d/dX8fMkB. I know you could just use soap and water, but IPA is great for bed-cleaning and any resin printing goodness you might have around. So you should have it anyway. And when you go to prime the mini, it will be soooo clean.

## Mini Printing Workflow

### 1. The Basics

1. Load the STL into Bambu Labs!
2. Set the Profile to **0.08mm High Quality**.
3. From the **Strength** menu, change **Wall loops** to **3**. *(Provides a slightly stronger outer shell to prevent damage from support material and reinforce tricky spots.)*

### 2. The Support

If the STL is **"unsupported"** or otherwise *not* **"supportless"** (not designed for FDM) then we'll need to generate our own supports to get the little guy from making a mess, and looking like a mess.

1. Rotate the mini backwards to **325 degrees** (which is 35 degrees back). *(This will help avoid support materials attaching to the front of the mini, getting caught between the legs, being generated both on the front and back of weapons, etc.)*
2. From the **Support** menu, check **Enable support**, change **Type** to **tree(auto)**, and check **On build plate only**. *(We'll generate our own support. Tree is easier to break off than the default and less disruptive to the mini.)*
3. Turn on **Advanced** and set the **Style** of Support to **Tree Slim**. *(This setting minimizes the touch-points on the mini. If your printer can't handle these "smaller noodles" then don't do this step.)*
4. From the **Support** menu, turn on **Advanced** and set the **Initial layer expansion** to 5mm. *(Because the mini is small, adding some more brim to the trees helps it stay on the plate.)*

### 3. The Tower

Layers that have less for the printer to print, such as the upper layers of a mini holding up a sword, will cause the printer to move on too quickly to the next layer before the previous one has sufficiently cooled. This will create some unsightly dipping and/or filament bulging to an otherwise beautifully printed mini. To remediate this, we'll create a "cooling tower" to keep the printer busy just long enough for each layer to cool before it moves on.

1. Click on the mini and in the lower-right popup, make note of the third **Size** value. *(This is the height of the mini.)*
2. Right-click next to the mini, select **Add Primitive**, and select **Cube**.
3. Select the new cube, then click the **Scale** tool button. *(Or just press the **s** key.)*
4. Uncheck **unform scale**, set the Z to **match the mini** (rounded up), and set both the X and Y to **15mm**.
5. Press the **a** key to auto-arrange the objects. Select the "tower" and use the arrow keys to move the tower behind the mini. *(We don't want a tower printing right in front of our mini!)*

### 4. The Cleanup

***GO SLOWLY!***

1. Try to cut the base off of the support noodles. This will give you better line of sight and allow you to individually wiggle the noodles as needed to break off support material. Cut the noodles from each other. More flexible.
2. Use side cutters to wiggle noodles near the contact points or break off noodles by pinching them with the cutters.
3. Once support material is removed, wash the mini to help reveal remaining support bits and fixable scarring.

## Other Notes

### Material Selection

- **PLA** or **PLA Tough** has consistently resulting in better quality prints. **PETG** tends to droop more on overhangs even with the cooling tower and struggles more with the tighter angles common on minis.

### Rotate-back Angle

The following represents the total amount of filament required to print four assorted minis at various angles of rotation (changes are due primarily to support material requirements, but also slightly different due to slicing):

- 20 deg = 10.58 m
- 25 deg = 10.35 m
- 30 deg = 10.32 m
- 35 deg = 10.27 m
- 40 deg = 10.10 m
- 45 deg = 10.12 m

The inflection point is generally around 40 degrees, however, the steeper the angles, the more detail loss we see on the back. So for now, we've stuck with 35 degrees.

### Additional Information

- [Bambu Filament Guide - Web](https://bambulab.com/en/filament-guide)
- [Bambu Filament Guide - PDF](filament-guide-en.pdf)

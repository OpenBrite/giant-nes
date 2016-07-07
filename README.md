# giant-nes
CAD files for a giant NES controller as seen (soon) on Instructables

## Why?

Stacy apparently always thought it would be cool to have a game controller so big that it forced multiple people to collaborate on it in order to play a game.  Stephen wanted to gain proficiency on the CNC router table before going onto make pinball playfields (and now those seem like a walk in the park compared to this).  Neither of them knew how much painting and sanding work they were in for.  While this 100x-sized NES controller can still be played by one person, two people can certainly enjoy it comfortably, since it's more than 4 feet wide and almost 2 feet long.

To find out what you're supposed to do with these files, visit our Instructable.

### Licensed under Creative Commons Zero 1.0 Universal

## Using these files

If you have VCarve 8.0 or newer, you can edit the design in that program before exporting it to your desired G-Code flavor.  This is also important if your table router doesn't speak "MultiCam G Code (inch) (*.cnc)".  Consider the three *.crv files representing the front & back of the controller face (including milling the buttons) and the all-important paint stencil.

Note the measurements throughout these files are in millimeters because the rest of the world besides the USA does things in metric and thus the numbers come out a whole lot rounder when you enter the metric mindset.

If you don't have VCarve 8.0 and your table router can understand these CNC files, by all means go ahead and run them (on DRY RUN first!).  The G-code files follow this naming convention:

* F[1-4]: Things you will mill out of the front of the controller face, sequentially from file F1 to F4
* B[1-2]: Things you will mill out of the back of the controller face, sequentially from file B1 to B3
* G1: Mill this out of the front of the controller face after you mill the back... well theoretically it shouldn't really matter if you flip it back around :-P
* S[1-2]: Things you will mill out of the paint stencil, sequentially from file S1 to S2

The file names usually contain some sort of description indicating the tool involved, such as "End Mill", "Ball Nose", or "V Bit", and a 4-digit number indicating the size of the tool in mils, such that 0125 = 1/8 inch and 1000 = 1 inch.

## Errata and Considerations

When using the B1-0250 End Sw Mts file, be sure to consider that your switches might be a different size than the ones I used.  Heck, even the ones I bought were surplus and I couldn't find the company who made them on Google, so it's likely I'll never find them again once the local store runs out.  My switches have a circular 8mm contact point, so if that doesn't describe your switches, you will definitely need to edit the NES Back file in VCarve or a compatible tool.

Even if you happen to find the exact same switches, it seems that the points I drilled into the back side were not exactly in the center of the buttons, particularly in A & B.  This could cause the button to get caught on the edge of the button pocket if it gets spun around.  To remedy this, one could consider gluing the A & B buttons to the switch.

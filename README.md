# iOS Web Apps: Photoshop actions for startup screens

Resizing startup screens is very boring.  This is a set of actions that will copy and resize your portrait and landscape startup screens to the various dimensions that you need for tablet (non-retina) and mobile (retina and non-retina).

## How-to

0. Copy the .atn file somewhere useful and load the actions into Photoshop via Actions panel > Load Actions...

1. Create your start screen in the largest sized portrait (1536 x 2008).

2. Also create your largest sized landscape (1496 x 2048, content should be rotated 90 degrees clockwise so the left edge is at the top).  The proportions are thinner and taller so you'll need to tweak the background manually.

3. Go back to the portrait version and run the "apple start images - portrait" action.  It creates 3 new documents.

4. Check the mobile versions (apple-touch-startup-retina and apple-touch-startup) as the width gets clipped a little.

5. Go back to the landscape version and run the "apple start images - landscape" action.  It creates 1 new document.

6. Save for Web and Devices in the png format for all images.

7. (Devs) Use some JavaScript along the lines of https://github.com/h5bp/mobile-boilerplate/issues/94 in the head of the HTML to output just 1 startup image.  A rare legitimate use of document.write.  If you list them all, they all get downloaded to the device.

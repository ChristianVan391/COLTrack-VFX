# COLTrack-VFX
## A simple, portable VFX camera tracking tool for Blender.
this is a simple VFX tracker I made for Blender 5.2* based on COLMAP.
I made this due to using Blender's built-in tracker being annoying and decided to share it for the rest of the world.

## features

- simple to use tracking.

- supports multiple videos.

- super accurate without sliding objects and mesh.

- json output and custom importer script**

- automatic lining up/normalization (no need to line up the scene to your world)

- based on Python, FFmpeg, and COLMAP***

## how to use

- 1 Download from [place holder link. yeah this is not public yet] and extract the zip

- 2 once extracted open up the folder "VFX_Tracker".

- 3 open "Check Setup.bat" to see if everything will work (do this once in a while)****.

- 4 place your videos into the folder "Videos".

- 5 double click "Track Videos.bat" and wait for it to finish tracking.

- 6 once finished you should have a .json file in the folder "Output".*****

- 7 to import your track into Blender go to the "scripting" tab and click Open and locate the folder "VFX_Tracker" and find "ImportTrack Blender 5.2.py".

- 8 now that the script is imported in Blender click "Run Script" (the play button).

- 9 a file picker will open. locate the folder "VFX_Tracker" and go to the folder "Output" and open the json file corresponding to the video you tracked.

- 10 now click the "layout" tab. you will see a point cloud (black dots) and a path (line/trail following camera path) these are under the new object "VFX_Track_Root" and should be disabled for render and may be disabled for viewport if needed.
## footnotes
- *tested in 5.2 LTS but should work in 5.2 regular and maybe older, versions but not guaranteed so be careful with old projects.
- **may work in other programs but the importer script may need to be modified.
- ***no need to install these as they are bundled in and will work automatically. also this is based on COLMAP 4.1.1 no-CUDA (CPU only) for compatibility.
- ****this is only to check if the core dependencies are included. if not please come redownload from [the place holder link we will need again].
- *****this may happen if the video did not have any parallax or something is wrong. videos orbiting the area and/or with good parallax can help. plus having good video input also helps.

## Issues & Support

If you encounter a bug or something isn't working correctly,
please [open an issue](https://github.com/ChristianVan391/COLTrack-VFX/issues)
with as much information as possible.

Please include:

- What you were trying to do
- What happened
- Any error messages
- Blender version
- A description of the video/footage being tracked

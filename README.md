# FP_ConstructionManual

FLipPad Construction Manual

# Software

* Scribus for the page layout
* FreeCAD for the PCB & case renderings

## FreeCAD Plugins

Due to different extra features we need, some new workbenches (addons) must be installed to FreeCAD:

* __Render:__ Install this workbench via the integrated addon manager (Tools -> Addon manager)
* __Animate:__ Currently (02/2022), the animate workbench has to be installed manually: https://jirivalasek.github.io/Animate/Guide/getting_started.html

## Additional hints

### Converting the output PNGs from Animate to gif/avi

Quality is not very good for .avi:

`ffmpeg -i "seq20220228171006-%5d.png"  -framerate 12 -y out.avi`

.gif quality is acceptable, but quite a big output file:

`ffmpeg -i "seq20220228171006-%5d.png"  -framerate 6 -filter_complex  "fps=6,split=2[palette_in][gif];[palette_in]palettegen[palette_out];[gif]fifo[gif_fifo]; [gif_fifo][palette_out]paletteuse" -y image.gif`

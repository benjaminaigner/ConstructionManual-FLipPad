# This is a non-working KiCAD PCB for FLipMouse 2

This PCB file is currently not functioning, this is only for 3D rendering.
Next batches might be using this project instead of the EAGLE files.

# Usage

If you want to adapt the renderings or any parts of the PCB:

* Apply changes to the PCB
* Export the PCB into a STEP file (PCBNew -> File -> Export -> STEP)
* Create a new FreeCAD project (v0.17 recommended)
* Set background color to simple color, white (Edit->Preferences->Display)
* Import the STEP file into FreeCAD (File -> Import)
* Adjust colors manually:
	- LEDs
	- (PCB)
* Execute macro from the FreeCAD_Macro subdirectory
* Images 4&5 are positioned manually (to see the PCB top on the bottom with already mounted
01x02 +  02x05 headers and capacitors).
* Image 4 contains the headers, including the 2 01x14 + 01x05 headers for the Teensy
* Image 5 is with Teensy as well


__Note:__ The KiCAD parts are named within FreeCAD, so it is possible that names within the macro have to be changed!

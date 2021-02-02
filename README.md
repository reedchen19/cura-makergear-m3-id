# cura-makergear-m3-id
Cura machine settings and extruder profiles for the MakerGear M3-ID. Start and end gcode is for IDEX (Independent Dual Extrusion) only

Use start-gcode instead of simple-start-gcode. simple-start-gcode results in worse prints

### Printer Settings
* X = 180 mm
* Y = 232 mm
* Z = 203 mm
* Build plate shape = Rectangular
* Origin at center = False
* Heated bed = True
* Heated build volume = False
* G-code flavor = Marlin

### Printhead Settings
* X min = -10 mm
* Y min = -60 mm
* X max = 30 mm
* Y max = 15 mm
* Gantry Height = 5 mm
* Number of Extruders = 2

### Extruder 1
* Nozzle size = 0.35 mm
* Compatible material diameter = 1.75 mm
* Nozzle offset X = 0
* Nozzle offset Y = 0
* Cooling fan number = 0
* No start or end gcode

### Extruder 2
* Nozzle size = 0.35 mm
* Compatible material diameter = 1.75 mm
* Nozzle offset X = 0
* Nozzle offset Y = 0
* Cooling fan number = 1
* No start or end gcode

Your Machine Settings window should look like this:
![img](https://github.com/reedchen19/cura-makergear-m3-id/blob/main/MachineSettings.png)

### Notes
Start and end gcode was taken from https://github.com/MakerGear/MakerGearM3Profiles and modified slightly. Most important modification was the addition of M605 S1
gcode for dual-nozzle mode.

Measurements for the printhead settings were made with rough estimates and are not exact.

Extruder profiles are mostly default with a few changes:
* 0.2 mm initial layer height
* 200 degC initial/final printing temperature
* 30 mm/s print speed
* 60 mm/s travel speed
* ooze shield enabled

Feel free to modify extruder profiles

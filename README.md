# Filament-Cutter-Sherpa-Mini
Filament Cutter Sherpa Mini Base ERCF

You will need to glue the blade into the blade holder.

The blade used is a standard 9mm cutter blade only the starting part is used.

Then you will also need to glue the cutter block.

Use a fairly strong spring with a 3mm screw which will come to rest on the side of your printer.

For the moment only support for switchwire has been made.

I am waiting for the use of makers who could possibly provide an stl or a method for voron 2.4 or trident

"Macro filament cutter, for stepperonline 59Nm for example, which requires increasing the run current to cut the filament"

[gcode_macro Filament_cutting]

gcode:
G92 E0
G1 E-35 F1800
G1 X20 F5000
SET_TMC_CURRENT STEPPER=stepper_x CURRENT=2
SET_TMC_CURRENT STEPPER=stepper_z CURRENT=2
G1 X0 F1000
G1 E-35 F1800
SET_TMC_CURRENT STEPPER=stepper_x CURRENT=1.100
SET_TMC_CURRENT STEPPER=stepper_z CURRENT=1.100


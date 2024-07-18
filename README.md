# 3D printer settings

## Extruder Settings
Diameter: 0.4 mm
Extrusion Multiplier: 1.04
Retraction Distance: 2.5 mm
Retraction Speed: 1800 mm/min
Coasting Distance: 0.2 mm

## Print Settings
Layer Height: 0.1 mm
Top Solid Layers: 7
Bottom Solid Layers: 7
Perimeter Outlines: 2
First Layer Height Percentage: 100%
First Layer Width Percentage: 100%
First Layer Underspeed: 0.5

## Raft
Use Raft: No
Raft Top Layers: 3
Raft Base Layers: 2
Raft Offset: 5 mm
Raft Separation Distance: 0.4 mm

## Skirt
Use Skirt: Yes
Skirt Layers: 1
Skirt Outlines: 2
Skirt Offset: 4 mm

## Infill
Infill Percentage: 10%
Internal Infill Pattern: Rectilinear
External Infill Pattern: Rectilinear
Infill Extrusion Width Percentage: 100%

## Supports
Generate Support: Yes
Support Infill Percentage: 10%
Support Type: Grid
Support Grid Spacing: 5 mm
Max Overhang Angle: 15°

## Temperature
Primary Extruder Temperatures:
Layer 1: 210°C
Layer 2: 205°C
Heated Bed Temperature:
Layer 1: 45°C

## Fan Speed
Layer 1: 0%
Layer 2: 20%
Layer 5: 40%
Layer 10: 60%

## Printer Overrides
Stroke X Override: 220 mm
Stroke Y Override: 220 mm
Stroke Z Override: 240 mm

## Speed Settings
Default Speed: 3000 mm/min
Outline Underspeed: 0.5
Solid Infill Underspeed: 0.8
Support Underspeed: 0.8
Rapid XY Speed: 4800 mm/min
Rapid Z Speed: 1002 mm/min

## Retraction
Retraction Min Travel: 3 mm
Tool Change Retraction Distance: 12 mm
Tool Change Retraction Speed: 600 mm/min
Firmware & Machine Configuration
Firmware Type: RepRap (Marlin/Repetier/Sprinter)
Baud Rate: 115200

## GCode
Starting GCode:
G28 ; home all axes
G29 ;
G1 X0 Y20 Z0.2 F3000 ; get ready to prime
G92 E0 ; reset extrusion distance
G1 X200 E20 F600 ; prime nozzle
Ending GCode:
M104 S0 ; turn off extruder
M140 S0 ; turn off bed
G1 X0 Y200 F1000 ; prepare for part removal
M84 ; disable motors

# Klipper Ender 5 Plus

Ajustes para Klipper de la Ender 5 Plus con SKR 1.4 Turbo y TMC 2209


## Simplify3D v5.0 Macros:
```
START_PRINT EXTRUDER_TEMP=[extruder0_temperature] BED_TEMP=[bed0_temperature]
```
```
END_PRINT
```
## PrusaSlicer:
```
// PrusaSlicer-SuperSlicer
M190 S0 ; Prevents prusaslicer from prepending m190 to the gcode ruining our macro
M109 S0 ; Prevents prusaslicer from prepending m109 to the gcode ruining our macro
START_PRINT EXTRUDER_TEMP=[first_layer_temperature] BED_TEMP=[first_layer_bed_temperature]
```
```
END_PRINT
```

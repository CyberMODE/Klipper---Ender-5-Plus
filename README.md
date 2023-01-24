# Klipper Ender 5 Plus

Ajustes para Klipper de la Ender 5 Plus con SKR 1.4 Turbo y TMC 2209

PAM https://github.com/HelgeKeck/pam

## Simplify3D v5.0 Macros:
```
MESH_CONFIG X0=[build_min_x] Y0=[build_min_y] X1=[build_max_x] Y1=[build_max_y]
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

# Klipper on a Prusa i3 MK3S

Stock configuration for the MK3/MK3S, converted over to Klipper. Use your standard Prusa printer profiles, but with Klipper.

## Slicer Start GCode

### SuperSlicer
```gcode
PRINT_START BED={first_layer_bed_temperature[initial_extruder]} EXTRUDER={first_layer_temperature[initial_extruder]+extruder_temperature_offset[initial_extruder]}
```

### PrusaSlicer
```gcode
PRINT_START BED={first_layer_bed_temperature[0]} EXTRUDER={first_layer_temperature[0]}
```

## Slicer End GCode
```gcode
PRINT_END
```

# Donations

Found this repo helpful? Buy me a [Ko-Fi](https://ko-fi.com/tinyfluffs_)

# License

MIT License

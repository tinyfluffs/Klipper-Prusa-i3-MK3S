# Klipper on a Prusa i3 MK3S

Stock configuration for the MK3/MK3S, converted over to Klipper. Use your standard Prusa printer profiles.

## Slicer Changes

If using the built-in filament profiles, __remove the start g-code__ under the filament section. This modifies the flow rate to 96% to compensate for older printers. The MK3/MK3S don't need this.

### Printer Start GCode

#### SuperSlicer
```
PRINT_START BED={first_layer_bed_temperature[initial_extruder]} EXTRUDER={first_layer_temperature[initial_extruder]+extruder_temperature_offset[initial_extruder]}
```

#### PrusaSlicer
```
PRINT_START BED={first_layer_bed_temperature[0]} EXTRUDER={first_layer_temperature[0]}
```

### Printer End G-Code
```
PRINT_END
```

# Donations

Found this repo helpful? Buy me a [Ko-Fi](https://ko-fi.com/tinyfluffs_)

# License

MIT License

# my-3018-cnc-laser

[Original machine I bought](https://aliexpress.ru/item/1005006562808373.html)

[Its thingiverse page, buylist, plans](https://www.thingiverse.com/thing:3508781)

[3018 github](https://github.com/MKme/3018)

## Upgrades

- [Axis handles](https://aliexpress.ru/item/32958606282.html)
- [Control board](https://aliexpress.ru/item/1005003183498253.html) with [Fluidnc](http://wiki.fluidnc.com/)
  - [Schematics](https://github.com/makerbase-mks/MKS-DLC32/blob/main/MKS-DLC32-main/hardware/MKS%20DLC32%20V2.1_003/MKS%20DLC32%20V2.1_003%20PIN.pdf)
  - [Pinout](https://github.com/makerbase-mks/MKS-DLC32/blob/main/MKS-DLC32-main/hardware/MKS%20DLC32%20V2.1_003/MKS%20DLC32%20V2.1_003%20PIN.pdf)
  - [Wiring manual](https://github.com/makerbase-mks/MKS-DLC32/blob/main/MKS-DLC32-main/doc/DLC32%20wiring%20manual.pdf)
  - [FluidNC wiki on DLC32 board](http://wiki.fluidnc.com/en/hardware/3rd-party/MKS_DLC32)
- [z probe](https://aliexpress.ru/item/1005005754638114.html?)
- [Endstops and other](https://www.thingiverse.com/thing:2796202) printed parts
- [Z carret](https://www.printables.com/model/367235-z-axis-modular-support-cnc-3018)
- [Laser & Shpindle holder](https://www.printables.com/model/367237-modular-spindle-and-laser-holder-for-cnc3018)

## Config

- [Laser engraver base config](https://github.com/bdring/fluidnc-config-files/blob/main/official/MKS_DLC32_v21_laser.yaml)
- [Laser engraver current config](MKS_DLC32_v21_laser.yaml)
- Laser engraver final config - TODO
- CNC config - TODO
- axis speed 1000mm/min
- Laser focus distance 45mm

### Switching config
As of [this instruction](http://wiki.fluidnc.com/en/config/overview)
one can change current config by sending command

```
$Config/Filename=my_machine.yaml
```

## Service

- lythol-24 for axis greasing
- stepper driver Vref value 0.76V https://www.youtube.com/watch?v=7VHwcEroHPk (Actual value ~1.3Vlower values make low torque)
- Laser module fan 30mm 12V
- Laser module dimensions 33x33mm

## Operation

1. Home
2. ``G92 X0 Y0 Z0``  # Depends on your working sheet/material
3. ``G0 X0 Y0 Z23``  # Just check moving
4. Start program

## Useful links
- https://jscut.org/jscut.html#  Cut from SVG online
- https://grid.space/kiri/ Cut from SVG (complicated)
- https://ncviewer.com/ GCODE viewer


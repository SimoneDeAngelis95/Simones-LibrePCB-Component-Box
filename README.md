<div align="center">
  <img src="library.png" width="320" alt="Simone's LibrePCB Component Box icon">

  # Simone's LibrePCB Component Box

  A carefully crafted collection of reusable components for LibrePCB.
</div>

## About

This library contains symbols, components, packages, devices, and selected 3D
models created for personal electronics projects and shared with the LibrePCB
community.

The current release was created and tested with **LibrePCB 2.1.1**.

## Included parts

### Modules and integrated circuits

- Daisy Seed3, including a custom 40-pin THT package and detailed STEP model
- 6N138 optocoupler
- 74HC14 hex Schmitt-trigger inverter
- CD4051 analog multiplexer/demultiplexer
- MCP6022 dual operational amplifier
- OPA2134PA dual audio JFET-input operational amplifier
- MCP23017 I/O-expander module
- I2C LCD display module
- KY-040 rotary encoder module

### Connectors and controls

- Female 5-pin DIN MIDI connector
- TS jack
- Two-pin DC power jack connection
- External switch
- Three-position SPDT switch (`ON-OFF-ON`) with a 2.54 mm wired footprint
- Wired three-pin potentiometer connection (`POT-WIRE-P2.54`)
- 16 mm right-angle PCB potentiometer with 5 mm terminal pitch

### Discrete semiconductors

- 1N5817 Schottky diode with a reusable DO-41 THT package
- Common-cathode RGB LED with a four-pin 2.54 mm wired footprint

The potentiometer devices reuse the standard potentiometer component from the
LibrePCB Base Library, which is declared as a dependency.

## Installation

Close LibrePCB, then clone the repository into the `data/libraries/local`
directory of your LibrePCB workspace:

```bash
git clone https://github.com/SimoneDeAngelis95/Simones-LibrePCB-Component-Box.git \
  Simones-LibrePCB-Component-Box.lplib
```

Alternatively, download the repository as a ZIP archive, extract it into the
same directory, and ensure that the extracted folder ends with `.lplib`.

Restart LibrePCB and wait for the library scan to complete.

## Library structure

- `sym/` - schematic symbols
- `cmp/` - logical components and signals
- `pkg/` - PCB packages and STEP models
- `dev/` - mappings between components and packages

## Contributing

Bug reports, dimensional corrections, and new part suggestions are welcome
through GitHub Issues. Please include the manufacturer's datasheet whenever a
change concerns mechanical dimensions or pin assignments.

## License

This library is released under the
[Creative Commons CC0 1.0 Universal](LICENSE.txt) public domain dedication.
You may use, modify, and redistribute it for any purpose, including commercial
projects, without attribution requirements.

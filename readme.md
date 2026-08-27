# ErgoFlow Wing-A

ErgoFlow Wing-A is a split ergonomic keyboard project.

This repository contains the 3D CAD model of the keyboard, manufacturing files, media, and the ZMK firmware configuration.

## Repository structure

```text
ErgoFlow_Wing-A/
│
├── CAD/
│   ├── 01 Case/
│   ├── 02 Wrist_rest/
│   ├── 03 Components/
│   └── Assem_full.SLDASM
│
├── Manufacturing/
│   ├── 3D print models STL/
│   └── PCB board/
│
├── ZMK_firmware/          # Git submodule
│
├── Media/
│   ├── Photo/
│   └── Render/
│
├── README.md
├── .gitmodules
└── .gitignore
```

## CAD

The main SolidWorks assembly is located at:

```text
CAD/Assem_full.SLDASM
```

The `CAD` directory contains the SolidWorks models used to design the keyboard:

* `CAD/01 Case/` — keyboard case and enclosure components
* `CAD/02 Wrist_rest/` — wrist rest
* `CAD/03 Components/` — components used in the assembly
* `CAD/Assem_full.SLDASM` — complete keyboard assembly

The CAD files are provided in SolidWorks format.

## Manufacturing

Manufacturing-ready files are located in:

```text
Manufacturing/
```

### 3D printing

Files for ordering the 3D-printed keyboard case are located in:

```text
Manufacturing/3D print models STL/
```

The STL files can be imported directly into a slicer or uploaded to a 3D printing service.

### PCB

Files for ordering the printed circuit boards are located in:

```text
Manufacturing/PCB board/
```

These files contain the manufacturing data required to order the PCB from a PCB manufacturer.

## Firmware

The keyboard firmware is maintained in a separate Git repository and included in this project as a Git submodule:

```text
ZMK_firmware/
```

The firmware repository contains the ZMK configuration, keymap, board configuration, and build files.

### Clone the repository with the firmware submodule

To clone the project together with all Git submodules, use:

```bash
git clone --recurse-submodules https://github.com/aL1fe/ErgoFlow_Wing-A.git
```

### Keymap editor

The keyboard keymap can be conveniently edited using the [ZMK Keymap Editor](https://nickcoutsos.github.io/keymap-editor/).
The editor provides a graphical interface for configuring the keyboard keymap.

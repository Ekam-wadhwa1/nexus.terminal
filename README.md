![banner](assets\banner.jpg)
# nexus terminal
this is a small handheld cyberdeck with a custom mechanical keyboard with macropad, rotary encoders and joystick for use as a reading terminal, hardware hacking tool or even a compact work station running windows, yes it can run full x86 windows

## Features

* **Custom Mechanical Keyboard:** Integrated layout featuring a dedicated macropad for custom shortcuts.
* **Tactile Controls:** Dual rotary encoders and a physical joystick for navigation and custom inputs.
* **keyboard display:** a 1.3" Oled display for setting macro's and show stats
* **Heavy Compute:** Powered by a LattePanda IOTA mainboard for full desktop-class performance in a portable form factor.
* **Fully Modular CAD:** Parametric case design optimized for 3D printing and easy hardware modification.
* **Active Cooling System:** Integrated cooling with a dedicated active cooler to maintain optimal temperatures under heavy processing loads.
* **Modular Type-C UART Interface:** An exposed Type-C module in keyboard wired for UART protocol, allowing you to instantly hot-plug custom external hardware modules, sensors, or debugging tools.

## Repository Structure

| Directory | Content Description |
| :--- | :--- |
| `ASSETS/` | Project imagery, graphics, and branding materials (e.g., banner, logos). |
| `CAD FILES/` | 3D mechanical assemblies separated into individual `STEP` and `STL` directories. |
| `DATASHEETS/` | Comprehensive hardware datasheets for core components (OLED, MCP23017, TP4056, switches, etc.). |
| `DIMENSIONS AND DRAWINGS/` | 2D layouts, dimensions, and reference drawings for the hardware displays. |
| `FUSION FILES/` | Original parametric design assets (`.f3d`) for custom individual components and sub-assemblies. |
| `KICAD FILES/KEYBOARD/` | Active development directory for the custom keyboard and macropad electronics engineering. |
| `PRINT FILES/` | Sorted, print-ready `.stl` slice files split by assembly groups (`DEVICE` vs `KEYBOARD`). |
| `PRODUCTION(KEYBOARD PCB)/` | Manufacturing-ready hardware deliverables (Gerber `.zip`, BOM, coordinate position files). |
| `scotto_kicad/` | Source hardware schematic captures, custom footprints, and layout design routing maps. |


 ## Getting Started

### Mechanical & CAD Files
* **For 3D Printing:** Navigate to `PRINT FILES/` or `CAD FILES/STL/`. The components are pre-oriented and split into clean assembly layers (`DEVICE` and `KEYBOARD`) for straightforward printing.
* **For Design History / Assembly:** Open the `.f3d` assets inside the `FUSION FILES/` directory using Autodesk Fusion to access the full parametric timeline and component design structure.

### Electronics & PCB Fabrication
* **Schematics & Layouts:** Open the `scotto_kicad/` directory using KiCad to view the schematic captures and matrix traces.
* **For Manufacturing:** Production-ready production outputs (including Gerber archives, component coordinates, and placement data) are fully generated and located in the `PRODUCTION(KEYBOARD PCB)/` folder.

### Modular Hacking Interface
* The integrated Type-C interface breaks out **UART** communication protocol pins. Custom external peripheral modules can be hot-plugged directly into this bus for hardware expansion.

## credits
keyboard footprint and kicad library- [joe scotto][scotto]
documentation for lattepanda iota- [lattepanda][panda]
documentation for 7 inch display- [display 7"][panda2]
documentation for 7.9 inch display- [display7.9"][waveshare]

## License
This project is licensed under the terms found in the [LICENSE](LICENSE) file included in this repository.

## badges
![GitHub repo size](https://img.shields.io/github/repo-size/ekam-wadhwa1/nexus.terminal?color=amber&style=flat-square)
![GitHub license](https://img.shields.io/github/license/ekam-wadhwa1/nexus.terminal?color=teal&style=flat-square)
![Hardware](https://img.shields.io/badge/hardware-custom%20PCB-blue?style=flat-square)
![CAD](https://img.shields.io/badge/CAD-Fusion%20360-orange?style=flat-square)

## about me
im just a student trying my best to do stuff i like

connect here
[![Instagram](https://img.shields.io/badge/Instagram-ekam.wadhwa1-E4405F?style=flat-square&logo=instagram&logoColor=white&color=amber)](https://www.instagram.com/ekam.wadhwa1/)



### links
[scotto]: https://github.com/joe-scotto/scottokeebs
[panda]: https://docs.lattepanda.com/content/iota_edition/specification/
[panda2]: https://docs.lattepanda.com/content/iota_edition/product_catalog/
[waveshare]: https://www.waveshare.com/wiki/7.9inch_HDMI_LCD?srsltid=AfmBOorE2-GmKdZrASGmWnHQZjMvq2EKgf3DztLH1sLowHcDzXAIXQx8

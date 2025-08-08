# 24S-DCDC — KiCad Project (skeleton pre-route)

**Status:** This is a *simplified, illustrative* routed board stub produced in-chat.  
It contains:
- A 100×100 mm outline with 4× M3 mounting holes (92 mm square pattern).
- XT90 input connector (J1) and three XT90 output connectors (J2=48V, J3=12V, J4=5V).
- Three "BuckBlock" placeholder footprints (B1 48V, B2 12V, B3 5V) with VIN/VOUT/GND pads.
- Thick copper tracks for VIN, GND, and each Vout to its XT90.
- **It is NOT a production layout**. You must replace placeholders with real footprints (LTC3895, FETs, inductors, caps), re-route with correct widths/clearances, and then generate Gerbers.

## Nets
- VIN, GND
- V48, V12, V5

## How to use
1. Open `hardware/kicad/24S-DCDC.kicad_pcb` in KiCad 7/8.
2. Replace placeholder footprints with real ones and import schematics/netlist.
3. Re-route power and high-speed loops, add planes/zones, clearances, and DRC rules.
4. Plot Gerbers/Drills via KiCad's `kicad-cli` or GUI.

> This file only serves as a *bridge* to get you unblocked while I prepare the full production layout offline.
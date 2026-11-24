# ISO Channel v0.99 — fabrication files

A small isolated output board for the HiPIMS controller. It drives the trigger inputs of oscilloscopes,
sensors and similar loads. Generated with KiCad 10.0.8 from `Channel.kicad_pcb`.

The fabrication files are in `gerber/`, and `gerber-iso-channel.zip` holds the same files.

## Board

| Parameter | Value |
|---|---|
| Layers | 2 |
| Size | 55.05 × 59.48 mm, rectangle |
| Thickness | 1.6 mm, FR4 |
| Copper | 35 µm (1 oz), both sides — the layer stack is not set in the design |
| Min track / clearance | 0.2 / 0.2 mm |
| Min drill | 0.3 mm (vias) |
| Vias (pad / drill) | 19 × 0.6 / 0.3, 1 × 0.8 / 0.4 mm |
| Plated holes | components 0.7–1.0 mm; 1 × 3.5 mm (mounting hole H4) |
| Non-plated holes | 3 × 3.5 mm (mounting holes H1–H3) — separate file |
| Slots / oblong holes | none |
| Components | top side only |
| Impedance control | not required |
| Surface finish, colours | not specified in the design — choose at order |

## Files

| File | Content |
|---|---|
| `Channel-F_Cu.gtl` | Top copper |
| `Channel-B_Cu.gbl` | Bottom copper |
| `Channel-F_Mask.gts` | Top solder mask |
| `Channel-B_Mask.gbs` | Bottom solder mask |
| `Channel-F_Silkscreen.gto` | Top silkscreen |
| `Channel-B_Silkscreen.gbo` | Bottom silkscreen (empty) |
| `Channel-F_Paste.gtp` | Top paste — stencil only |
| `Channel-B_Paste.gbp` | Bottom paste (empty) |
| `Channel-Edge_Cuts.gm1` | Board outline |
| `Channel-PTH.drl` | Plated holes, Excellon, metric |
| `Channel-NPTH.drl` | Non-plated holes, Excellon, metric |
| `Channel-job.gbrjob` | Gerber job file |
| `Channel-PTH-drl_map.gbr`, `Channel-NPTH-drl_map.gbr` | Drill maps — for reference only, not needed for fabrication |

Gerber RS-274X (X2 attributes), units mm, format 4.6. All layers share the same origin.

---
title: Gerber / Fabrication
---

## Downloads

<div class="btn-group">
  <a class="btn btn-primary" href="{{ '/assets/downloads/gerber.zip' | relative_url }}">
    <span class="btn-icon">&#11015;</span> Gerber Files (.zip)
  </a>
  <a class="btn btn-secondary" href="{{ '/assets/downloads/nc_drill.zip' | relative_url }}">
    <span class="btn-icon">&#11015;</span> NC Drill Files (.zip)
  </a>
  <a class="btn btn-secondary" href="{{ '/assets/downloads/odb.zip' | relative_url }}">
    <span class="btn-icon">&#11015;</span> ODB++ Package (.zip)
  </a>
</div>

## Layer Stack

| Layer | File Extension | Description |
|-------|---------------|-------------|
| Top Copper | `.GTL` | Top signal layer |
| Inner 1 | `.G1` | Inner signal/plane |
| Inner 2 | `.G2` | Inner signal/plane |
| Bottom Copper | `.GBL` | Bottom signal layer |
| Top Soldermask | `.GTS` | Top solder mask |
| Bottom Soldermask | `.GBS` | Bottom solder mask |
| Top Silkscreen | `.GTO` | Top overlay |
| Bottom Silkscreen | `.GBO` | Bottom overlay |
| Top Paste | `.GTP` | Top solder paste |
| Bottom Paste | `.GPB` | Bottom solder paste |
| Board Outline | `.GKO` | Keep-out / board edge |

## Fabrication Notes

<!-- Add any specific fabrication requirements here -->

| Parameter | Value |
|-----------|-------|
| Board thickness | <!-- 1.6mm --> |
| Surface finish | <!-- ENIG / HASL / OSP --> |
| Min trace width | <!-- 0.1mm --> |
| Min via drill | <!-- 0.2mm --> |
| Controlled impedance | <!-- Yes/No --> |

<div class="info-box note">
  Always verify the board outline and layer stack with your PCB manufacturer before ordering.
</div>

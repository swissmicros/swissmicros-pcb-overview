---
title: Bill of Materials
---

## Download

<div class="btn-group">
{% if site.bom_file %}
  <a class="btn btn-primary" href="{{ '/assets/downloads/' | append: site.bom_file | relative_url }}">
    <span class="btn-icon">&#11015;</span> Download BOM (.xlsx)
  </a>
{% else %}
  <div class="info-box warning">BOM not yet available for this release.</div>
{% endif %}
</div>

## Summary

<!-- Add component count summary here -->

| Category | Count |
|----------|-------|
| ICs / Active | <!-- --> |
| Resistors | <!-- --> |
| Capacitors | <!-- --> |
| Connectors | <!-- --> |
| Inductors / Ferrites | <!-- --> |
| **Total placements** | <!-- --> |

## Notes

<!-- Add any BOM-specific notes, e.g. approved substitutes, long-lead items -->

<div class="info-box note">
  The complete BOM with manufacturer part numbers and approved alternatives is in the downloaded Excel file.
</div>

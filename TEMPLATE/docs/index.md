---
title: Overview
---

## Project Summary

<!-- Add a brief description of this board -->

{% if site.project_description %}{{ site.project_description }}{% endif %}

{% if site.project_layers %}
**Layers:** {{ site.project_layers }}-layer PCB
{% endif %}

## Board Preview

{% if site.project_slug %}
<img src="{{ '/assets/images/' | append: site.project_slug | append: '.png' | relative_url }}"
     alt="{{ site.project_name }} board"
     style="max-width:100%;border:1px solid #e0d8ce;border-radius:4px;padding:8px;">
{% endif %}

## Quick Downloads

<div class="btn-group">
{% if site.pdf_schematic %}
<a class="btn btn-primary" href="{{ '/assets/downloads/' | append: site.pdf_schematic | relative_url }}">
  <span class="btn-icon">&#128196;</span> Schematics PDF
</a>
{% endif %}
{% if site.pdf_3d %}
<a class="btn btn-secondary" href="{{ '/assets/downloads/' | append: site.pdf_3d | relative_url }}">
  <span class="btn-icon">&#128247;</span> 3D View PDF
</a>
{% endif %}
{% if site.bom_file %}
<a class="btn btn-secondary" href="{{ '/assets/downloads/' | append: site.bom_file | relative_url }}">
  <span class="btn-icon">&#128202;</span> Bill of Materials
</a>
{% endif %}
<a class="btn btn-secondary" href="{{ '/assets/downloads/gerber.zip' | relative_url }}">
  <span class="btn-icon">&#128229;</span> Gerber Files
</a>
</div>

## Revision History

| Version | Date | Notes |
|---------|------|-------|
| <!-- Rev 1.0 --> | <!-- YYYY-MM-DD --> | Initial release |

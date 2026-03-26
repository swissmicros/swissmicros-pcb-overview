---
title: Schematics
---

{% if site.pdf_schematic %}
<div class="btn-group">
  <a class="btn btn-primary" href="{{ '/assets/downloads/' | append: site.pdf_schematic | relative_url }}">
    <span class="btn-icon">&#11015;</span> Download Schematic PDF
  </a>
  {% if site.pdf_3d %}
  <a class="btn btn-secondary" href="{{ '/assets/downloads/' | append: site.pdf_3d | relative_url }}">
    <span class="btn-icon">&#11015;</span> Download 3D View PDF
  </a>
  {% endif %}
</div>

<div class="pdf-container">
  <embed class="pdf-embed"
         src="{{ '/assets/downloads/' | append: site.pdf_schematic | relative_url }}#toolbar=1&navpanes=0"
         type="application/pdf">
  <div class="pdf-fallback">
    PDF preview not available in your browser.
    <a href="{{ '/assets/downloads/' | append: site.pdf_schematic | relative_url }}">Open PDF directly</a>
  </div>
</div>

{% else %}
<div class="info-box warning">
  Schematic PDF not yet available for this release.
</div>
{% endif %}

---
layout: default
title: PCB Projects
---

# SwissMicros PCB Projects

Internal hardware documentation for CalcBase PCB designs. Select a project to view schematics, gerber files, BOM, and assembly documentation.

<div class="project-grid">
{% for project in site.projects %}
<div class="project-card">
  <div class="card-header">{{ project.repo }}</div>
  <div class="card-body">
    <h3>{{ project.name }}</h3>
    <p>{{ project.description }}</p>
  </div>
  <div class="card-footer">
    {% if project.status == "released" %}
      <span class="status-badge released">Released</span>
    {% elsif project.status == "wip" %}
      <span class="status-badge wip">In Progress</span>
    {% else %}
      <span class="status-badge concept">Concept</span>
    {% endif %}
    {% if project.latest_release %}
      <span class="release-date">{{ project.latest_release }}</span>
    {% endif %}
    {% if project.url %}
      <a class="card-link" href="{{ project.url }}">View Docs &rarr;</a>
    {% else %}
      <span class="card-link" style="opacity:0.4;cursor:default;">No docs yet</span>
    {% endif %}
  </div>
</div>
{% endfor %}
</div>

---
layout: default
title: Airport Buffer Time Reference
description: Baseline airport arrival buffers by scenario. Add your ground transit time on top.
permalink: /airport-buffer-time/
---

<div class="page-hero">
  <h1>Airport Buffer Time Reference</h1>
  <p>Baseline airport arrival buffers by scenario. Add your ground transit time on top.</p>
</div>


<div class="page-shell">
<p><a class="btn btn-primary"
   href="https://tools.solotraveler.org/tools/airport-buffer-calculator/"
   target="_blank"
   rel="noopener">
  Open Airport Buffer Calculator →
</a></p>
  <div class="table-wrap" role="region" aria-label="Airport Buffer Time Reference table">
    <table>
      <thead>
        <tr>
          <th>Scenario</th>
          <th>Domestic (minutes)</th>
          <th>International (minutes)</th>
          <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.airport_buffer %}
        <tr>
          <td>{{ row["Scenario"] }}</td>
          <td>{{ row["Domestic (minutes)"] }}</td>
          <td>{{ row["International (minutes)"] }}</td>
          <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

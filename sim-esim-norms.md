---
layout: default
title: SIM / eSIM Norms by Region
description: High-level expectations for ID requirements and the easiest approach by region.
permalink: /sim-esim-norms/
---

<div class="page-hero">
  <h1>SIM / eSIM Norms by Region</h1>
  <p>High-level expectations for ID requirements and the easiest approach by region.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="SIM / eSIM Norms by Region table">
    <table>
      <thead>
        <tr>
        <th>Region</th>
    <th>ID requirement for SIM</th>
    <th>Prepaid SIM ease (1-5)</th>
    <th>eSIM availability (1-5)</th>
    <th>Best approach (typical)</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.sim_esim_norms %}
        <tr>
          <td>{{ row["Region"] }}</td>
      <td>{{ row["ID requirement for SIM"] }}</td>
      <td>{{ row["Prepaid SIM ease (1-5)"] }}</td>
      <td>{{ row["eSIM availability (1-5)"] }}</td>
      <td>{{ row["Best approach (typical)"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

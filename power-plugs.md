---
layout: default
title: Power Plugs + Voltage by Country
description: Outlet types, voltage, and frequency reference for travel adapters and electronics planning.
permalink: /power-plugs/
---

<div class="page-hero">
  <h1>Power Plugs + Voltage by Country</h1>
  <p>Outlet types, voltage, and frequency reference for travel adapters and electronics planning.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Power Plugs + Voltage by Country table">
    <table>
      <thead>
        <tr>
        <th>Country</th>
    <th>Plug type(s)</th>
    <th>Voltage (V)</th>
    <th>Frequency (Hz)</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.power_plugs %}
        <tr>
          <td>{{ row["Country"] }}</td>
      <td>{{ row["Plug type(s)"] }}</td>
      <td>{{ row["Voltage (V)"] }}</td>
      <td>{{ row["Frequency (Hz)"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

---
layout: default
title: Emergency Numbers by Country
description: Police, ambulance, and fire emergency numbers for common destinations. Always verify locally when possible.
permalink: /emergency-numbers/
---

<div class="page-hero">
  <h1>Emergency Numbers by Country</h1>
  <p>Police, ambulance, and fire emergency numbers for common destinations. Always verify locally when possible.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Emergency Numbers by Country table">
    <table>
      <thead>
        <tr>
        <th>Country</th>
    <th>Police</th>
    <th>Ambulance</th>
    <th>Fire</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.emergency_numbers %}
        <tr>
          <td>{{ row.Country }}</td>
      <td>{{ row.Police }}</td>
      <td>{{ row.Ambulance }}</td>
      <td>{{ row.Fire }}</td>
      <td>{{ row.Notes }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

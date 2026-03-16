---
layout: default
title: Carry-on Limits Cheat Sheet (Major Airlines)
description: Quick reference to carry-on size/weight and personal item allowances for major airlines.
permalink: /carry-on-limits/
---

<div class="page-hero">
  <h1>Carry-on Limits Cheat Sheet (Major Airlines)</h1>
  <p>Quick reference to carry-on size/weight and personal item allowances for major airlines.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Carry-on Limits Cheat Sheet (Major Airlines) table">
    <table>
      <thead>
        <tr>
          <th>Airline</th>
          <th>Region</th>
          <th>Carry-on size (cm)</th>
          <th>Carry-on weight</th>
          <th>Personal item</th>
          <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.carryon_limits %}
        <tr>
          <td>{{ row["Airline"] }}</td>
          <td>{{ row["Region"] }}</td>
          <td>{{ row["Carry-on size (cm)"] }}</td>
          <td>{{ row["Carry-on weight"] }}</td>
          <td>{{ row["Personal item"] }}</td>
          <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

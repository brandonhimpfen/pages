---
layout: default
title: Transit Safety Norms
description: A practical reference for what’s normal (and what’s not) when traveling solo using local transit, taxis, and intercity transport.
permalink: /transit-safety-norms/
---

<div class="page-hero">
  <h1>Transit Safety Norms</h1>
  <p>A practical reference for what’s normal (and what’s not) when traveling solo using local transit, taxis, and intercity transport.</p>
</div>

<div class="page-shell">

  <div class="table-wrap" role="region" aria-label="Transit Safety Norms table">
    <table>
      <thead>
        <tr>
        <th>Context</th>
    <th>Norm (what’s typical)</th>
    <th>Risk flags</th>
    <th>Safer default</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.transit_safety_norms %}
        <tr>
          <td>{{ row["Context"] }}</td>
      <td>{{ row["Norm (what’s typical)"] }}</td>
      <td>{{ row["Risk flags"] }}</td>
      <td>{{ row["Safer default"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

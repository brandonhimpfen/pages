---
layout: default
title: Medication Naming Differences
description: Common medication name differences you’ll see while traveling (e.g., acetaminophen vs paracetamol).
permalink: /medication-naming-differences/
---

<div class="page-hero">
  <h1>Medication Naming Differences</h1>
  <p>Common medication name differences you’ll see while traveling (e.g., acetaminophen vs paracetamol).</p>
</div>

<div class="page-shell">

  <div class="table-wrap" role="region" aria-label="Medication Naming Differences table">
    <table>
      <thead>
        <tr>
        <th>Medication (common name)</th>
    <th>Also known as</th>
    <th>Region notes</th>
    <th>Common use notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.medication_naming %}
        <tr>
          <td>{{ row["Medication (common name)"] }}</td>
      <td>{{ row["Also known as"] }}</td>
      <td>{{ row["Region notes"] }}</td>
      <td>{{ row["Common use notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

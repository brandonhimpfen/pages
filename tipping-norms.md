---
layout: default
title: Tipping Norms Quick Reference
description: Common tipping expectations for restaurants and taxis. Practices vary by city and context.
permalink: /tipping-norms/
---

<div class="page-hero">
  <h1>Tipping Norms Quick Reference</h1>
  <p>Common tipping expectations for restaurants and taxis. Practices vary by city and context.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Tipping Norms Quick Reference table">
    <table>
      <thead>
        <tr>
        <th>Country</th>
    <th>Restaurants</th>
    <th>Taxi</th>
    <th>Rounded/Other</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.tipping %}
        <tr>
          <td>{{ row["Country"] }}</td>
      <td>{{ row["Restaurants"] }}</td>
      <td>{{ row["Taxi"] }}</td>
      <td>{{ row["Rounded/Other"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

---
layout: default
title: Solo Traveler Etiquette Reference
description: "Lightweight social defaults for solo travelers: small situations that come up often, and simple ways to navigate them."
permalink: /solo-traveler-etiquette/
---

<div class="page-hero">
  <h1>Solo Traveler Etiquette Reference</h1>
  <p>Lightweight social defaults for solo travelers: small situations that come up often, and simple ways to navigate them.</p>
</div>

<div class="page-shell">

  <div class="table-wrap" role="region" aria-label="Solo Traveler Etiquette Reference table">
    <table>
      <thead>
        <tr>
        <th>Situation</th>
    <th>What often happens</th>
    <th>Good default response</th>
    <th>Why it works</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.solo_etiquette %}
        <tr>
          <td>{{ row["Situation"] }}</td>
      <td>{{ row["What often happens"] }}</td>
      <td>{{ row["Good default response"] }}</td>
      <td>{{ row["Why it works"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

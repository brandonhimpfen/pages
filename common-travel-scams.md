---
layout: default
title: Common Travel Scams (Region Reference)
description: Patterns to watch for. Not fear-based, just the common repeats and how to respond.
permalink: /common-travel-scams/
---

<div class="page-hero">
  <h1>Common Travel Scams (Region Reference)</h1>
  <p>Patterns to watch for. Not fear-based, just the common repeats and how to respond.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Common Travel Scams (Region Reference) table">
    <table>
      <thead>
        <tr>
        <th>Region</th>
    <th>Scam type</th>
    <th>Where it happens</th>
    <th>What it looks like</th>
    <th>What to do</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.common_scams %}
        <tr>
          <td>{{ row["Region"] }}</td>
      <td>{{ row["Scam type"] }}</td>
      <td>{{ row["Where it happens"] }}</td>
      <td>{{ row["What it looks like"] }}</td>
      <td>{{ row["What to do"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

---
layout: default
title: Visa-free Stay Lengths (Top Destinations)
description: High-level reference for visa-free or authorization-based tourist stays for common passport holders.
permalink: /visa-free-stays/
---

<div class="page-hero">
  <h1>Visa-free Stay Lengths (Top Destinations)</h1>
  <p>High-level reference for visa-free or authorization-based tourist stays for common passport holders.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Visa-free Stay Lengths (Top Destinations) table">
    <table>
      <thead>
        <tr>
        <th>Passport</th>
    <th>Destination</th>
    <th>Visa-free/visa-on-arrival</th>
    <th>Max stay (days)</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.visa_free %}
        <tr>
          <td>{{ row["Passport"] }}</td>
      <td>{{ row["Destination"] }}</td>
      <td>{{ row["Visa-free/visa-on-arrival"] }}</td>
      <td>{{ row["Max stay (days)"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

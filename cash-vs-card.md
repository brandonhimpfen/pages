---
layout: default
title: Cash vs Card Practicality by Country
description: A quick sense check for how cash-heavy a place tends to be, plus ATM reliability.
permalink: /cash-vs-card/
---

<div class="page-hero">
  <h1>Cash vs Card Practicality by Country</h1>
  <p>A quick sense check for how cash-heavy a place tends to be, plus ATM reliability.</p>
</div>

<div class="page-shell">
  <div class="table-wrap" role="region" aria-label="Cash vs Card Practicality by Country table">
    <table>
      <thead>
        <tr>
        <th>Country/Region</th>
    <th>Card acceptance (1-5)</th>
    <th>Cash needed (1-5)</th>
    <th>ATM access (1-5)</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.cash_vs_card %}
        <tr>
          <td>{{ row["Country/Region"] }}</td>
      <td>{{ row["Card acceptance (1-5)"] }}</td>
      <td>{{ row["Cash needed (1-5)"] }}</td>
      <td>{{ row["ATM access (1-5)"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

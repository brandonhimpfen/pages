---
layout: default
title: Embassy / Consulate Official Links Directory
description: Official sources for travel advisories, consular help, and embassy/consulate locators. (Links only; not a full directory.)
permalink: /embassy-links/
---

<div class="page-hero">
  <h1>Embassy / Consulate Official Links Directory</h1>
  <p>Official sources for travel advisories, consular help, and embassy/consulate locators. (Links only; not a full directory.)</p>
</div>

<div class="page-shell">
  <p class="small">Tip: bookmark your home country’s embassy locator before you travel.</p>
  <div class="table-wrap" role="region" aria-label="Embassy / Consulate Official Links Directory table">
    <table>
      <thead>
        <tr>
        <th>Country/Region</th>
    <th>Official travel advice</th>
    <th>Embassy/consulate locator</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.embassy_links %}
        <tr>
          <td>{{ row["Country/Region"] }}</td>
      <td>{{ row["Official travel advice"] }}</td>
      <td>{{ row["Embassy/consulate locator"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

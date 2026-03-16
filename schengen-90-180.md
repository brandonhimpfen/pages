---
layout: default
title: Schengen 90/180 Reference + Examples
description: A simplified reference for the Schengen short-stay rule (90 days in any rolling 180-day period).
permalink: /schengen-90-180/
---

<div class="page-hero">
  <h1>Schengen 90/180 Reference + Examples</h1>
  <p>A simplified reference for the Schengen short-stay rule (90 days in any rolling 180-day period).</p>
</div>

<div class="page-shell">
  <p class="small"><strong>Reminder:</strong> this is a reference page, not legal advice. Always verify current immigration rules for your nationality.</p>
  <div class="table-wrap" role="region" aria-label="Schengen 90/180 Reference + Examples table">
    <table>
      <thead>
        <tr>
        <th>Example</th>
    <th>Planned days in Schengen</th>
    <th>Rolling 180-day logic (summary)</th>
    <th>Result</th>
    <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        {% for row in site.data.schengen_90_180 %}
        <tr>
          <td>{{ row["Example"] }}</td>
      <td>{{ row["Planned days in Schengen"] }}</td>
      <td>{{ row["Rolling 180-day logic (summary)"] }}</td>
      <td>{{ row["Result"] }}</td>
      <td>{{ row["Notes"] }}</td>
        </tr>
        {% endfor %}
      </tbody>
    </table>
  </div>
  <p class="small">Last updated: {% assign today = "now" | date: "%Y-%m-%d" %}{{ today }}</p>
</div>

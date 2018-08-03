---
title: Player Rankings
keywords: Tournament Players Rankings Database
sidebar: ch_sidebar
permalink: tmx_players_rankings.html
toc: false
---

### Points Tables

Player Rankings are available when [Organization Keys](tmx_configuration.html) include __Points Tables__.

### Generating

Generating Ranking Lists is a two step process
* Calculate Ranking Points for all players for a selected date
* Generate Ranking List for a selected date

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'> {% include image.html file="ch_rankings_calculate.png" alt="Calculate" caption="Calculate" %}</div>
   {% include image.html file="ch_rankings_generate.png" alt="Generate" caption="Generate" %}
</div>

### Rank Lists
Rank Lists are generated for all Player Categories which have been defined by an [Organization Key](tmx_configuration.html) and are exportable in multiple formats including PDF, CSV, JSON and XLSX.

{% include image.html file="ch_rankings_lists.png" alt="Rank Lists" caption="Rank Lists" %}

### Rankings Charts

After Rank Lists have been generated, Rankings Charts are available for all players.

Datapoints represent each date chosen for Rank List generation.

{% include image.html file="ch_rankings_chart.png" alt="Rankings Chart" caption="Rankings Chart" %}

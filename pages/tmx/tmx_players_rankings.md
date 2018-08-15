---
title: Žebříčky hráčů
keywords: Tournament Players Rankings Database
sidebar: ch_sidebar
permalink: tmx_players_rankings.html
toc: false
---

### Tabulky bodů

Žebříčky hráčů jsou dostupné když [Organizační klíč](tmx_configuration.html) obsahuje __Tabulky bodů__.

### Sestavování žebříčků

Sestavování žebříčků je dvoustupňový proces
* výpočet bodů do žebříčku pro všechny hráče k vybranému datu
* sestavování žebříčku hráčů k vybranému datu

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'> {% include image.html file="ch_rankings_calculate.png" alt="Vypočítat" caption="Vypočítat" %}</div>
   {% include image.html file="ch_rankings_generate.png" alt="Sestavovat" caption="Sestavovat" %}
</div>

### Žebříčky
Žebříčky jsou sestavovány pro všechny hráčské kategorie které byly definovány v [Organizačním klíči](tmx_configuration.html) a lze je exportovat do
mnoha formátů včetně PDF, CSV, JSON and XLSX.

{% include image.html file="ch_rankings_lists.png" alt="Žebříčky" caption="Žebříčky" %}

### Žebříčkové grafy

Po sestavení žebříčků jsou k dispozici i žebříčkové grafy pro všechny hráče.

Body k jednotlivým datům představují každé vybrané datum pro generovaný žebříček.

{% include image.html file="ch_rankings_chart.png" alt="ˇŽebříčkové grafy" caption="Žebříčkové grafy" %}

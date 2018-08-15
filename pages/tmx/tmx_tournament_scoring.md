---
title: Zadávání výsledků
keywords: Scoring Matches
sidebar: ch_sidebar
permalink: tmx_tournament_scoring.html
toc: true
---

Jakmile je hrací plán vytvořen tak je možno zadávat výsledky jednotlivých utkání.

Výsledky mohou být zadávány přímo do hracích plánů a skupin, v záložce [Seznam utkání](tmx_tournament_matches.html) nebo v [Rozpisu utkání](tmx_tournament_schedule.html).

## Eliminační hrací plány

Po vytvoření eliminačního hracího plánu jsou utkání, u kterých může být zadán výsledek, zvýrazněna.

{% include image.html file="ch_scoring_elimination_positions.png" alt="Zvýrazněná utkání" caption="Zvýrazněná utkání" %}

## Skupinové hrací plány

Pozice, kam můžou být zadány výsledky jsou zvýrazněny _modře_ pokud se nad nimi pohybuje kurzorem.

Pozice, kam výsledek nemůže být zadán kvůli volnému kolu (Byes), jsou zbarveny světle žlutě.

{% include image.html file="ch_scoring_rr_positions.png" alt="Zvýrazněná utkání" caption="Zvýrazněná utkání" %}

## Zápis výsledku

Metoda zápisu výsledku je stejná pro všechny soutěže.

Activní buňky výběru skóre jsou __bílé__ a slouží k zápisu počtu her ke každému hráči.

{% include image.html file="ch_scoring_entry.png" alt="Zápis výsledku" caption="Zápis výsledku" %}

### Formát skóre
Ke změně formátu výsledku pro jednotlivá utkání je třeba kliknout na ikonu v pravém horním rohu okna pro zadávání výsledků a změnit __formát skóre__.

{% include image.html file="ch_scoring_configuration.png" alt="Formát skóre" caption="Formát skóre" %}

### Automatické dokončování

Pro každý set je třeba zadat pouze jednu hodnotu, a to nižší počet her u hráče který set prohrál.

{% include image.html file="ch_scoring_games.png" alt="Zadávání počtu her" caption="Zadávání počtu her" %}

Systém automaticky doplní druhý počet her které vyhrál druhý hráč a skóre se automaticky posune k zadání dalšího setu pokud není zápis výsledku ukončen.

{% include image.html file="ch_scoring_first_set.png" alt="Skóre 1.setu" caption="Skóre 1.setu" %}

### Změna skóre v setu

Pokud je třeba změnit výsledek v setu, kliknutí na skóre v setu u příslušného hráče znovu zobrazí okno pro výběr hodnoty / počtu her v tomto setu.

{% include image.html file="ch_scoring_edit_first_set.png" alt="Změna skóre v setu" caption="Změna skóre v setu" %}

### Nedokončená utkání, vzdání, skreče, postup bez boje a diskvalifikace

Kliknutí na zelenou __pomlčku__ "-" vpravo zobrazí volby pro zápis výsledku nedokončeného utkání jako je skreč, vzdání (Retirement), postup bez boje (Walkover) nebo diskvalifikace (Default), tak jako volbu označit utkání jako __přerušené (Interrupted)__ nebo __živé (Live)__.

{% include image.html file="ch_scoring_options.png" alt="Volby skóre" caption="Volby skóre" %}

### Akceptace výsledku utkání

Až je zápis výsledku ukončen, tak se kliknutím na tlačítko __"Akceptovat"__ výsledek uloží.

{% include image.html file="ch_scoring_live.png" alt="Akceptace skóre" caption="Akceptace skóre" %}

### Editace výsledku

Výsledek utkání může být editován kliknutím na __existující skóre__.

{% include image.html file="ch_scoring_incomplete.png" alt="Editace skóre" caption="Editace skóre" %}

Jakmile je výsledek utkání zadán, tak je umožněn zápis skóre pro následující utkání (pokud jsou oba hráči známi).

{% include image.html file="ch_scoring_complete.png" alt="Skóre dokončeno" caption="Skóre dokončeno" %}

### Odstranění utkání

Výsledek utkání může být odstraněn z hracího plánu pomocí [kontextového  kliknutí](tmx_fundamentals.html).

Výsledek utkání je také odstraněn když je skóre _vyčištěno_ v okně pro zadávání výsledků.

{% include image.html file="ch_scoring_remove.png" alt="Odstranit utkání" caption="Odstranit utkání" %}

### Výsledek tie-breaku

Zápis výsledku tie-breaku je podobný jako zadání výsledku v setu jen s tím rozdílem, že do vstupního pole musí být manuálně zadán výsledek tie-breaku místo výběru hodnoty (stačí zadat nižší počet bodů u hráče který tie-break prohrál).

{% include image.html file="ch_scoring_tiebreak.png" alt="Skóre tie-breaku" caption="Skóre tie-breaku" %}

{% include important.html content='Jelikož jsou použita vstupní pole pro zadání výsledku tie-breaku, tak stisk klávesy __Enter/Return__ _je nutný_ k dokončení zápisu skóre.' %}

{% include image.html file="ch_scoring_winner.png" alt="Vítěz utkání" caption="Vítěz utkání" %}

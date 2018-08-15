---
title: Turnajové hrací plány
keywords: tournament draws
sidebar: ch_sidebar
permalink: tmx_tournament_draws.html
toc: true
---

## Akční ikony

V záložce __Hrací plány__ napravo od __výběru soutěže__ je několik "akčních ikon":

{% include image.html file="ch_draws_tab.png" alt="Hrací plány" caption="Záložka hrací plány" %}

* __Ikona Vyčistit hrací plán:__ znovu obnoví (resetuje) vybraný hrací plán
* __Ikona Zástupci hráčů:__ identifikuje zástupce hráčů, kteří byli přítomni losování
* __Ikona PDF:__ vytvoří PDF soubor s hracím plánem a pořadím hráčů, kompletním hracím plánem a Lucky Loser přihláškami

### Opětovné vytvoření hracího plánu

Pokud je z nějakého důvodu třeba vytvořit hrací plán od samého začátku, ikona __Vyčistit hrací plán__ obnoví hrací plán do počátečního stavu.

{% include note.html content='Ikona __Vyčistit hrací plán__ není k dispozici pokud byl zadán alespoň jeden výsledek utkání.' %}

### Zástupci hráčů

Ikona __Zástupci hráčů__ spustí dialogové okno kam je možno zadat maximálně dva hráče kteří byli přítomni losování hracího plánu.

{% include image.html file="ch_draws_player_representatives.png" alt="Zástupci hráčů" caption="Zástupci hráčů" %}

Zástupcí hráčů se objeví dole na PDF výtisku příslušného hracího plánu.

### Pořadí hráčů pro hrací plán

Pokud nebyl hrací plán ještě dokončen (všichni hráči umístěni), pak __PDF ikona__ vytvoří PDF soubor s __pořadím hráčů pro hrací plán__, což je tabulka hráčů seřazených podle jejich žebříčku.

Tato tabulka hráčů se použije k [manuální tvorbě hracího plánu](tmx_tournament_draws.html#manual-draw-creation) a nebude vytvořena když je hrací plán sestaven  [automaticky](tmx_events_management.html#automated-draws).

{% include image.html file="ch_draws_draw_order.png" alt="Pořadí hráčů" caption="Pořadí hráčů pro hrací plán" %}

## Vyřazovací hrací plány

Když je hrací plán vytvářen [automaticky](tmx_events_management.html#automated-draws), pak jsou všichni hráči umístěni na řádky hracího plánu bez manuálního zásahu automaticky a hrací plán je připraven k zadávání [výsledků](tmx_tournament_scoring.html).

{% include image.html file="ch_draws_main.png" alt="Hlavní hrací plán" caption="Automaticky vytvořený hrací plán" %}

### Výměna pozic, náhradníci, Lucky Losers (Šťastní Poražení)

Jakmile je hrací plán vytvořen, [kontextové kliknutí](tmx_fundamentals.html) na hráče vyvolá okno s nabídkou dostupných možností.

{% include image.html file="ch_draws_player_options.png" alt="Možnosti" caption="Hráčské možnosti" %}

Je-li __nasazený hráč__ vyměněn v hracím plánu s __nenasazeným hráčem__, nebo nahrazen __náhradníkem__ či __Lucky Loserem__, pak je informace o nasazení hráče odstraněna.

{% include image.html file="ch_draws_player_replacement.png" alt="Nahrazení" caption="Nahrazení hráče" %}

### Manuální vytvoření hracího plánu

I když je hrací plán tvořen manuálně, tak 1. a 2. nasazený hráč je vždy umístěn do hracího plánu automaticky.

Ostatní nasazení hráči jsou umísťování v "nasazovacích skupinách".  Třetí a čtvrtý nasazení jsou společně v jedné nasazovací skupině. Další nasazovací skupina, pokud je třeba, by byla z nasazených hráčů č.5, 6, 7 and 8 atd.

Hráči mohou být na hrací plán umísťování třemi způsoby:
* zadáním __pořadí hráče pro hrací plán__
* vyhledáním hráče podle jména
* vybráním hráče ze seznamu dostupných hráčů

{% include image.html file="ch_draws_player_selection.png" alt="Výběr hráče" caption="Výběr hráče" %}

První dvě volby jsou dostupné kliknutím na příslušnou pozici v hracím plánu:

[Kontextové kliknutí](tmx_fundamentals.html) na příslušnou pozici hracího plánu vyvolá seznam dostupných hráčů a umožní jejich umístění v hracím plánu:

{% include image.html file="ch_draws_player_selection_context.png" alt="Výběr nasazeného hráče" caption="Manuální výběr nasazeného hráče" %}

### Odstranění hráčů

{% include image.html file="ch_draws_manual_remove.png" alt="Odstranit hráče" caption="Odstranit hráče" %}

Hráči mohou být odstraněni pomocí [kontextového kliknutí](tmx_fundamentals.html) na své jméno.

{% include important.html content='Jakmile je hrací plán vytvořen a všichni hráči jsou umístěni pak mohou být hráči jen vyměněni nebo nahrazeni náhradníky či  Lucky Losers.' %}

## Skupinový hrací plán

Je-li hrací plán vytvořen [automaticky](tmx_events_management.html#automated-draws), pak jsou všichni hráči umístěni na řádky hracího plánu systémem bez manuálního zásahu a hrací plán je připraven k zadávání [výsledků](tmx_tournament_scoring.html).

{% include image.html file="ch_draws_rr_automated.png" alt="Automatický hrací plán" caption="Vytvoření hracího plánu automaticky" %}

### Manuální umístění hráčů

Jsou-li skupiny vytvářeny manuálně, pak jsou hráči umísťováni stejným způsobem jako v [jiných hracích plánech](tmx_tournament_draws.html#manual-draw-creation), pomocí normálního kliknutí nebo [kontextového kliknutí](tmx_fundamentals.html) na příslušnou pozici v hracím plánu.

Ve výchozím nastavení jsou v každé skupině dva nasazení hráči.  Toto nastavení může být změněno pomocí [konfiguračního klíče](tmx_configuration.html).

{% include tip.html content='Ve skupinovém hracím plánu jsou platné pozice na hracím plánu zvýrazněny když se kurzor myši umístí nad skupinou.' %}

{% include image.html file="ch_draws_rr_player_placement.png" alt="Umístit hráče" caption="Platná pozice hracího plánu" %}

[Kontextové kliknutí](tmx_fundamentals.html) může byt také použito k odstranění hráče a jeho nahrazením dostupným náhradníkem.

{% include image.html file="ch_draws_rr_player_options.png" alt="Volby hráče" caption="Volby hráče" %}

### Poměr výher

Až když jsou [výsledky](tmx_tournament_scoring.html) kompletní, tak je sloupec s __pořadím ve skupině (#)__ označen pokud mají hráči stejný __poměr výher__.

{% include image.html file="ch_draws_rr_sub_order.png" alt="POmocné pořadí" caption="Pomocné pořadí ve skupině" %}

[Kontextové kliknutí](tmx_fundamentals.html) na buňky v __+/-__ sloupci zobrazí hráčův __poměr výher__.

{% include image.html file="ch_draws_rr_ratios.png" alt="Poměr výher" caption="Poměr výher" %}

[Kontextové kliknutí](tmx_fundamentals.html) na označenou buňku nastaví "pomocné pořadí", které je použito pro určení pořadí ve skupině a případný postup ze skupiny do dalších utkání v turnaji.

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'>{% include image.html file="ch_draws_rr_sub_order_selection.png" alt="Pomocné pořadí" caption="Výběr pomocného pořadí" %}</div>
   {% include image.html file="ch_draws_rr_sub_order_defined.png" alt="Definice pomocného pořadí" caption="Definice pomocného pořadí" %}
</div>

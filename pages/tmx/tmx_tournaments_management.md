---
title: Správa turnajů
keywords: Tournament Calendar Management
sidebar: ch_sidebar
permalink: tmx_tournaments_management.html
toc: true
---

## Synchronizace turnajů

Je-li [vyhledávací pole](tmx_searchbox.html) v turnajovém režimu, tak je počet turnajů v kalendáři zobrazen vpravo nahoře od navigační lišty. (Viz [Používání vyhledávacího pole](tmx_fundamentals.html) k návodu jak změnit režim vyhledávání).

Podržením kurzoru vlevo od ikony turnaje s počtem turnajů zobrazí ikonu __Obnovení databáze__.  Pokud je CourtHive/TMX nakonfigurován k synchronizaci s externí databází organizace, turnaje mohou být načteny ze vzdáleného serveru.

{% include image.html file="ch_tournaments_count.png" alt="Vyhledávání turnajů" caption="Režim vyhledávání turnajů" %}

Kliknutí na ikonu __Obnovení databáze__ načte nové turnaje které vznikly *po* posledním zápisu v lokálním kalendáři turnajů.

["Kontextové kliknutí"](tmx_fundamentals.html) na ikonu __Obnovení databáze__ načte celý kalendář turnajů ze serveru a přidá turnaje které chybí v lokální databázi.

## Manuální přidání turnaje

V kalendáři turnajů, napravo od filtru věkové kategorie, je ikona __Přidat turnaj__.

{% include image.html file="ch_add_tournament_icon.png" alt="Přidat turnaj" caption="Přidat turnaj" %}

Kliknutí na ikonu __Přidat turnaj__ otevře dialogové okno pro zadání informací o novém turnaji.  

Pole označená __žlutě__ musí být vyplněna předtím než dojde k uložení turnaje.

<div style='display: flex; flex-wrap: wrap;'>
   {% include image.html file="ch_add_tournament.png" alt="Přidat turnaj" %}
   {% include image.html file="ch_challenge.png" alt="Přidat turnaj" %}
</div>

{% include image.html file="ch_challenge_calendar.png" alt="Turnaj přidán" %}

{% include note.html content='Pro schválené organizace, ["kontextové kliknutí"](tmx_fundamentals.html) na ikonu __Přidat turnaj__ zobrazí okno pro zadání __kódového čísla turnaje__ k načtení turnajových dat přímo ze vzdáleného zdroje.' %}

## Smazání a editace turnaje

["Kontextové kliknutí"](tmx_fundamentals.html) na jakýkoli turnaj zobrazí možnosti buďto editovat nebo smazat turnaj.

{% include image.html file="ch_tournament_delete.png" alt="Smazat turnaj" caption="Editovat nebo smazat turnaj" %}

Výběr editace turnaje otevře stejné dialogové okno jako při přidání turnaje s možností změnit nebo doplnit zadané hodnoty.

{% include note.html content='Pro schválené organizace existuje navíc volba "Spojit" turnaje, která má efekt spojení seznamu všech registrovaných hráčů do jednoho pod jeden turnaj.' %}

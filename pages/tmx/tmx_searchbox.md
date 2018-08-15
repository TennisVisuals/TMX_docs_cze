---
title: Používání vyhledávacího pole
keywords: Searching
sidebar: ch_sidebar
permalink: tmx_searchbox.html
toc: true
---
CourtHive/TMX vyhledávací pole může být použito k vyhledání hráčů, turnajů a klubů.  

{% include important.html content="Pokud diakritika __není__ zapnuta v [Nastavení](tmx_setup.html) pak použijte např.'S' místo 'Š'." %}

{% include tip.html content="Chcete-li změnit režim vyhledávání, klikněte na 'zvětšovací lupu' ve vyhledávacím poli." %}

Ikona napravo od vyhledávacího pole závisí na zapnutém režimu vyhledávání a zobrazuje počet hráčů, turnajů a klubů uložených v lokální databázi.

{% include image.html file="ch_search_players.png" alt="Vyhledávat hráče" caption="Vyhledávat hráče" %}

Výchozím nastavením vyhledávacího pole je vyhledávání hráčů a výchozím nastavením pořadí vyhledávání je Jméno / Příjmení.  Pořadí vyhledávání lze změnit kontextovým kliknutím ve vyhledávacím poli.

{% include image.html file="ch_search_order.png" alt="Pořadí vyhledávání" caption="Kontextové kliknutí ke změně pořadí vyhledávání" %}

Při editaci turnaje může vyhledávací pole změnit své chování. Během fáze přihlašování hráčů se používá k přidání hráčů kteří nebyli předtím registrováni nebo k přihlášení (a odhlášení) registrovaných hráčů. Při vytváření soutěží se vyhledávací pole využívá ke schvalování hráčů a k vytváření dvojic pro čtyřhru.

Další informace o chování vyhledávacího pole mohou být nalezeny v odpovídajících sekcích této dokumentace.

## Režim vyhledávaní

Kliknutím na vyhledávací lupu ve vyhledávacím poli se změní režim vyhledávání.  

{% include image.html file="ch_search_tournaments.png" alt="Vyhledat turnaj" caption="Režim vyhledání turnaje" %}

## Kontextové sensitivní vyhledávání

Chování vyhledávacího pole se během některých operací mění.

* Při __přidávání__ hráčů do turnaje budou vyhledáni pouze hráči pro danou věkovou kategorii
* Při __schvalování__ hráčů pro turnajovou soutěž pouze hráči přihlášení do soutěže budou vyhledáni

{% include image.html file="ch_search_add_player.png" alt="Přidat hráče" caption="Přidat hráče" %}

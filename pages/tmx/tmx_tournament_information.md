---
title: Turnajová data
keywords: tournament information
sidebar: ch_sidebar
permalink: tmx_tournament_information.html
toc: true
---

## Úvod

Informace o turnaji se primárně používají při tisku / ukládání PDF seznamu přihlášených hráčů, soutěžních hracích plánů a turnajových rozpisů utkání.  

Datumy __začátku__ a __konce__ turnaje určí dny kdy mohou být soutěže v rámci turnaje naplánovány.

{% include image.html file="ch_challenge_edit.png" alt="Přidat hráče" caption="Editovací režim turnaje" %}

## Uložení turnajových dat

Turnajová data se při změnách automaticky ukládají do lokálního úložiště v prohlížeči.  Jsou dva způsoby jak zálohovat turnajová data a jak sdílet tato data s ostatními.

{% include image.html file="ch_tournaments_save.png" alt="Uložit turnaj" caption="Možnosti uložení" %}

Šipka __Nahoru__ exportuje / odesílá __turnajová data__ na [CourtHive Cloud Server](tmx_cloud_server.html) z kterého mohou být následně stažena jakýmkoli jiným uživatelem který má turnaj ve svém kalendáři.

Šipka __Dolů__ importuje / stahuje __turnajová data__ v JSON formátu do lokálního úložiště na disku. Tento soubor může být importován do CourtHive/TMX pomocí přetažení do Import/Export cílové zóny.

{% include image.html file="ch_tournaments_save_state.png" alt="Stav zálohování" caption="Stav zálohování" %}

"Export / Push" a "Import / Pull" ikony mění barvu tak aby signalizovala jestli byly nějaké změny provedeny v lokální kopii turnaje od doby kdy byl turnaj naposledy odeslán či stažen.

__Žlutá__ signalizuje "Neaktuální" a __zelená__ označuje "aktuální".

{% include note.html content='Když jsou turnajové soutěže dokončeny, turnajová data jsou automaticky odeslána na server.' %}

## Turnajové poznámky

Turnajové poznámky lze použít pouze pokud je [zveřejňování](tmx_publishing_overview.html) povoleno.

{% include image.html file="ch_tournament_notes_edit.png" alt="Poznámky" caption="Editace turnajových poznámek" %}

Turnajové poznámky jsou "dezinfikovány", aby se zabránilo [XSS útokům](https://en.wikipedia.org/wiki/Cross-site_scripting); to znamená, že pouze podskupina HTML kódů je povolena.

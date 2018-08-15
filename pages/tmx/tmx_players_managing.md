---
title: Správa databáze hráčů
keywords: Tournament Players Database
sidebar: ch_sidebar
permalink: tmx_players_managing.html
toc: false
---

Podpora správy lokální databáze hráčů v prvním vydání CourtHive/TMX je minimální.

Při běžném používání organizacemi které nakonfigurovaly TMX k propojení se svými existujícími systému pro registraci hráčů na turnaje, se lokální databáze hráčů
využívá primárně k usnadnění přidání hráčú kteří se přihlásili dodatečně na místě k účasti.

Pro jednotlivce nebo kluby, kdo pořádají turnaje nezávisle na externím turnajovém registračním systému, použití lokální databáze hráčů znamená,
že informace o hráčích je třeba zadat pouze jednou.

V současnosti není možno editovat hráče kteří byli importováni. Předpokládá se, že data hráčů jsou spravována externě a importována pouze za účelem usnadnění
zadávání hráčů pro vytvářené turnaje.  Verze 2.x se bude více integrovat s komponenty třetích stran které spravují data hráčů.

## Přidání hráčů

Hráči mohou být přidáni třemi způsoby do lokální CourtHive/TMX databáze.

### Vzdálená synchronizace databáze

Pokud je CourtHive/TMX nakonfigurován [Organizačním klíčem](tmx_configuration.html) pak může být databáze hráčů načtena umístěním kurzoru myši vlevo vedle ikony __Počet hráčů__ v pravém horním rohu, poté kontextovým kliknutím k zobrazení dialogu a potvrzením obnovení databáze (nebo přímým normálním kliknutím vlevo vedle ikony pro počet hráčů).

{% include image.html file="ch_players_refresh.png" alt="Hráči" caption="Obnovit databázi" %}

Po úspěšném načtení databáze hráčů se __počet hráčů__ změní tak, aby odrážel skutečný počet hráčů v lokální databázi.

### Chyť/Pusť Import

Pro hromadné načtení databáze hráčů tam kde není k dispozici vzdáleně přístupná databáze byla vytvořena __Tabulková šablona__.

Tato šablona, jakmile je naplněna daty s hráči, může být načtena ze souborového systému, nebo "chycena" a "puštěna" (Drag & Drop) v oblasti pro import dat,
jenž je přístupná kliknutím na __Import/Export__ ikonu z domovské stránky.

__Tabulkovou šablonu__ lze stáhnout z __Import/Export__ stránky kliknutím na ikonu tabulky.

<div style='display: flex; flex-wrap: wrap;'>
<div style='padding-right: 1em;'>{% include image.html file="ch_import_export.png" alt="Import" caption="Import/Export" %}</div>
{% include image.html file="ch_import_template.png" alt="Import šablony" caption="Šablona" %}
</div>

V __Tabulkové šabloně__ jsou 4 listy. "CourtHive" list je prázdný, ale musí být vložen do tabulky aby systém soubor rozeznal. Ostatní 3 listy jsou volitelné
a mohou být smazány v závislosti na tom jaký typ dat je importován. Pro hráče je důležité aby hráčovo ID bylo unikátní.

### Manuální vložení

Lokální databáze hráčů může být vytvořena nebo existující databáze rozšířena tím, že lze každého hráče zadat jednotlivě.

Ikona __Přidat hráče__ je dostupná z domovské stránky kliknutím na ikonu __Hráči.__

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'> {% include image.html file="ch_players_icon.png" alt="Hráči" caption="Ikona hráči" %}</div>
   {% include image.html file="ch_players_add_icon.png" alt="Přidat hráče" caption="Přidat hráče" %}
</div>

Pouze vyplnění polí označených __žlutě__ je požadováno.

{% include image.html file="ch_players_add_form.png" alt="Informace o hráči" caption="Základní informace o hráči" %}

{% include note.html content='Hráči mohou být také manuálně zadáni při přidávání hráčů do turnaje, pokud hráč není během vyhledávání nalezen.' %}

### Turnajové výsledky

Když jsou turnaje a utkání přidány do lokální databáze, turnajové výsledky se stanou dostupnými v systému.

{% include image.html file="ch_players_ladder.png" alt="Turnajové výsledky" caption="Turnajové výsledky" %}

Žebříková ("Ladder") vizualizace turnajových výsledků zahrnuje povrch (barvu), kategorii, finalní kolo (pozici) and kategorii turnaje.

---
title: TMX Rychlý manuál
keywords: Example Tutorial Quick Start
sidebar: ch_sidebar
permalink: tmx_quick_start.html
toc: true
---
## Overview

Účelem tohoto rychlého manuálu je pomoci s použitím TMX pro co nejrychlejší vytvoření hracích plánů prvního turnaje.

Tento rychlý manuál obsahuje následující:
- zadání konfiguračního klíče umožňujícího načtení hráčů na žebříčku
- vytvoření turnaje
- přidání hráčů do turnaje
- přihlášení přidaných (registrovaných) hráčů pro turnaj
- vytvoření turnajových soutěží
- prezentace (schválení) hráčů pro příslušnou turnajovou soutěž
- vytvoření hracího plánu pro turnajovou soutěž

## Demonstrační video

Toto video zachycuje všechny kroky popsané v TMX Rychlém manuálu.

{% unless site.output == "pdf" %}
   <iframe width="560" height="315" src="https://www.youtube.com/embed/6wkHX5HzVSk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
{% endunless %}

## Zadání konfiguračního klíče

CourtHive/TMX může být konfigurován k importu ATP/WTA/ITF hráčů přímo do turnaje.  

Na domovské stránce přejděte na pole zadání klíče kliknutím na ikonu Klíče.

{% include image.html file="ch_keys.png" alt="Klíče" caption="Klíče" %}

Zadejte klíč "players" do dialogového okna [Konfigurační klíč](tmx_configuration.html) klikněte na __Odeslat__.

{% include image.html file="ch_key_players.png" alt="ATP/WTA" caption="Konfigurační klíč" %}

Nic viditelného se nestane když je klíč odeslán ale systém je tímto nakonfigurován příslušnými parametry pro načtení žebříčku hráčů podle kategorií.

## Vytvoření turnaje

Na domovské stránce přejděte do kalendáře turnajů kliknutím na ikonu Turnaje

{% include image.html file="ch_tournaments.png" alt="Tournaments" caption="Tournaments" %}

__Turnajový kalendář__ zobrazí turnaje v rámci vybraného časového období, případně omezené věkovou kategorií.  

Napravo od filtru věkové kategorie je ikonka __Přidat turnaj__.

{% include image.html file="ch_add_tournament_icon.png" alt="Turnajové filtry" caption="Turnajové filtry" %}

Kliknutí na ikonu __Přidat turnaj__ otevře okno pro zadání informací o novém turnaji.  

Pole označené ___žlutě___ jsou povinné aby turnaj mohl být přidán.

<div style='display: flex; flex-wrap: wrap;'>
   {% include image.html file="ch_add_tournament.png" alt="Přidat turnaj" %}
   {% include image.html file="ch_challenge.png" alt="Přidat turnaj" %}
</div>

{% include important.html content="V tomto příkladu přidáme hráče ___bez data narození___, takže není třeba omezení žádnou věkovou kategorií"%}

{% include image.html file="ch_challenge_calendar.png" alt="Turnaj přidán" %}

## Editace turnaje

Kliknutí na turnaj v kalendáři turnajů nejdříve otevře záložku Turnaj (= přehled o turnaji).  Všimněte si, že v pravém horním rohu je __ikonka tužky__.  

{% include image.html file="ch_challenge_modal.png" alt="Turnaj" caption="Turnaj" %}

Kliknutím na __ikonu tužky__ přejdete do ___editovacího režimu___.

{% include image.html file="ch_editing_mode.png" alt="Editovací režim" caption="Další záložky se objeví v editovacím režimu" %}

## Přidat hráče

V záložce __Hráči__ lze přidat hráče do turnaje kteří jsou pak prezentováni když dorazí do dějiště turnaje.

{% include image.html file="ch_players_tab.png" alt="Hráči" caption="Turnajoví hráči" %}

Vzhledem k tomu, že CourtHive/TMX byl nakonfigurován k načtení _hráčů na žebříčku_ z různých zdrojů, kliknutím na ikonu __Obnovit__ úplně vpravo zobrazí volby dostupné pro import hráčů.

{% include image.html file="ch_player_import.png" alt="Player Import" caption="Vyber hráče k importu" %}

ATP, WTA, and ITF ikonky importují hráče podle žebříčků jejich příslušných organizací.  Ikona "Načíst hráče / Load Players" umožní importovat tabulku s hráči ve formátu __Excel XLSX__.  Lze použít [TMX šablona](tmx_players_managing.html#dragdrop-import) nebo UTR hodnocení které může být generováno [zde... pokud máte účet](https://app.myutr.com/players/ratingslist){:target="_ blank"}.

Pro ilustraci v tomto manuálu, klikněte na __ATP__ volbu.

{% include image.html file="ch_atp_players.png" alt="ATP Players" caption="Žebříček ATP hráčů" %}

## Přihlášení hráčů

Předtím, než mohou být hráči přidání do turnajové soutěže, tak musí být přihlášeni v záložce __Hráči__. To lze provést dvěma způsoby: Použitím vyhledávacího pole v horní části obrazovky, nebo __kliknutím__ na jméno hráče.  

Pro účely tohoto manuálnu, jednoduše klikněte postupně na prvních 8 hráčů pro přihlášení do turnajové soutěže.

{% include note.html content="Přihlášení hráči se objeví __dole__ pod registrovanými, dosud nepřihlášenými hráči." %}

{% include image.html file="ch_atp_players_signed_in.png" alt="Signed In" caption="Přihlášení hráči" %}

## Přidání soutěže

Nyní se můžete přepnout do záložky __Soutěže__ kliknutím na záložku.

Přidejte svoji první soutěž kliknutím na ikonu __Přidat soutěž__.  Uvidíte 8 hráčů v sekci ___Přihlášení___ pro soutěž, pokud vyhovují kritériím nastaveným na  _pohlaví_ and _věkovou kategorii_.

{% include image.html file="ch_quick_start_event.png" alt="Turnajová soutěž" caption="Přidání nové soutěže do turnaje" %}

Hráči mohou být __schváleni__ (přesunuti do sekce __Prezentovaní__) pro soutěž celkem _čtyřmi_ způsoby:
- kliknutím na jméno hráče
- kontextovým kliknutím na jméno hráče k prezentaci hráče jako _volná karta_ (wildcard)
- kliknutím na __+__ ikonu na pravé straně sekce __Přihlášení__ (ke schválení všech hráčů)
- vyhledáním hráče ve vyhledávacím poli (___pouze poté co byla turnajová soutěž uložena___)

Jakmile jste schválili všech 8 hráčů, klikněte na __Uložit soutěž__ a pak na ikonu __Automatický los__.

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'>
        {% include image.html file="ch_events_auto_play.png" alt="Play" %}
   </div>
   <div style='padding-bottom: 1em;'>
        {% include image.html file="ch_events_auto_pause.png" alt="Pause" %}
   </div>
</div>

Jakmile je soutěž uložena, objeví se záložka __Hrací plány__.

Pokud jste stiskli tlačítko __Automatický los__, pak se také objeví záložka __Utkání__.

{% include image.html file="ch_quick_start_auto_event.png" alt="Turnajová soutěž" caption="Soutěž uložena, Automatický los" %}

## Prohlížení hracího plánu

Nyní můžete přejít do záložky __Hrací plány__.

{% include image.html file="ch_quick_start_draw.png" alt="Event Draw" caption="Eliminační hrací plán" %}

Teď jste připravení [Zadat výsledky](tmx_tournament_scoring.html) a vytisknout PDF hrací plány.

Můžete vytvořit libovolné množství soutěží v rámci turnaje: vyřazovací hrací plán, skupiny, kompas hrací plán, rozložené vstupní hrací plány, čtyřhry atd.  

Můžete také propojit kvalifikační hrací plán s hlavní soutěží a se soutěží útěchy a sledovat postupy hráčů do jednotlivých soutěží.  

Rovněž můžete přidat do turnaje WTA nebo ITF hráče a vytvořit ženské nebo smíšené soutěže.

___Have Fun!___

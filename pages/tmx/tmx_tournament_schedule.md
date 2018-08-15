---
title: Rozpis utkání
keywords: tournament schedule
sidebar: ch_sidebar
permalink: tmx_tournament_schedule.html
toc: true
---

{% include important.html content="Záložka __Rozpis utkání__ se neobjeví dokud alespoň jedna [turnajová soutěž](tmx_events_management.html) nebyla vytvořena a jeden turnajový [Areál](tmx_tournament_courts.html) nebyl nadefinován." %}

## Akční ikony

V pravé části záložky od __Výběru hracího dne__ je několik "akčních ikon"

* __Ikona "Naplánovat utkání / (Ikona hráče):__ přepíná plánovací panel rozpisu utkání s nabídkou dosud nenaplánovaných utkání
* __Ikona "OOP komentář" / Časová ikona:__ zobrazí dialogové okno pro zadání poznámek k rozpisu utkání
* __PDF ikona:__ vytvoří PDF soubor s rozpisem utkání

{% include image.html file="ch_schedule_tab.png" alt="Rozpis utkání" caption="Turnajový rozpis utkání" %}


## Plánování utkání v rozpisu

Kliknutí na ikonu __Naplánovat utkání__ ukáže / skryje panel s nenaplánovanými zápasy.

{% include image.html file="ch_schedule_scheduling_panel.png" alt="Plánovací panel" caption="Plánovací panel" %}

### Výběr hracího dne

Během plánování utkání použití tlačítka __Výběr hracího dne__ určí konkrétní den na který budou utkání naplánována.

### Filtrování utkání

Na __plánovacím panelu__ je možné filtrovat utkání podle __soutěže__ a podle __kola__.

### Automatické plánování

Tlačítko __Automatické plánování__ začne proces naplánování, t.j. nasazení utkání v plánovacím panelu na dvorce.

Pokud jsou plánovana na dvorce utkání z více kol ze soutěže pak musí být vybrána plánovací priorita.

{% include image.html file="ch_schedule_priority.png" alt="Plánovací priorita" caption="Plánovací priorita" %}

__Priorita dle pořadí__ znamená, že utkání z jedné soutěže budou naplánována v pořadí shora dolů dle hracího plánu, bez ohledu na _kolo_ ke kterému utkání přísluší.

__Priorita dle kola__ znamená že utkání dřívějších kol budou naplánována _před_ pozdějšími koly.

### Manuální plánování

Utkání lze přidat do rozpisu manuálně dvěma způsoby:
* Přesunutím utkání z plánovacího panelu na vybraný dvorec
* Kliknutím na vybraný dvorec a zadáním jména hráče

#### Plánování přetažením (Chyť a Pusť)
{% unless site.output == "pdf" %}
   <iframe width="560" height="315" src="https://www.youtube.com/embed/wr8Z4Pw9YqA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
{% endunless %}

#### Stažení utkání na dvorec (buňku)
{% include image.html file="ch_schedule_pulling.png" alt="Vyhledání utkání" caption="Vyhledání utkání" %}

### Plánované časy utkání

Plánované časy utkání pro __celý řádek rozpisu utkání__ lze zadat pomocí [kontextového kliknutí](tmx_fundamentals.html) na číslo řádku vlevo.

{% include image.html file="ch_schedule_metadata.png" alt="Vyhledání utkání" caption="Vyhledání utkání" %}

Plánované časy utkání pro __individuální utkání__ lze zadat pomocí [kontextového kliknutí](tmx_fundamentals.html) na vybranou buňku (dvorec na řádku).

### Metadata utkání

[Kontextové kliknutí](tmx_fundamentals.html) na vybrané utkání v rozpisu vyvolá možnosti zadání specifických metadat pro každé utkání.

{% include image.html file="ch_schedule_match_metadata.png" alt="Metadata utkání" caption="Metadata utkání" %}

## Poznámka rozhodčího

Ikona __OOP komentář / Časová ikona__ otevře dialogové okno kam může rozhodčí zadat poznámku která se objeví dole v PDF rozpisu utkání a nahoře v online rozpisu utkání.

{% include image.html file="ch_schedule_order_of_play.png" alt="Poznámky k rozpisu" caption="Poznámky k rozpisu" %}

## Zadávání výsledků

Kliknutí na utkání v rozpisu otevře dialogové okno k zadání výsledku. Pokud je otevřen __plánovací panel__ tak lze vyvolat okno pro zadání výsledku [kontextovým kliknutím](tmx_fundamentals.html).

[Výsledky utkání lze zadávat v rozpisu utkání stejným způsobem jako v jiných záložkách.](tmx_tournament_scoring.html#score-entry)

{% include image.html file="ch_schedule_status.png" alt="Stav v rozpisu" caption="Stav v rozpisu" %}

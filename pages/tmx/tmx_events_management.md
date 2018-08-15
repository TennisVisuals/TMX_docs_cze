---
title: Turnajové soutěže
keywords: tournament event management
sidebar: ch_sidebar
permalink: tmx_events_management.html
toc: true
---

## Přidání a smazání soutěží

{% include image.html file="ch_events_add.png" alt="Přidat soutěž" caption="Přidat novou turnajovou soutěž" %}

Pole výběru pohlaví __Muži / Ženy__ předpokládá při přidání nové soutěže:
* výchozí "Muži" když jsou pouze muži přihlášeni
* výchozí ""Ženy" když jsou pouze ženy přihlášeny
* výchozí ""Ženy" když mužská soutěž dvouhry už existuje nebo naopak

{% include image.html file="ch_events_unsaved.png" alt="Uložit soutěž" caption="Uložit novou turnajovou soutěž" %}

{% include note.html content="Pro každou novou soutěž jsou __Přihlášení__ hráči filtováni podle konfigurace soutěže" %}

{% include important.html content="Soutěže musí být uloženy předtím než Hrací plány mohou být vytvořeny a rozpis utkání naplánován" %}

Soutěže které byly uloženy se objeví v __Seznamu soutěží__ a __Uložit soutěž__ tlačítko je nahrazeno tlačítkem __Smazat soutěž__.

{% include image.html file="ch_events_saved.png" alt="Uložené soutěže" caption="Uložené soutěže" %}

## Schvalování hráčů

Dostupní hráči jsou uvedeni v záložce __Přihlášení__ v pořadí podle žebříčku__ (#).

{% include image.html file="ch_events_approving.png" alt="Schvalování hráčů" caption="Schvalování hráčů" %}

Všichni přihlášení hráči mohou být schváleni kliknutím na __+__ v pravém horním rohu sekce Přihlášení hráči.

Všichni schválení hráči v sekci __Prezentovaní__ mohou být odstraněni kliknutím na __-__ v pravém horním rohu sekce Prezentovaní hráči.

Hráč může být přidán individuálně kliknutím na jeho jméno nebo použitím vyhledávacího pole, které je zde omezeno jen na přihlášené hráče.

{% include image.html file="ch_events_approve_search.png" alt="Hledat ke schválení" caption="Hledat ke schválení" %}

Hráči mohou být schválení jako __Volné karty__ pomocí [Kontextního kliknutí](tms_fundamentals.html) na své jméno.

{% include image.html file="ch_events_wildcard.png" alt="Schválit volnou kartu" caption="Schválit volnou kartu" %}

Poté, co jsou hráči schváleni a přesunuti do sekce __Prezentovaní__, jsou tito hráči seřazeni podle příjmení and žebříček hráče je nahrazen pozicí nasazení,
a pokud přichází v úvahu, i způsobem akceptace (Q, WC, LL).

{% include image.html file="ch_events_approved_seeding.png" alt="Schválit volnou kartu" caption="Schválit volnou kartu" %}

## Seznam soutěží

__Seznam soutěží__ zobrazuje informaci o každé soutěži v kompaktní formě.

Kliknutí na soutěž otevře nebo zavře dialog __Detaily o soutěži__ , kde je možné editovat soutěž.

{% include image.html file="ch_events_list.png" alt="Seznam soutěží" caption="Seznam soutěží" %}

Informace zobrazené o každé soutěži zahrnují: velikost hracího pole, počet schválených hráčů / dvojic, celkový počet utkání, počet naplánovaných utkání v rozpisu,
kategorie soutěže, hala/venku, povrch, jestli byl vytvořen hrací plán, and jestli byla soutěž publikována.

## Formát skóre

Formát skóre je použit pro všechna utkání v soutěži.  Když je formát skóre změněn poté co soutěž již začala a úvodní výsledky jsou zadány, pak se formát skóre změní do budoucna jen pro ta utkání u kterých ještě nebyl výsledek zadán.

{% include image.html file="ch_events_scoring_default.png" alt="Výchozí formát skóre" caption="Výchozí formát skóre" %}

## Automatické losování hracího plánu

V dialogu __Detaily o soutěži__ je pro každou soutěž k dispozici tlačítko pro aktivaci / deaktivaci automatického losování hracího plánu.

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'>{% include image.html file="ch_events_auto_play.png" alt="Spustit" caption="Spustit" %}</div>
   {% include image.html file="ch_events_auto_pause.png" alt="Pauza" caption="Pauza" %}
</div>

{% include note.html content='Automatické losování může být zakázáno pomocí [Organizačního klíče](tmx_configuration.html) pokud není oficiálně schváleno' %}

## Propojené soutěže

Soutěže mohou být spolu propojeny pokud jsou v nastavení stejného pohlaví a __Typy hracího plánu__ se  doplňují.

Pokud mužská __Vyřazovací soutěž__ existuje když je přidána mužská __Kvalifikační soutěž__, nebo naopak, možnost propojit obě soutěže se objeví v levém spodním
rohu dialogu __Detaily o soutěži__.

Pro __Kvalifikační soutěž__ je k dispozici pole výběru počtu hráčů kteří postoupí do hlavní soutěže.

{% include image.html file="ch_events_qualification.png" alt="Kvalifikační soutěž" caption="Přidání kvalifikační soutěže" %}

Kyž je __Kvalifikační soutěž__ propojena s __Vyřazovací soutěží__ tak hráči, kteří jsou už ve __Vyřazovací soutěži__ zmizí ze seznamu přihlášených hráčů.

{% include image.html file="ch_events_linked_qualification.png" alt="Propojené soutěže" caption="Propojená kvalifikační soutěž" %}

Poté co jsou hráči schváleni a počet kvalifikantů byl vybrán (čtyři v tomto příkladu), __Seznam soutěží__ aktualizuje velikost hracího pole, počet
hráčů, a počet utkání pro propojenou __Vyřazovací soutěž__.

{% include image.html file="ch_events_linked_qualifiers.png" alt="Propojení kvalifikanti" caption="Propojení kvalifikanti" %}

Hráči, kteří se automaticky kvalifikují se objeví jako __Prezentovaní__ hráči v propojené __Vyřazovací soutěži__.

{% include image.html file="ch_events_players_qualified.png" alt="Kvalifikanti" caption="Kvalifikovaní hráči" %}

## Lucky Losers (Štastní poražení)

__Lucky Losers__ mohou být přidáni do seznamu __Prezentovaných__ hráčů pomocí [Kontextového kliknutí](tmx_fundamentals.html) na hlavičku __Přihlášení__
a poté jejich výběrem ze seznamu nabídnutých hráčů.

{% include image.html file="ch_events_lucky_losers.png" alt="Lucky Losers" caption="Lucky Losers" %}

## Čtyřhry

Vytváření __Soutěží čtyřhry__ je téměř identické se __Soutěží dvouhry__, kromě toho že pro __Soutěž čtyřhry__ dvojice pro čtyřhru musí být vytvořeny
předtím než mohou být schváleny / prezentovány.

__Dvojice pro čtyřhru__ se vytvoří jednoduše vybráním jednotlivých hráčů v dvojici _v pořadí_.

{% include image.html file="ch_events_doubles_teams.png" alt="Dvojice pro čtyřhru" caption="Dvojice pro čtyřhru" %}

### Kombinovaný žebříček pro čtyřhry

Výchozí konfigurace v CourtHive/TMX k seřazení dvojic je podle _kombinovaného žebříčku_, což znamená, že žebříček dvouhry obou hráčů dvojice je sečten.  
Toto výchozí nastavení může být změněno pomocí [Organizačního klíče](tmx_configuration.html) jelikož některé organizace počítají žebříček pro čtyřhry jinak.

Dvojice které mají stejný kombinovaný žebříček jsou vyznačeny __žlutě__.

[Kontextové kliknutí](tmx_fundamentals.html) na takovou dvojici pro čtyřhru vytvoří možnost zadat "pomocné pořadí".

{% include image.html file="ch_events_doubles_options.png" alt="Možnosti pro pár čtyřhry" caption="Možnosti pro pár čtyřhry" %}

"Pomocné pořadí" umožní, aby byly jednotlivé dvojice pro čtyřhru odlišeny z důvodu __nasazení__.

{% include image.html file="ch_events_doubles_subrank.png" alt="Pomocné pořadí" caption="Pomocné pořadí" %}

### Schvalování dvojic pro čtyřhru

Dvojice pro čtyřhru můžou být schváleny _individuálně_ (včetně volných karet) pomocí [Kontextového kliknutí](tmx_fundamentals.html).

Dvojice můžou být rovněž schváleny _hromadně_ pomocí kliknutí na __+__ v pravém horním rohu sekce pro "Dvojice".

{% include image.html file="ch_events_doubles_approving.png" alt="Schvalování dvojic" caption="Schvalování dvojic" %}

### Odstranění dvojic pro čtyřhru

Kliknutí na individuální hráče v sekci "Přihlášení" vytvoří dvojice pro čtyřhru.

Kliknutí na dvojici ji odstraní ze sekce "Prezentovaní", nebo vrátí individuální hráče do sekce "Přihlášení".

## Skupinové soutěže

Soutěže skupin mohou být jako samostatné nebo propojené s __Vyřazovací soutěží__.
* Počet __skupin__ je vypočítán automaticky podle __velikosti skupiny__
* Počty hráčů ve skupině nastavitelné v poli __velikost skupiny__ jsou konfigurovány pomocí [Organizačního klíče](tmx_configuration.html)
* Pole __Kvalifikanti__ je k dispozici jen pokud je skupinová soutěž propojená s jinou soutěží
* Volba umožňujíci propojit soutěž s jinou soutěží je objeví jen když příslušná soutěž existuje

{% include image.html file="ch_events_round_robin.png" alt="Skupinová soutěž" caption="Nastavení soutěže skupin" %}

### Kvalifikanti

Kvalifikanti z každé skupiny jsou seřazeni podle poměru vítězných utkání, setů, gamů a bodů.

Podrobné vysvětlení k pořadí ve skupinách je k nalezení v dokumentaci [__Poměr výher__](tmx_tournament_draws.html#win-ratios).

{% include image.html file="ch_draws_rr_order.png" alt="Pořadí" caption="Kalkulované pořadí ve skupině" %}

{% include tip.html content="Výchozí nastavení je  __jeden__ kvalifikant z každé skupiny; toto nastavení může být změněno __pouze__ v dialogu __Detaily o soutěži__ pro skupinovou soutěž." %}

{% include important.html content="Druhý (a třetí) kvalifikant z každé skupiny je určen __až poté__ co jsou výsledky všech skupin kompletní." %}

{% include note.html content="Pokud vybraný počet kvalifikantů není násobkem počtu skupin, dodateční hráči z každé skupiny (1., 2., 3., atd. z každé skupiny) jsou
kvalifikování nejdříve podle žebříčku a pak podle __Poměru výher__." %}

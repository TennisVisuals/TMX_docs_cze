---
title: Jak zveřejňování funguje
keywords: Publishing Live Scores
sidebar: ch_sidebar
permalink: tmx_publishing_overview.html
toc: true
---

## Veřejný obsah

Existují tři druhy informací které mohou být zveřejňovány z [CourtHive/TMX](https://courthive.com/tmx) do [CourtHive/Live](https://courthive.com/live):
* Turnajové detaily (název, datumy, obecné informace)
* Turnajové plány / Rozpis utkání ("Order of Play" = OOP)
* Turnajové soutěže (výsledky utkání, hrací plány)

## Požadavky ke zveřejňování

Zveřejnění je možné jen pokud [Organizační klíč](tmx_configuration.html) byl zadán.  Poté co byl platný konfigurační klíč zadán, ikona zveřejnění se objeví v záložce __Turnaj__ v __Editačním módu.__

Turnaj je možné editovat a zveřejňovat jen pokud je CourtHive/TMX klient konfigurován pro stejnou Organizaci ke které turnaj patří.

## Identity prohlížeče

Každý prohlížeč (Chrome, Opera, Firefox, Safari) na každém zařízení obdrží tzv. Universal Unique Identifier (UUID).  Navíc, pokud se do prohlížeče Chrome přihlásíte pomocí různých účtů Google, pak každý účet prohlížeče __ve stejném počítači / zařízení__ má svůj vlastní identifikátor UUID.

{% include important.html content='Autorizační klíč musí být zadán ve stejné identifikaci prohlížeče která bude použita ke zveřejnění turnaje. Zadání autorizačního klíče v prohlížeči Firefox neopravňuje prohlížeč Chrome pro daný turnaj; a zadání autorizačního klíče při přihlášení jako jeden uživatel nebude autorizovat jiné uživatelské účty ve stejném prohlížeči.' %}

CourtHive Cloud Server (CCS) kontroluje UUID klientů při určování zda může být turnaj zveřejněn jako "Oficiální" nebo "Neoficiální".  CCS povolí pouze __jednomu__ klientovi ve stejném čase aby mohl zveřejnit či zrušit zveřejnění turnaje.  

Viz: [Autorizační klíče](tmx_publishing_overview.html#authorization-keys).

{% include tip.html content='Turnaje které byly zveřejněny neoficiálně mohou být zobrazeny na CourtHive/Live vložením "?test" na konec URL organizace.' %}

## Ikony zveřejňování

Když jsou ikony zveřejňování viditelné, jejich barva označuje, zda bylo něco zveřejněno a pokud ano, tak jestli jsou zveřejněné informace aktuální nebo zastaralé.

{% include image.html file="ch_events_list_publishing.png" alt="Stav zveřejnění" caption="Stav zveřejnění" %}

Kliknutí na __Ikonu zveřejnění__ spustí proces zveřejňování. Ikona nezmění barvu dokud CourtHive Cloud Server nezjistí, že zveřejňovaná položka byla přijata.  
<br>

| Barva | Vysvětlení  |
|-------|--------|
| <img src="./images/ch_publishing_unpublished.png" alt="Zveřejněno"> | Nezveřejněno  |
| <img src="./images/ch_publishing_published.png" alt="Zveřejněno"> | Zveřejněno, aktuální  |
| <img src="./images/ch_publishing_outofdate.png" alt="Zveřejněno"> | Zveřejněno, zastaralé  |

V __Seznamu soutěží__ kliknutí na ikonu __Zveřejnit__ funguje jako přepínání mezi zveřejněním a zrušením zveřejnění.

Ve záložce Turnaj, Hrací plán a Rozpis utkání funguje kliknutí na ikonu __Zveřejnit__ a [Kontextové kliknutí](tmx_fundamentals.html) a pak potvrzení na __"Zrušit zveřejnění"__.

### Zrušení zveřejnění VŠECH turnajových soutěží
[Kontextové kliknutí](tmx_fundamentals.html) na ikonu __Zveřejnit__ v hlavičce __seznamu soutěží__ v záložce __Soutěže__ zruší zveřejnění všech turnajových soutěží.

### Zrušení zveřejnění turnaje
[Kontextové kliknutí](tmx_fundamentals.html) na ikonu __Zveřejnit__ v záložce __Turnaj__ odstraní
kompletně celý turnaj z [CourtHive/Live](https://courthive.com/live).

## Autorizační klíče
Pokud jste součástí organizace, která schválila používání CourtHive, pak může být turnaj oficiálně zveřejněn zadáním autorizačního klíče.  

Autorizační klíče jsou __jednorázové__, což znamená, že jakmile byly zadány, nemohou být znovu použity. Pouze jeden prohlížeč na jednom počítači smí být autorizován k oficiálnímu zveřejňování turnajových informací.

{% include image.html file="ch_home_green.png" alt="Autorizován" caption="Autorizován" %}

Pokud není předem příslušný turnaj ve Vašem kalendáři, zadání Autorizačního klíče ho přidá do lokální databáze.  

["Kontextové kliknutí"](tmx_fundamentals.html) na ikonu Domů zobrazí autorizační zprávu.  

{% include tip.html content="Kliknutím na autorizační zprávu přejdete přímo do turnaje." %}

## Příklady scénářů

Každý prohlížeč má jedinečnou identitu a zadáním jednorázového Autorizačního klíče poskytuje serveru jedinečný identifikátor prohlížeče, takže pouze tento konkrétní prohlížeč muže zveřejňovat "oficiálně".

Prohlížeč, ve kterém je zadán Autorizační klíč, již musí být nakonfigurován pro stejnou organizaci která vytvořila turnaj.

Jediný rozdíl mezi Organizačním klíčem __Admin__ a klíčem __Rozhodčí__ je, že ten s __Admin__ klíčem může generovat klíče pro autorizaci turnajů.

Pokud chce administrátor vytvořit Autorizační klíč tak musí mít turnaj ve svém kalendáři a ve svém autorizovaném prohlížeči.  Pokud nemá rozhodčí turnaj ve svém kalendáři, tak bude tento turnaj přidán automaticky (ze serveru) až rozhodčí zadá Autorizační klíč.

Každý rozhodčí, který má Organizační klíč může vytvořit a zveřejnit svoje vlastní turnaje "Neoficiálně".  (Různé verze téhož turnaje mohou být zveřejněny  "neoficiálně" a "oficiálně").

Každý rozhodčí s Organizačním klíčem může také "Stáhnout / PULL" (cloud fetch) oficiální verzi turnaje ze serveru, ale pouze pokud celý turnaj byl "Odeslán /PUSHED" na server (šipka Nahoru v záložce Turnaj).

Pokud rozhodčí vytvoří svůj vlastní turnaj který není na seznamu turnajů u administrátora, jakým způsobem může potom administrátor vygenerovat autorizační klíč pro daný turnaj?  
Jediný způsob je, že rozhodčí exportuje turnaj lokálně na disk a pošle turnajový soubor administrátorovi (přes email/zprávu). Poté administrátor importuje soubor s turnajem do svého  lokálního kalendáře turnajů a vygeneruje pro rozhodčího Autorizační klíč nutný ke zveřejňování.

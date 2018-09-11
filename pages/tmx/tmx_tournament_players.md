---
title: Hráči
keywords: tournament players
sidebar: ch_sidebar
permalink: tmx_tournament_players.html
toc: true
---

## Úvod

V záložce __Hráči__ se spravují hráči přihlášení na turnaj.  Registrovaní hráči mohou být synchronizováni se vzdálenými servery; další hráči mohou být přidáni z lokální databáze nebo odstraněni z turnaje; hráči mohou být rovněž přihlášeni a odhlášeni z turnaje.

{% include image.html file="ch_tournament_players.png" alt="Turnajoví hráči" caption="Turnajoví hráči" %}

Od verze 1.0 CourtHive/TMX je pouze jedna věková kategorie hráčů dostupná pro turnaj, takže výběr věkové kategorie je zafixován podle kategorie vybrané během vytvoření turnaje.

## Synchronizace registrovaných hráčů

[Organizační klíč](tmx_configuration.html) může konfigurovat CourtHive/TMX aby načítal hráče registrované na turnaj ze vzdálených serverů.

Pokud byl Organizační klíč zadán, kliknutí na __Obnovit ikonu__ vpravo nahoře zkontroluje vzdálený server pro nově registrované hráče.

[Kontextové kliknutí](tmx_fundamentals.html) na __Obnovit ikonu__ nahradí jakýkoli existující seznam aktuálním seznamem  registrovaných hráčů ze serveru.

## Přidání hráčú z lokální databáze

{% include image.html file="ch_search_add_player.png" alt="Přidat hráče" caption="Přidat hráče" %}

Pokud jsou hráči v lokální databázi, mohou být do turnaje přidáni pomocí [Vyhledávacího pole](tmx_searchbox.html).

Pouze hráči oprávnění startovat v dané věkové kategorii budou nalezeni při vyhledávání v tomto kontextu.

{% include image.html file="ch_search_roger.png" alt="Přidat hráče" caption="Vyhledání oprávněných hráčů" %}

## Změna žebříčku

Po přidání hráčů do turnaje se objeví __Ikona Žebříček__ vlevo od __Ikony Obnovit__.  Pokud je třeba upravit žebříček hráče, klikněte na __Ikonu Žebříček__ k přepnutí do editovacího režimu žebříčku.

{% include image.html file="ch_rankings_icon.png" alt="Změnit žebříček" %}

{% include image.html file="ch_rankings_edit.png" alt="Změnit žebříček" caption="Změnit žebříček" %}

### Pomocný žebříček

Žebříček hráče může být změněn buďto před nebo poté co byl hráč přihlášen.

Poté co byl hráč přihlášen, TMX prověří jestli jsou nějací hráči se stejným žebříčkem.  Pokud ano pak se objeví dodatečné vstupní pole vedle žebříčku těchto hráčů, kam lze zadat "pomocný žebříček" k odlišení hráčů při nasazování do hracího plánu.  

{% include image.html file="ch_rankings_subrank.png" alt="Pomocný žebříček" %}

## Filtrování hráčů

V pravém horním rohu záložky __Hráči__ se nachází filtry pohlaví, které umožní aby byl seznam hráčů filtrován na pouze muži / chlapci nebo ženy / dívky.  Tyto filtry se používají při prezentaci hráčů jelikož na mnoha turnajích se muži a ženy prezentují v různých časech.

{% include image.html file="ch_players_filtering.png" alt="Filtrování" caption="Filtr pohlaví" %}

__Filtr pohlaví__ také změní chování __PDF ikony__ tak, že seznam přihlášených hráčů může být generován podle pohlaví v souladu s pracovním postupem ředitelství turnaje.

## Tisk přihlašovacích seznamů

Pokud jsou hráči registrováni na turnaj, zobrazí se __PDF ikona__ vpravo vedle výběru věkové kategorie.

{% include image.html file="ch_players_sign_in.png" alt="Přihlášení" caption="Tisk přihlašovacích seznamů" %}

Kliknutím na __PDF ikonu__ můžete zvolit možnost tisku přihlašovacích seznamů buďto pro dvouhru nebo pro čtyřhru.  Pokud byli všichni hráči přihlášeni, tak výchozí chování je tisk přihlašovacího seznamu pro čtyřhru.

{% include tip.html content="__Filtry pohlaví__ k tisku správných přihlašovacích seznamů." %}

{% include note.html content="PDF přihlašovací seznamy jsou buďto uloženy nebo otevřeny v nové záložce prohlížeče, v závislosti na [Nastavení](tmx_setup.html#check-your-default-settings)." %}

## Přihlášení a odhlášení

Nejjednodušší způsob, jak přihlásit nebo odhlásit hráče, je kliknout na jeho jméno.

{% include tip.html content="Kromě přidávání nových hráčů, [Vyhledávací pole](tmx_searchbox.html) může být rovněž použito k přihlášení nebo k odhlášení hráčů kteří už jsou registrováni.  To je zejména užitečné když je v turnaji hodně hráčů a pak je obtížné najít hráče podle jména jen procházením seznamu hráčů." %}

{% include note.html content="Hráči, kterí jsou schváleni v turnajové soutěži nemohou být odhlášeni z turnaje." %}

## Úprava a mazání hráčů

[Podpora pro modifikání hráčských dat je minimální](tmx_players_managing.html).

[Kontextovým kliknutím](tmx_fundamentals.html) na hráče je možno upravovat jméno hráče a zemi kterou reprezentují.

Hráči kteří nebyli schváleni pro žádnou soutěž mohou být také odstraněni.

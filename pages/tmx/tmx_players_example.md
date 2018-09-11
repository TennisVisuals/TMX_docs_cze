---
title: Příklad databáze hráčů
keywords: Example Tournament Players Database
sidebar: ch_sidebar
permalink: tmx_players_example.html
toc: false
---

## ATP/WTA databáze hráčů

Aplikaci CourtHive/TMX může být povoleno připojení k ukázkové databázi hráčů zadáním "atpwta" v dialogu pro [Konfigurační klíč](tmx_configuration.html)
a stiskem klávesy __Odeslat__.

{% include image.html file="ch_key_atpwta.png" alt="ATP/WTA" caption="Konfigurační klíč" %}

Nic viditelného se nestane když je tento klíč odeslán, systém bude pouze nakonfigurován s příslušnými parametry pro připojení ke vzdálené databázi.

Chcete-li načíst ukázkovou databázi hráčů, umístěte kurzor myši vlevo vedle ikony __Hráči__ v pravém horním rohu a klikněte na __OK__ tlačítko v dialogu __Obnovit seznam__.

{% include image.html file="ch_players_refresh.png" alt="Hráči" caption="Obnovit databázi" %}

Po načtení lokální datatáze hráčů ze vzdáleného serveru se __Počet hráčů__ změní tak, aby odrážel skutečný počet načtených hráčů.

{% include image.html file="ch_players_loaded.png" alt="Hráči" caption="Načtení hráči" %}

Poté bude možné používat [Vyhledávací pole](tmx_searchbox.html) k vyhledání vybraných hráčů.

{% include image.html file="ch_players_nadal.png" alt="Vyhledat" caption="Vyhledat hráče" %}

Ve výchozím nastavení nejsou žádné jiné údaje o hráčích než rok narození a země kterou reprezentují. Poté, co je hráč zařazen do turnajové soutěže a výsledek jeho
utkání zadán, budou zobrazena zápasová data příslušného hráče.  Žebříčková data budou dostupná po vygenerování žebříčků podle turnajových výsledků.

{% include image.html file="ch_players_nadal_data.png" alt="Vyhledat" caption="Data hráče" %}

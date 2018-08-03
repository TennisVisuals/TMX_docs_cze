---
title: Example Player Dataset
keywords: Example Tournament Players Database
sidebar: ch_sidebar
permalink: tmx_players_example.html
toc: false
---

## ATP/WTA Player Database

CourtHive can be enabled to connect to an example player database by entering "atpwta" in the [Configuration Key](tmx_configuration.html) dialogue and pressing the __Submit__ button.

{% include image.html file="ch_key_atpwta.png" alt="ATP/WTA" caption="Configuration Key" %}

Nothing visible will happen when this key is entered, the system will only be configured with the apprpriate parameters for connecting to a remote database.

To load the exmaple database, hover the mouse over the __Player Count__ icon in the upper right corner and click on the __Refresh__ icon that appears to the left.

{% include image.html file="ch_players_refresh.png" alt="Players" caption="Refresh Database" %}

Once the local database has been populated from the remote server, the __Player Count__ will change to reflect the number of players loaded.

{% include image.html file="ch_players_loaded.png" alt="Players" caption="Players Loaded" %}

It will now be possible to use the [Search Box](tmx_searchbox.html) to search for players.

{% include image.html file="ch_players_nadal.png" alt="Search" caption="Player Search" %}

By default there is no player data other than birth year and country represented.  After a player has been included in Tournament Events and Match Results have been entered, Match Data will be presented.  Ranking Data will be available after rank lists have been generated from Tournament Results.

{% include image.html file="ch_players_nadal_data.png" alt="Search" caption="Player Data" %}

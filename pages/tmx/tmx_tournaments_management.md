---
title: Managing Tournaments
keywords: Tournament Calendar Management
sidebar: ch_sidebar
permalink: tmx_tournaments_management.html
toc: true
---

## Synchronizing Tournaments

When the [Search Box](tmx_searchbox.html) is in Tournaments Mode, the number of tournaments in the calendar is displayed on the far right of the navigation bar. (See [Using the Search Box](tmx_fundamentals.html) to learn how to change the Search Box Mode).

Hovering over the Tournament Count displays a __Refresh Icon__.  If CourtHive/TMX is configured to synchronize with an organization database, tournaments may be loaded from a remote server.

{% include image.html file="ch_tournaments_count.png" alt="Tournament Search" caption="Tournament Search Mode" %}

Clicking the refresh icon requests new tournaments which occur *after* the last entry in the local calendar.

["Context Clicking"](tmx_fundamentals.html) the refresh icon reloads the entire calendar from the server and adds any tournaments which may be missing from the local calendar.

## Manually Adding Tournaments

To the right of the Tournament Category Filter is an Add Tournament Icon.

{% include image.html file="ch_add_tournament_icon.png" alt="Add Tournament" caption="Add Tournament" %}

Clicking the Add Tournament Icon launches an Add Tournament dialogue.  

Fields in __Yellow__ are required before a new tournament can be added.

<div style='display: flex; flex-wrap: wrap;'>
   {% include image.html file="ch_add_tournament.png" alt="Add Tournament" %}
   {% include image.html file="ch_challenge.png" alt="Add Tournament" %}
</div>

{% include image.html file="ch_challenge_calendar.png" alt="Tournament Added" %}

{% include note.html content='In some configurations, ["Context Clicking"](tmx_fundamentals.html) the Add Tournament Icon allows the entry of a tournament ID which can pull tournament information directly from a remote server.' %}

## Deleting and Editing Tournaments

["Context Click"](tmx_fundamentals.html) on any tournament for the option to either edit or delete the tournament.

{% include image.html file="ch_tournament_delete.png" alt="Delete Tournament" caption="Edit or Delete a Tournament" %}

Choosing to edit a tournament launches the same dialogue used to Add a New Tournament, with all of the values filled in.

{% include note.html content='In some configurations there is the option to "Merge" tournaments, which has the effect of combining lists of registered players.' %}

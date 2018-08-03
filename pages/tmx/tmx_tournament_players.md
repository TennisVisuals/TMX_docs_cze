---
title: Tournament Players Tab
keywords: tournament players
sidebar: ch_sidebar
permalink: tmx_tournament_players.html
toc: true
---

## Introduction

The Players Tab is where tournament players are managed.  Registered players may be synchronized with remote servers; additional players may be added from the local dataabase or removed from the tournament; players may also be signed in or out of the tournament.

{% include image.html file="ch_tournament_players.png" alt="Tournament Players" caption="Tournament Players" %}

## Synchronizing Registered Players

[Organization Keys](tmx_configuration.html) can configure CourtHive/TMX to retrieve players registered for tournaments from remote servers.

If an Organization Key has been entered, clicking on the __Refresh Icon__ on the far right checks the remote server for newly registered players.

[Context Clicking](tmx_fundamentals.html) on the __Refresh Icon__ replaces any existing list with an up-to-date list of registered players from the server.

## Adding Players from the Local Database

{% include image.html file="ch_search_add_player.png" alt="Add Player" caption="Add Player" %}

If there are players in the local player database they may be added to the tournament using the [Search Box](tmx_searchbox.html).

Only players who are eligible for the Tournament Category will be found when searching in this context.

{% include image.html file="ch_search_roger.png" alt="Add Player" caption="Eligible Player Search" %}

## Modifying Rankings 

Once players have been added to a tournament, a __Rankings Icon__ appears to the left of the __Refresh Icon__.  If player rankings need to be modified, click the __Rankings Icon__ to enter rankings edit mode. 

{% include image.html file="ch_rankings_icon.png" alt="Modify Rankings" %}

{% include image.html file="ch_rankings_edit.png" alt="Edit Rankings" caption="Edit Rankings" %}

### Subrankings

Player rankings can be modified either before or after players have been signed in.

Once players have been signed in, TMX checks to see whether there are players with equivalent rankings.  If any players have equivalent rankings, an additional entry box appears next to those players' rankings where a "subranking" may be entered to differentiate such players for seeding purposes.  

{% include image.html file="ch_rankings_subrank.png" alt="Subrank" %}

## Filtering Players

In the upper right of the __Players Tab__ there are gender filters which enable the player list to be filtered.  These filters are used when signing in players, since for many tournaments Male and Female players sign in at different times.

{% include image.html file="ch_players_filtering.png" alt="Filtering" caption="Gender Filters" %}

__Gender Filters__ also change the behavior of the __PDF Icon__ so that Sign-In sheets may be generated which are appropriate to the tournament organizer's workflow.

## Printing Sign-In Sheets

If there are players registered for a tournament, a __PDF Icon__ appears to the right of the __Category Selector__.

{% include image.html file="ch_players_sign_in.png" alt="Sign-In" caption="Print Sign-In Sheet" %}

Clicking the __PDF Icon__ presents a choice of printing either a Singles or a Doubles Sign-In Sheet.  If all players have been signed in, then the default behavior is to print a doubles Sign-In Sheet.

{% include tip.html content="__Gender Filters__ should be used so that appropriate Sign-In sheets can be printed." %}

{% include note.html content="PDF Sign-In sheets are either saved or opened in a new Browser Tab, depending on the [Setting](tmx_setup.html#check-your-default-settings)." %}

## Sign-In and Sign-Out 

The simplest way to sign-in or sign-out players is to click on the player's name.

{% include tip.html content="In addition to adding new players, the [Search Box](tmx_searchbox.html) may also be used to sign in or out players who are already registered.  This is particularly useful when there are numerous players and it is difficult to find a player's name by scanning the list." %}

{% include note.html content="Players who are approved for tournament events may not be signed out from a tournament." %}

## Editing and Deleting Players

[Support for modifying player data is minimal](tmx_players_managing.html).

By [Context Clicking](tmx_fundamentals.html) on a player it is possible to edit a player's name or the country which they represent.

Players who have not been approved for any tournament events may also be deleted.

---
title: Tournament Draws
keywords: tournament draws
sidebar: ch_sidebar
permalink: tmx_tournament_draws.html
toc: true
---

## Action Icons

To the right of the __Event Selector__ are several "Action Icons"

{% include image.html file="ch_draws_tab.png" alt="Draws" caption="Tournament Draws Tab" %}

* __Recycle Icon:__ regenerate the currently selected draw
* __Player Icon:__ identify player representatives who witness draw creation
* __PDF Icon:__ generate a PDF of the Player Draw Order, Completed Draw, or Lucky Loser Sign up sheet

### Reganerating Draws

If for any reason a draw needs to be started from scratch, the __Recycyle Icon__ will reset the draw to it's initial state.

{% include note.html content='The __Recycle Icon__ is not available if any match results has been entered.' %}

### Player Representatives

The __PLayer Icon__ launches a dialogue for identifying players who witness draw creation.

{% include image.html file="ch_draws_player_representatives.png" alt="Representatives" caption="Player Representatives" %}

Player representatives will appear at the bottom of PDF printouts of each draw.

### Player Draw Order

If a draw has not been completed (all players placed), then the __PDF Icon__ generates a PDF of the __player draw order__, which is a table of players orderd by their ranking.

This list is used for [Manual Draw Creation](tmx_tournament_draws.html#manual-draw-creation) and will not be generated if draw generation is [Automated](tmx_events_management.html#automated-draws).

{% include image.html file="ch_draws_draw_order.png" alt="Draw Order" caption="Draw Order" %}

## Elimination Draws

If draw generation is [Automated](tmx_events_management.html#automated-draws) then all players are placed automatically and draws are ready for [Scoring](tmx_tournament_scoring.html).

{% include image.html file="ch_draws_main.png" alt="Main Draw" caption="Automated Draw" %}

### Swapping Positions, Alternates, Lucky Losers

Once a draw is complete, [Context Clicking](tmx_fundamentals.html) on a player presents available options.

{% include image.html file="ch_draws_player_options.png" alt="Options" caption="Player Options" %}

If a __seeded player__ is swapped with an __unseeded player__, or replaced by an __alternate__ or __lucky loser__ then seeding information is removed.

{% include image.html file="ch_draws_player_replacement.png" alt="Replacement" caption="Player Replacement" %}

### Manual Draw Creation

When draws are created manually, the 1st and 2nd seed are always placed automatically.

Other seeded players are placed in "Seed Groups".  The 3rd and 4th players are together in a seed group.  The next group, if applicable, would be seeds 5, 6, 7 and 8.

Players may be placed in three ways:
* Enterng a player's __Draw Order__
* Searching for a player by name
* Selecting from a list of available players

{% include image.html file="ch_draws_player_selection.png" alt="Player Selection" caption="Player Selection" %}

The first two options are available when __Clicking__ on a valid draw position:

[Context Clicking](tmx_fundamentals.html) on a valid draw position allows placement by selecting from a list of available players:

{% include image.html file="ch_draws_player_selection_context.png" alt="Seed Selection" caption="Manual Seed Selection" %}

### Removing Players

{% include image.html file="ch_draws_manual_remove.png" alt="Remove Player" caption="Remove Player" %}

Player are removed by [Context Clicking](tmx_fundamentals.html) on their name.

{% include important.html content='Once a draw is complete players can only swapped or replaced by alternates or lucky losers.' %}

## Round Robin Brackets

If draw generation is [Automated](tmx_events_management.html#automated-draws) then all players are placed automatically and draws are ready for [Scoring](tmx_tournament_scoring.html).

{% include image.html file="ch_draws_rr_automated.png" alt="Automatic Draw" caption="Automatic Draw Generation" %}

### Manual Player Placement

When Round Robins are created manually, players are placed in the same way that they are [placed in other draws](tmx_tournament_draws.html#manual-draw-creation), by clicking or [Context Clicking](tmx_fundamentals.html) on valid draw positions.

By default, two players are seeded for each bracket.  This is a setting which can be altered by [Configuration Keys](tmx_configuration.html).

{% include tip.html content='In Round Robin brackets, valid draw positions are highlighted when the mouse is hovering over a bracket.' %}

{% include image.html file="ch_draws_rr_player_placement.png" alt="Place Player" caption="Valid Draw Position" %}

[Context Clicking](tmx_fundamentals.html) is also used to remove players and replace them with alternates, when available.

{% include image.html file="ch_draws_rr_player_options.png" alt="Player Options" caption="Player Options" %}

### Win Ratios

When [scoring](tmx_tournament_scoring.html) is complete, the __Order (#)__ column is highlighted if players have equivalent __Win Ratios__. 

{% include image.html file="ch_draws_rr_sub_order.png" alt="Sub Order" caption="Round Robin Sub Order" %}

[Context Click](tmx_fundamentals.html) on cells in the __+/-__ column to view a player's __Win Ratios__.

{% include image.html file="ch_draws_rr_ratios.png" alt="Win Ratios" caption="Win Ratios" %}

[Context Click](tmx_fundamentals.html) on a highlighted cell to assign a "Sub Order", which is used to determine the order in which players will be qualified from the bracket.

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'>{% include image.html file="ch_draws_rr_sub_order_selection.png" alt="Sub Order" caption="Sub Order Selection" %}</div>
   {% include image.html file="ch_draws_rr_sub_order_defined.png" alt="Sub Order Defined" caption="Sub Order Defined" %}
</div>

---
title: Tournament Events
keywords: tournament event management
sidebar: ch_sidebar
permalink: tmx_events_management.html
toc: true
---

## Adding and Deleting Events

{% include image.html file="ch_events_add.png" alt="Add New Event" caption="Add New Tournament Event" %}

The __Gender Selector__ makes assumptions when new events are being added:
* default to Male if only male players have been signed-in
* default to Female if only female players have been signed-in
* default to Female if a Male Singles event already exists, or vice-versa

{% include image.html file="ch_events_unsaved.png" alt="Save New Event" caption="Save New Tournament Event" %}

{% include note.html content="For each new event __eligible__ players are filtered according to the event configuration" %}

{% include important.html content="Events must be saved before Draws can be created and Matches scheduled" %}

Events which have been saved appear in the __Event List__ and the __Save__ button is replaced by a __Delete Button__.

{% include image.html file="ch_events_saved.png" alt="Saved Events" caption="Saved Events" %}

## Approving Players

Elibible players are shown with __Rank Order__ (#).

{% include image.html file="ch_events_approving.png" alt="Approving Players" caption="Approving Players" %}

All eligible players can be approved by clicking __+__ in the upper right corner of the eligible players section.

All approved players can be removed by clicking __-__ in the upper right corner of the approved players section.

Player can be added individually by clicking their names or by using the search box, which in this context is restricted to players eligible for the current event.

{% include image.html file="ch_events_approve_search.png" alt="Search Approve" caption="Search Approve" %}

Players can be approved as a __Wildcard__ by [Context Clicking](tms_fundamentals.html) on their name.

{% include image.html file="ch_events_wildcard.png" alt="Approve Wildcard" caption="Approve Wildcard" %}

Once approved, players are sorted by last name and player rank order is replaced by seeding position, if applicable, or method of entry (Q, WC, LL).

{% include image.html file="ch_events_approved_seeding.png" alt="Approve Wildcard" caption="Approve Wildcard" %}

## Event List

The __Event List__ dipslays information about each event in a compact form.

Clicking on an event opens or closes the __Event Details__ dialogue, where it is possible to edit an event.

{% include image.html file="ch_events_list.png" alt="Events List" caption="Events List" %}

Information displayed about each event includes Draw Size, Number of Approved Players, Total Number of Matches, Number of Scheduled Matches, Event Rank, Indoor/Outdoor, Surface, whether a Draw has been created, and whether an event has been published.

## Scoring Format

The scoring format is used for all matches within an event.  If the scoring format is changed after an event has begun, then the score format is changed for all matches which have not yet been scored.

{% include image.html file="ch_events_scoring_default.png" alt="Default Scoring" caption="Default Scoring" %}

## Automated Draws

In the __Event Detail__ dialogue for each event is a button for enabling/disabling automatic draw generation.

<div style='display: flex; flex-wrap: wrap;'>
   <div style='padding-right: 1em;'>{% include image.html file="ch_events_auto_play.png" alt="Play" caption="Play" %}</div>
   {% include image.html file="ch_events_auto_pause.png" alt="Pause" caption="Pause" %}
</div>

{% include note.html content='Automated Draws can be disabled by [Organization Keys](tmx_configuration.html) when they are not officially endorsed' %}

## Linking Events

Events may be linked together if they have the same Gender Setting and are complementary __Draw Types__.

If a Male __Elimination Event__ exits when adding a Male __Qualification Event__, or vice-versa, the option to link events appears in the bottom left corner of the __Event Detail__ dialogue.

For a __Qualification Event__ there is also a selector to define the number of players who will advance to a main draw event.

{% include image.html file="ch_events_qualification.png" alt="Qualification Event" caption="Adding a Qualification Event" %}

When a __Qualification Event__ is linked to an __Elimination Event__ then the players already in the __Elimination Event__ disappear from the eligible players list.

{% include image.html file="ch_events_linked_qualification.png" alt="Linked Event" caption="Linked Qualification Event" %}

After players are approved and the number of qualifiers has been selected (__four__ in this example), the __Event List__ updates the Draw Size, Number of players, and Number of Matches for the linked __Elimination Event__.

{% include image.html file="ch_events_linked_qualifiers.png" alt="Linked Qualifiers" caption="Linked Qualifiers" %}

Players who qualify automatically appear as __Approved__ players in the linked __Elimination Event__.

{% include image.html file="ch_events_players_qualified.png" alt="Qualifiers" caption="Qualified Players" %}

## Lucky Losers

__Lucky Losers__ may be added to the __Approved__ players list by [Context Clicking](tmx_fundamentals.html) on the __Eligible__ heading and selecting them from the list of players that is presented.

{% include image.html file="ch_events_lucky_losers.png" alt="Lucky Losers" caption="Lucky Losers" %}

## Doubles Teams

The creation of __Doubles Events__ is almost identical to __Singles Events__, except that for __Doubles Events__ doubles teams must be constructed before they can be approved.

__Doubles Teams__ are constructed simply by selecting team members _in order_.

{% include image.html file="ch_events_doubles_teams.png" alt="Doubles Teams" caption="Doubles Teams" %}

### Combined Rankings

The default configuration is for CourtHive/TMX to order teams by _combined rankings_, which means that singles rankings of team members are combined.  This option can be modified by [Organization Keys](tmx_configuration.html) as some organizations calculate doubles rankings independently.

Teams which have identical combined rankings are highlighted in __yellow__.

[Context Clicking](tmx_fundamentals.html) on a doubles teams presents options which include assigning a "Subrank".

{% include image.html file="ch_events_doubles_options.png" alt="Doubles Options" caption="Doubles Options" %}

"Subranking" enables teams to be differentiated for the purposes of __seeding__.

{% include image.html file="ch_events_doubles_subrank.png" alt="Doubles Subrank" caption="Doubles Subrank" %}

### Approving Teams

Doubles Teams can be approved _individually_ (including as a Wildcard) by [Context Clicking](tmx_fundamentals.html).

Teams can also be approved _in bulk_ by clicking on the __+__ in the upper right corner of the "Teams" section.

{% include image.html file="ch_events_doubles_approving.png" alt="Approving Teams" caption="Approving Teams" %}

### Removing Teams

Clicking on individual players in the "Eligible" section builds teams.

Clicking on Teams removes them from the "Approved" section, or returns individual players to the "Eligible" section.

## Round Robin Events

Round Robins can either be stand-alone or linked to __Elimination Events__. 
* The number of __brackets__ is calculated automatically from the __Bracket Size__
* The sizes available in the __Bracket Size__ selector are configured by [Organization Keys](tmx_configuration.html)
* The __Qualifiers__ selector only when a Round Robin is linked to another event
* The option to link to another event only appears when appropriate events exist

{% include image.html file="ch_events_round_robin.png" alt="Round Robin" caption="Round Robin Settings" %}

### Qualifiers

Qualifiers in each bracket are ordered by the ratio of matches, sets, games and points won.

Please see the documentation on [__Win Ratios__](tmx_tournament_draws.html#win-ratios) for an in-depth explanation.

{% include image.html file="ch_draws_rr_order.png" alt="Rank Order" caption="Calculated Rank Order" %}

{% include tip.html content="Round Robin Events default to __one__ qualifier per bracket; this setting can __only__ be changed in the Round Robin __Event Detail__ dialogue." %}

{% include important.html content="Second (and third) qualifiers from each bracket are calculated __after__ all brackets are complete." %}

{% include note.html content="If the selected number of qualifiers is not a multiple of the number of brackets, additional qualifiers from each ordered group (1st, 2nd, 3rd, etc. from each bracket) are qualified first by ranking and then by win ratio." %}



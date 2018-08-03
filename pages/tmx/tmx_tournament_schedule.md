---
title: Tournament Schedule
keywords: tournament schedule
sidebar: ch_sidebar
permalink: tmx_tournament_schedule.html
toc: true
---

{% include important.html content="The __Scheduling Tab__ will not appear until at least one [Tournament Event](tmx_events_management.html) has been created and one [Court Location](tmx_tournament_courts.html) has been defined." %}

## Action Icons

To the right of the __Day Selector__ are several "Action Icons"

* __Match Icon:__ toggle match scheduling panel
* __Timing Icon:__ toggle timing notes panel
* __PDF Icon:__ generate a PDF of the schedule

{% include image.html file="ch_schedule_tab.png" alt="Schedule" caption="Tournament Scheduling" %}


## Scheduling Matches

Clicking on the __Match Icon__ shows/hides the match scheduling panel.

{% include image.html file="ch_schedule_scheduling_panel.png" alt="Scheduling Panel" caption="Scheduling Panel" %}

### Day Selection

When scheduling matches, the __Day Selector__ determines the day on which matches will be scheduled.

### Filtering Matches

On the __scheduling panel__ it is possible to filter matches by __Event__ and __Round__.

### Auto Scheduling

The __Auto Schedule__ button begins the process of scheduling matches shown in the match list of the __scheduling panel__.

If multiple rounds of an event are being scheduled then scheduling priority must be chosen.

{% include image.html file="ch_schedule_priority.png" alt="Scheduling Priority" caption="Scheduling Priority" %}

__Order Prioity__ means that matches within one event will be scheduled in order from the top to the bottom, regardless of the _round_ in which they occur.

__Round Prioity__ means that earlier rounds will be scheduled _before_ later rounds.

### Manual Scheduling

Matches may be added to the schedule manually in two ways:
* Draging and Dropping matches from the match list into the desired schedule cells
* "Pulling" matches into schedule cells by clicking on a desired cell and beginning to type a player's name

#### Drag and Drop Scheduling
{% unless site.output == "pdf" %}
   <iframe width="560" height="315" src="https://www.youtube.com/embed/wr8Z4Pw9YqA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
{% endunless %}

#### Pulling Matches into Cells
{% include image.html file="ch_schedule_pulling.png" alt="Match Search" caption="Match Search" %}

### Match Times

Match Times for a __Schedule Row__ are added by [Context Clicking](tmx_fundamentals.html) on the Row Number Cell on the left.

{% include image.html file="ch_schedule_metadata.png" alt="Match Search" caption="Match Search" %}

Match Times for __individual matches__ are added by [Context Clicking](tmx_fundamentals.html) on specific cells.

### Match Metadata

[Context Click](tmx_fundamentals.html) on schedule cells to define specific metadata for each match.

{% include image.html file="ch_schedule_match_metadata.png" alt="Match Metadata" caption="Match Metadata" %}

## Referee Notes

The __Timing Icon__ opens a dialogue where a referee may enter notes which will appear at the bottom of PDFs and at the top of online schedules.

{% include image.html file="ch_schedule_order_of_play.png" alt="Scheduling Notes" caption="Scheduling Notes" %}

## Scoring Matches

Click on schedule cells to add scores to matches.

[Matches are scored in the schedule in the same way they are scored in other contexts.](tmx_tournament_scoring.html#score-entry)

{% include image.html file="ch_schedule_status.png" alt="Schedule Status" caption="Schedule Status" %}

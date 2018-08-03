---
title: Tournament Information Tab
keywords: tournament information
sidebar: ch_sidebar
permalink: tmx_tournament_information.html
toc: true
---

## Introduction

Tournament Information is used primarily when printing/saving PDF Sign-in Sheets, Event Draws, and Tournament Schedules.  

Tournament __Start__ and __End__ dates determine the days on which events may be scheduled.

{% include image.html file="ch_challenge_edit.png" alt="Add Player" caption="Tournament Editing Mode" %}

## Saving Tournament Data

Tournament data is automatically saved locally as changes are made.  There are two options for backing up tournament data and sharing tournaments with others.

{% include image.html file="ch_tournaments_save.png" alt="Save Tournament" caption="Save Options" %}

The __UP__ arrow pushes the __Tournament Record__ to the [CourtHive Cloud Server](tmx_cloud_server.html) from which it may be retrieved by any other user who has the tournament in their calendar.

The __DOWN__ arrow exports the __Tournament Record__ in JSON format to the local file system.  This file may be imported into any CourtHive/TMX client by drag/dropping it into the Import/Expoert target area.

{% include image.html file="ch_tournaments_save_state.png" alt="Save State" caption="Save State" %}

The "Push" and "Export" icons change color to indicate whether changes have been made to the the local copy of the tournament since the tournament was last pushed or exported. 

__Yellow__ indicates "Out of Date" and __Green__ indicates "Up to Date".

{% include note.html content='When Tournament Events are completed, Tournament Records are automatically "pushed" to the server.' %}

## Tournament Notes

Tournament Notes are only applicable when [Publishing](tmx_publishing_overview.html) is enabled.

{% include image.html file="ch_tournament_notes_edit.png" alt="Notes" caption="Editing Tournament Notes" %}

Tournament notes are "sanitized" to prevent [XSS Attacks](https://en.wikipedia.org/wiki/Cross-site_scripting); this means that only a subset of HTML tags are allowed.

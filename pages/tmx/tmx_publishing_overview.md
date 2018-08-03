---
title: How Publishing Works
keywords: Publishing Live Scores
sidebar: ch_sidebar
permalink: tmx_publishing_overview.html
toc: true
---

## Published Content

There are three types of information that can be published from [CourtHive/TMX](https://courthive.com/tmx) to [CourtHive/Live](https://courthive.com/live):
* Tournament Details (Name, Dates)
* Tournament Schedules / Order of Play (OOP)
* Tournament Events

## Requirements for Publishing

Publishing is only available once an [Organization Key](tmx_configuration.html) has been entered.  Once a valid configuration key has been entered, publishing icons will appear on Tournament Information Tabs when in __Editing Mode.__

It is only possible to edit and publish a tournament if the CourtHive/TMX client is configured for the same Organization to which the tournament belongs.

## Browser Identities

Each browser (Chrome, Opera, Firefox, Safari) on every computer receives a Universal Unique Identifier (UUID).  Additionally, if you log into Chrome using different Google Accounts, then each browser account __on the same computer__ has its own UUID.

{% include important.html content='An Authorization Key must be entered in the same browser identity which will be used to publish a tournament. Entering an Authorization Key in Firefox will not authorize a Chrome browser for a given tournament; and entering an Authorization Key while logged in as one user will not authorize other user accounts in the same browser.' %}

The CourtHive Cloud Server (CCS) checks the UUID of clients when determining whether a tournament can be published as "Official" or "Unofficial".  The CCS only allows __one__ client at a time to be authorized to publish/unpublish a tournament.  

See: [Authorization Keys](tmx_publishing_overview.html#authorization-keys).

{% include tip.html content='Tournaments which have been published unofficially can be viewed on CourtHive/Live by appending "?test" to the URL for the Organization.' %}

## Publishing Icons

When publishing icons are visible, their color indicates whether something has been published, and if published, whether something is up-to-date or out-of-date.

{% include image.html file="ch_events_list_publishing.png" alt="Publish State" caption="Publish State" %}

Clicking on a __Publishing Icon__ initiates publishing.  An icon will not change color until the CourtHive Cloud Server has acknowledged that the published item has been received.  
<br>

| Color | Explanation |
|-------|--------|
| <img src="./images/ch_publishing_unpublished.png" alt="Publish"> | Unpublished  |
| <img src="./images/ch_publishing_published.png" alt="Publish"> | Published, Up-to-date  |
| <img src="./images/ch_publishing_outofdate.png" alt="Publish"> | Published, Out-of-date  |

In the __Events List__ clicking on a publishing icon acts like a toggle between publish/unpublish.

In the Tournament, Draws, and Schedule Tabs, click on an icon to __Publish__ and [Context Click](tmx_fundamentals.html) to __"Unpublished"__.

### Unpublishing ALL Tournament Events

[Context Clicking](tmx_fundamentals.html) the __Publishing Icon__ in the header of the __Event List__ in the __Events Tab__ will unpublish all tournament events.

### Unpublishing A Tournament

[Context Clicking](tmx_fundamentals.html) the publish icon on the __Tournaments Tab__ will completely remove a tournament from [CourtHive/Live](https://courthive.com/live).

## Authorization Keys
If you are part of an organization which has approved the use of CourtHive, tournaments can be officially published only after an authorization key has been entered.  

Authorization Keys are __single use__, meaning that once they have been entered they cannot be reused.  Only one browser on one computer may be authorized to officially publish tournaments.

{% include image.html file="ch_home_green.png" alt="Authorized" caption="Authorized" %}

If a tournament is not included in your calendar, the authorization key will add the tournament.  

["Context Click"](tmx_fundamentals.html) on the Home Icon to see the authorization message.  

{% include tip.html content="Click on an authorization message to go directly to a tournament." %}

## Example Scenarios

Each browser has a unique identity, and entering a single-use authorization key gives the server that browser's unique identifier, so only that specific browser can publish "officially".

The browser into which an authorization key is entered must already be configured for the SAME ORGANIZATION which created the tournament.

The only difference between an Organization __Admin__ key and a __Referee__ key is that someone with an __Admin__ key can generate Tournament Authorization Keys.

In order to generate an authorization key, an admin obviously has to have the tournament in their calendar... it has to be on the admin computer.  If the referee doesn't have the tournament in their calendar, the tournament will be added to their calendar automatically (from the server) when they enter the authorization key.

Every Referee who has an Organization Key can create and publish their own tournaments "Unofficially".  (Different versions of the same tournament can be published "unofficially" and "officially").

Any referee with an organization key can also "PULL" (cloud fetch) an official version of a tournament from the server, but only if the entire tournament has been "PUSHED" to the server (Up Arrow on the Tournaments Tab).

If a referee creates their own tournament which is not in the admin calendar, then how can the admin generate an authorization key for that tournament?  The only way is for the referee to EXPORT the tournament locally, SEND the tournament to the __Admin__ (via email/message) and have the __Admin__ drag/drop import the tournament into their local calendar so that they will have the tournament ID in their system...

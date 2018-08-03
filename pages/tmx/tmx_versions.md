---
title: Versions
keywords: Versions
sidebar: ch_sidebar
permalink: tmx_versions.html
toc: true
---
## Release cycle
* CourtHive/TMX is in continuous development with frequent releases.  
* The current "stable" version can always be found at [https://CourtHive.com/tmx](https://CourtHive.com/tmx).  
* If your organization hosts a version of CourtHive/TMX, the release cycle may be defined by the organization.

## Understanding the Version Number
The version number follows this pattern:  _Major.minor.added.changed.fixed_

* Every time a __minor__ release is made, _changed_ and _fixed_ are reset to zero.
* Every time a __major__ release is made, _added_, _changed_, and _fixed_ are reset to zero.
* There will be only 9 minor releases within each major release.

## Updating to the latest version
If your browser supports [Service Workers](https://caniuse.com/#feat=serviceworkers), then a version of CourtHive/TMX is cached locally.  The Home icon turns __yellow__ to indicate that a new version is available.  

{% include image.html file="ch_home_yellow.png" alt="Update" caption="Update Message" %}

[Context Click](tmx_fundamentals.html) on the Home icon to see the update message. When a new version is available, the Service Worker begins updating your cache after you refresh your browser.

{% include image.html file="ch_new_version.png" alt="Update" caption="Update Available" %}

{% include important.html content="At present you will need to wait a minute or so then refresh your browser a second time to insure that the latest version is loaded; hopefully by the 1.0 release all of this will take place smoothly in the background." %}

{% include note.html content="If your browser __does not__ support Service Workers then refreshing your browser will always load the current version, but you will not be able to load CourtHive/TMX when you are not connected to the internet." %}

{% include tip.html content="Context Click on the Home Icon at any time to check your version." %}

## Old and New Versions
* The __last__ version of CourHive/TMX are available on: [https://CourtHive.com/tmx-](https://CourtHive.com/tmx-)
* The __next__ release candidate is available on [https://CourtHive.com/tmx+](https://CourtHive.com/tmx+)
* __Bleeding edge__ releases and urgent bug fixes are available on [https://CourtHive.com/tmx++](https://CourtHive.com/tmx++)

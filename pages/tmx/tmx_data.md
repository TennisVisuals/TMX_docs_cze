---
title: Local and Remote Data
keywords: data management
sidebar: ch_sidebar
permalink: tmx_data.html
toc: false
---

## Local Data

CourtHive/TMX makes use of [IndexedDB](https://en.wikipedia.org/wiki/Indexed_Database_API) to build a local database which includes (among other things) settings, players, rankings, tournaments, matches and points.

__IndexedDB__ is part of all modern browsers, but its function can sometimes be restricted by particular browser settings, including [Private Browsing](https://en.wikipedia.org/wiki/Privacy_mode).

CourtHive/TMX uses the Home Icon to indicate when there may be issues with the persistence of local data.  If a possible issue is detected, the Home Icon turns <font color='red'>Red</font>.  Data may still be saved, but it is not guaranteed, which means the [User Agent](https://en.wikipedia.org/wiki/User_agent) may in some cases delete  site-specific data.

See [Tournament Information](tmx_tournament_information.html) for instructions on how to push/pull copies of tournaments to/from the CourtHive Server and save copies of tournaments locally. See [Local Data](tmx_data_local.html) for instructions on how to reload tournaments from your local file system.

The local database can be populated in two ways:
* Drag/Drop of JSON, XLSX, or CSV Files: See [Importing/Exporting Local Data](tmx_data_local.html)
* Fetching Data from the Cloud: See [Uploading/Downloading Cloud Data](tmx_data_cloud.html)

## Remote Data

CourtHive/TMX uses [Web Sockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) to communicate with a CourtHive Cloud Server (CCS).  The CCS can both manage a data store and access third party data stores, such as a database hosted on a server maintained by a national tennis federation.

When CourtHive/TMX has been configured with a key supplied by a third party organization it knows how to synchronize its local data with the remote data provided by the third party.

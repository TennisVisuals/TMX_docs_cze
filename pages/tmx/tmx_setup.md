---
title: CourtHive/TMX Setup
keywords: Installation, Setup
sidebar: ch_sidebar
permalink: tmx_setup.html
toc: false
---
## Configure Your Browser

CourtHive/TMX is implemented as a [Progressive Web App](https://en.wikipedia.org/wiki/Progressive_Web_Apps){:target="_ blank"}, which means that after it is opened in your browser for the first time, it can be launched even when the internet is disconnected... provided that your browser supports [Service Workers](https://caniuse.com/#feat=serviceworkers).  

{% include tip.html content="Create a bookmark to [CourtHive.com/tmx](https://CourtHive.com/tmx) to launch the application when you are offline." %}

Some browsers, such as Firefox, disable Service Workers when cookies are disabled.  To use all of the features of CourtHive/TMX you should allow cookies (even thought CourtHive/TMX doesn't make use of cookies).

{% include important.html content="For full offline support, allow cookies for Courthive.com" %}

## Check Your Default Settings

From the Home Screen, click on the settings icon to configure your preferences.  If you have been given a [Configuration Key](tmx_configuration.html) some settings may have been configured for you and may be unavailable (such as Organization Logos).

{% include image.html file="ch_settings_icon.png" alt="Settings" caption="Settings" %}

| Tab | Setting Name | Explanation |
|-------|--------|---------|
| Org | Logos | Upload logos for use on PDF Sign-in Sheets, Schedules, and Draws |
| General | Week Starts Monday | Set first week day to Monday instead of Sunday |
| Search | Last Name, First Name | Reverse the default order when typing names |
| Search | Diacritics | Search using Diacritics (accents above/below characters) |
| Draws | Compressed Draw Formats | Whether to allow 12, 24, 48 draw sizes |
| Draws | Automatic Bye Placement | De-select if you want to place Byes manually |
| Draws | Fixed Bye Order | Do not place byes strictly by seeding |
| Draws | LL from All Qualifying Rounds | Include losers from all rounds on LL sign up sheet |
| Draws | Court Details | Display scheduled court in draw |
| Draws | Matches Before Count | Display # of prior matches  in draw |
| Publishing | Require Confirmation | Do not publish without confirmation |
| Publishing | Publish when score entered | Immediate publishing |
| Printing | Save PDFs | Save immediately instead of opening in a new tab |
| Schedule | Scores in draw order| As opposed to Winner Score first |
| Schedule | Schedule Completed Matches | Show completed matches in search |

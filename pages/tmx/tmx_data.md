---
title: Lokální a vzdálená data
keywords: data management
sidebar: ch_sidebar
permalink: tmx_data.html
toc: false
---

## Lokální data

CourtHive/TMX využívá [IndexedDB](https://en.wikipedia.org/wiki/Indexed_Database_API) ke stavbě lokální databáze která zahrnuje zejména nastavení, hráče, žebříčky, turnaje, utkání a body.

__IndexedDB__ je součástí všech moderních internetových prohlížečů ale tato funkce může být někdy omezena v nastavení prohlížeče, i včetně [Private Browsing](https://en.wikipedia.org/wiki/Privacy_mode).

CourtHive/TMX používá ikonu Domů k indikaci problému s perzistencí lokálních dat.  Pokud je problém zjištěn, ikona Domů se zbarví <font color='red'>červeně</font>.  Data mohou být i tak uložena ale není to garantováno. To znamená, že [User Agent](https://en.wikipedia.org/wiki/User_agent) může
v některých vybraných případech smazat tato data specifická pro konkrétní internetovou stránku.

Viz [Informace o turnaji](tmx_tournament_information.html) pro instrukce jak odeslat/stáhnout kopie turnajů na/z CourtHive Cloud Serveru a uložit kopie turnajů lokálně.

Viz [Lokální data](tmx_data_local.html) pro instrukce jak znovu nahrát turnaje z vlastního lokálního úložiště souborů.

Lokální databáze může být naplněna dvěma způsoby:
* Chyť/Pusť JSON, XLSX, nebo CSV soubory: Viz [Import a export lokálních dat](tmx_data_local.html)
* Přivedení dat z Cloudu: Viz [Odesílání a stahování cloudových dat](tmx_data_cloud.html)

## Vzdálená data

CourtHive/TMX používá [Web Sockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) ke komunikaci s CourtHive Cloud Serverem (CCS).  CCS může spravovat vlastní datové úložiště a přistupovat k datovým úložištím třetích stran, jako databáze hostované na serveru spravovaném národní tenisovou asociací.

Pokud byl CourtHive/TMX konfigurován s klíčem dodaným třetí stranou, tak sám rozpozná jak synchronizovat svá lokální data se vzdálenými daty poskytnutými touto třetí  stranou.

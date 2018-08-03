---
title: Konfigurační klíče
keywords: Installation, Setup
sidebar: ch_sidebar
permalink: tmx_configuration.html
toc: false
---

{% include image.html file="ch_keys.png" alt="Configuration Keys" caption="Ikona klíče" %}

Konfigurační klíče se dodávají ve dvou variantách:
* __Organizační klíče:__ poskytnuty organizacím, které validovaly CourtHive pro použití na turnajích.  
* __Autorizační klíče:__ jednorázoví klíče generované správci organizace

Oba typy klíčů jsou zadávány pomocí dialogu Klíče, ke kterému přistupujete kliknutím na ikonu Klíče na domovské stránce.

{% include image.html file="ch_enter_key.png" alt="Enter Configuration Key" caption="Zadejte konfigurační klíč" %}

{% include important.html content="Klíč musí být zadán nebo zkopírován a vložen do vstupního pole a musí být klepnuto na tlačítko Odeslat (nebo musí být stisknuto tlačítko Enter / Zpět), aby se klíč aktivoval." %}

{% include tip.html content="Klávesové zkratky pro kopírování / vkládání jsou Command-C / Command-V (Mac) a Control-C / Control-V (Windows)" %}

Klíč může určit výchozí nastavení pro koncového uživatele, stejně jako specifická nastavení jen pro danou organizaci jako např. jak mohou být tvořeny hrací plány turnajů a jak mohou být data vyměňována s jinými systémy. Klíč může také aktivovat nebo deaktivovat funkce systému a rozlišovat role v organizaci, jako je například rozhodčí nebo správce.

{% include note.html content='Pokud není konfigurační klíč "jednorázový", je uložen jako "existující" klíč v lokální databázi. Pokud organizace změní výchozí konfiguraci nebo pokud rozhodčí potřebuje přepnout mezi dvěma různými organizacemi, mohou být uložené klíče znovu načteny.' %}

## Funkce konfigurované pomocí klíče

### Aktivovat / Deaktivovat
* Funkce databáze hráčů
* Funkce databáze klubů
* Výpočet stavu žebříčků
* Delegace na mobilní zařízení

### Systémové služby
* Vzdálené zdroje dat

### Atributy organizace
* Název organizace, logo, zkratka
* Mediální sponzoři organizace
* Výchozí formáty skóre
* Tabulky bodů
* Kategorie hráčů
* Pravidla pro nasazování hráčů
* Povolit / zakázat automatické vytvoření hracích plánů

### Funkce administrátora
* Generování autorizačního klíče k oprávnění pro zveřejňování

### Reset systému
* [Obnovení / reset systému](tmx_reset.html) CourtHive/TMX do původního stavu

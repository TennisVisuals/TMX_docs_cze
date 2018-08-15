---
title: Konfigurační a autorizační klíče
keywords: Installation, Setup
sidebar: ch_sidebar
permalink: tmx_configuration.html
toc: false
---

{% include image.html file="ch_keys.png" alt="Konfigurační klíče" caption="Ikona klíče" %}

Klíče se dodávají ve dvou variantách:
* __Konfigurační klíče:__ poskytnuty organizacím, které schválili CourtHive pro použití na turnajích.  
* __Autorizační klíče:__ jednorázové klíče generované správcem / administrátorem organizace za účelem zveřejňování turnaje

Oba typy klíčů jsou zadávány pomocí dialogu "Klíče", ke kterému se přistupuje kliknutím na ikonu Klíče na domovské stránce.

{% include image.html file="ch_enter_key.png" alt="Enter Configuration Key" caption="Zadejte konfigurační klíč" %}

{% include important.html content="Klíč musí být zadán nebo zkopírován a vložen do vstupního pole a musí být kliknuto na tlačítko Odeslat (nebo musí být stisknuto tlačítko Enter / Zpět), aby se klíč aktivoval." %}

{% include tip.html content="Klávesové zkratky pro kopírování / vkládání jsou Command-C / Command-V (Mac) a Control-C / Control-V (Windows)" %}

__Konfigurační klíč__ může změnit výchozí nastavení systému pro uživatele, omezit vybrané komponenty pro použití a kontrolovat specifická nastavení jako způsob a počty nasazených hráčů, jak jsou alokovány body pro žebříčky a jestli jsou dostupné vzdálené služby pro kalendáře turnajů a registrace, jak mohou být data synchronizovány s jinými systémy.  

__Organizační klíč__ je specifickým typem konfiguračního klíče, jako je např. mappování jazyků. Klíč může také aktivovat nebo deaktivovat funkce systému a rozlišovat role v organizaci, jako je například rozhodčí nebo správce.

{% include note.html content='Pokud není konfigurační klíč "jednorázový", je uložen jako "existující" klíč v lokální databázi. Pokud organizace změní výchozí konfiguraci nebo pokud rozhodčí potřebuje přepnout mezi dvěma různými organizacemi, musí být uložené klíče znovu načteny.' %}

## Funkce konfigurovatelné pomocí klíče

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
* Povolení / zákaz automatického vytváření hracích plánů

### Funkce administrátora
* Generování autorizačního klíče k oprávnění pro zveřejňování

### Reset systému
* [Obnovení / reset systému](tmx_reset.html) CourtHive/TMX do původního stavu

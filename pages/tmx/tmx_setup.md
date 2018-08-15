---
title: Instalace CourtHive/TMX
keywords: Installation, Setup
sidebar: ch_sidebar
permalink: tmx_setup.html
toc: false
---
## Konfigurace prohlížeče

CourtHive/TMX je implementován jako [progresivní webová aplikace](https://en.wikipedia.org/wiki/Progressive_Web_Apps), což znamená, že po prvním otevření ve Vašem prohlížeči může být spuštěna i po odpojení internetu, za předpokladu, že Váš prohlížeč podporuje [Service Workers](https://caniuse.com/#feat=serviceworkers).  

{% include tip.html content="Vytvořte záložku pro [CourtHive.com/TMX](https://CourtHive.com/tmx), abyste mohli spustit aplikaci, když jste offline." %}

Některé prohlížeče, jako například Firefox, zakážou Service Workers, pokud nejsou povoleny soubory cookies. Chcete-li používat všechny funkce CourtHive/TMX, měli byste povolit soubory cookies (i když CourtHive/TMX nevyužívá cookies).

{% include important.html content="Pro plnou offline podporu povolte cookies pro Courthive.com" %}

## Kontrola výchozího nastavení

Na domovské stránce klikněte na ikonu Nastavení a nakonfigurujte své předvolby. Pokud jste obdrželi [Konfigurační klíč](tmx_configuration.html), mohla být některá nastavení už nakonfigurována a nemusí být dostupná (například Loga organizace).

{% include image.html file="ch_settings_icon.png" alt="Nastavení" caption="Nastavení" %}

| Záložka | Název nastavení | Vysvětlení |
|-------|--------|---------|
| Org | Loga | Nahrajte loga pro použití v PDF seznamech přihlášených hráčů, hracích plánech a rozpisech utkání |
| Obecné nastavení | Týden začíná v pondělí | Nastaví první týdenní den od pondělí místo neděle |
| Obecné nastavení | Odkazy na dokumentaci | Zobrazí v příslušných záložkách odkazy na dokumentaci |
| Vyhledávání | Příjmení, jméno | Při zadávání jmen se vrací výchozí pořadí |
| Vyhledávání | Diakritika | Hledání pomocí diakritiky (znaky nad nebo pod) |
| Hrací plány | Komprimovaný formát hracího plánu | Zda-li povolit komprimované hrací pole pro 12, 24 a 48 hráčů |
| Hrací plány | Automatické přidělení volných kol (byes) | Neoznačovat pokud mají být vybrána umístění volných kol (byes) manuálně |
| Hrací plány | Fixní distribuce volných kol (byes) | Volná kola fixně na řádky místo podle nasazení hráčů |
| Hrací plány | Automaticky separovat hráče podle zemí | Při automatickém losování jsou hráči ze stejných zemí odděleni |
| Hrací plány | Automaticky separovat hráče podle klubů | Při automatickém losování jsou hráči ze stejných klubů odděleni |
| Hrací plány | Lucky Losers ze všech kvalifikačních kol | Zahrnout Lucky Losers ze všech kol na seznam dostupných Lucky Losers |
| Hrací plány | Kvalifikaci navázat na soutěž útěchy | Poražení z kvalifikace se mohou zúčastnit soutěže útěchy |
| Hrací plány | Hráči v soutěži útěchy ze všech kol hlavní soutěže | Všichni poražení ze všech kol hlavní soutěže se mohou zúčastnit soutěže útěchy |
| Hrací plány | Nasazovat hráče v soutěži útěchy | V soutěži útěchy nasazovat hráče podle žebříčku |
| Hrací plány | Zobrazit vlajky zemí | Zobrazí vlajku země u každého hráče v hracím plánu |
| Hrací plány | Číslo kurtu a pořadí utkání viditelné v hracím plánu | Zobrazí číslo kurtu a pořadí utkání na kurtu v hracím plánu |
| Hrací plány | Počet předchozích utkání na dvorci | Zobrazí počet předchozích utkání na kurtu v hracím plánu |
| Hrací plány | Zobrazit datum utkání v eliminačním hracím plánu | Zobrazí i datum utkání v eliminačním hracím plánu |
| Zveřejňování | Vyžadovat potvrzení zveřejnění  | Ke zveřejnění nedojde bez potvrzení |
| Zveřejňování | Zveřejnit hned jak je skóre zapsáno | Okamžité zveřejnění |
| Zveřejňování | Zveřejnit hrací plán živě v průběhu losování | Živě v průběhu losování ukazovat zaplňování pozic na hracím plánu |
| Tisk | Uložit PDFs | Uložit okamžitě do vybrané složky namísto otevření na nové záložce prohlížeče |
| Rozpis utkání | Výsledky utkání zobrazit vždy z pohledu vítěze | Pokud zatrženo tak je skóre vždy zobrazeno z pohledu vítěze bez ohledu na to který hráč je uveden v rozpisu utkání jako první |
| Rozpis utkání | Ukončená utkání vyhledávat v rozpisu | Zobrazí ukončené zápasy ve vyhledávání |

---
title: Instalace CourtHive / TMX
keywords: Installation, Setup
sidebar: ch_sidebar
permalink: tmx_setup.html
toc: false
---
## Nakonfigurujte prohlížeč

CourtHive / TMX je implementována jako [progresivní webová aplikace](https://en.wikipedia.org/wiki/Progressive_Web_Apps){:target="_ blank"}, což znamená, že po prvním otevření ve vašem prohlížeči může být spuštěna i po odpojení internetu ... za předpokladu, že Váš prohlížeč podporuje [Service Workers](https://caniuse.com/#feat=serviceworkers).  

{% include tip.html content="Vytvořte záložku pro [CourtHive.com/tmx](https://CourtHive.com/tmx), abyste spustili aplikaci, když jste offline." %}

SNěkteré prohlížeče, jako například Firefox, zakážou Service Workers pokud nejsou povoleny soubory cookies. Chcete-li používat všechny funkce CourtHive / TMX, měli byste povolit soubory cookies (i když CourtHive / TMX nevyužívá cookies).

{% include important.html content="Pro plnou offline podporu povolte cookies pro Courthive.com" %}

## Zkontrolujte výchozí nastavení

Na domovské obrazovce klikněte na ikonu nastavení a nakonfigurujte své předvolby. Pokud jste obdrželi [konfigurační klíč](tmx_configuration.html), mohly být některé konfigurace pro vás nakonfigurovány a nemusí být dostupné (například Loga organizace).

{% include image.html file="ch_settings_icon.png" alt="Settings" caption="Settings" %}

| Záložka | Název nastavení | Vysvětlení |
|-------|--------|---------|
| Org | Loga | Nahrajte loga pro použití v PDF seznamech přihlášených hráčů, hracích plánech a rozpisech utkání |
| Obecné nastavení | Týden začíná v pondělí | Nastaví první týdenní den od pondělí místo neděle |
| Vyhledávání | Příjmení, jméno | Při zadávání jmen se vrací výchozí pořadí |
| Vyhledávání | Diakritika | Hledání pomocí diakritiky (znaky nad nebo pod) |
| Hrací plány | Compressed Draw Formats | Whether to allow 12, 24, 48 draw sizes |
| Hrací plány | Automatic Bye Placement | De-select if you want to place Byes manually |
| Hrací plány | Fixed Bye Order | Do not place byes strictly by seeding |
| Hrací plány | LL from All Qualifying Rounds | Include losers from all rounds on LL sign up sheet |
| Hrací plány | Court Details | Display scheduled court in draw |
| Hrací plány | Matches Before Count | Display # of prior matches  in draw |
| Zveřejňování | Vyžádovat potvrzení zveřejnění  | Ke zveřejnění nedojde bez potvrzení |
| Zveřejňování | Zveřejnit hned jak je skóre zapsáno | Okamžité zveřejnění |
| Tisk | Uložit PDFs | Uložit okamžitě namísto otevření na nové záložce |
| Rozpis utkání | Výsledky utkání v pořadí dle hracího plánu | Pokud zatrženo tak skóre z pohledu vítěze |
| Rozpis utkání | Skončená utkání vyhledávat v rozpisu | Zobrazí skončené zápasy ve vyhledávání |

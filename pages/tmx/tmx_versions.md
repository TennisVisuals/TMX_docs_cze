---
title: Verze
keywords: Verze
sidebar: ch_sidebar
permalink: tmx_versions.html
toc: true
---
## Cyklus uvolňování nových verzí
* CourtHive / TMX je v neustálém vývoji s častým vydáváním nových verzí.  
* Aktuální "stabilní" verze je vždy k dispozici na adrese [https://CourtHive.com/tmx](https://CourtHive.com/tmx).  
* Pokud organizace hostuje verzi služby CourtHive / TMX, může tato organizace definovat cyklus uvolňování nových verzí.

## Vysvětlení čísla verze
Číslo verze následuje tento vzor:  _Major.minor.added.changed.fixed_

* Pokaždé, když dojde k __menšímu__ uvolnění nové verze, změní se a fixuje se na nulu.
* Pokaždé, když dojde k __rozsáhlému__ uvolnění nové verze, přidání, změna a oprava se vynulují.
* V každé hlavní verzi bude pouze 9 malých vydání nových verzí.

## Aktualizace na nejnovější verzi
Pokud váš prohlížeč podporuje [Service Workers](https://caniuse.com/#feat=serviceworkers), pak je verze aplikace CourtHive / TMX uložena v lokální mezipaměti. Ikona Domů svítí žlutě, což znamená, že je k dispozici nová verze.  

{% include image.html file="ch_home_yellow.png" alt="Update" caption="Zpráva o aktualizaci" %}

[Kontext kliknutím](tmx_fundamentals.html) na ikonu Domů zobrazíte aktualizační zprávu. Je-li k dispozici nová verze, Service Workers po aktualizaci začne aktualizovat lokální mezipaměť.

{% include image.html file="ch_new_version.png" alt="Update" caption="Aktualizace k dispozici" %}

{% include important.html content="V současné době budete muset chvíli počkat a potom obnovit prohlížeč podruhé, abyste se ujistili, že je načtena nejnovější verze. Doufáme, že v 1.0 vydání to vše bude probíhat hladce na pozadí." %}

{% include note.html content="Pokud váš prohlížeč nepodporuje Service Workers, obnovení prohlížeče vždy načte aktuální verzi, ale nebudete moci načíst CourtHive / TMX, pokud nejste připojeni k internetu." %}

{% include tip.html content="Kontext kliknutím na ikonu Domů můžete kdykoli zkontrolovat aktuální verzi." %}

## Staré a nové verze
* Poslední verze CourHive / TMX je k dispozici na adrese: [https://CourtHive.com/tmx-](https://CourtHive.com/tmx-)
* Další kandidát na vydání nové verze je k dispozici na adrese: [https://CourtHive.com/tmx+](https://CourtHive.com/tmx+)
* Naléhavé opravy chyb naleznete na adrese: [https://CourtHive.com/tmx++](https://CourtHive.com/tmx++)

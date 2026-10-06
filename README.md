# Jae-Encyklopedia

Česká encyklopedie k MMORPG **Aion 2** – jeden statický soubor `index.html` (HTML + Tailwind + vanilla JS), určený pro GitHub Pages.

## Co v ní je
- **8 záložek:** Úvod, Obecné, PvE Obsah, PvP Obsah, Progrese a Ekonomika, Nástroje a Limity, To-Do List, Mapa (většina má podzáložky).
- **Časovače v hlavičce:** Rift, Shugo Festival, denní a týdenní reset, Artifact Siege, Abyss boss (v UTC; autoritativní je vždy in-game countdown).
- **Kalkulačky:** Odyle Energy, Enhancement a další v záložce Nástroje a Limity.
- **To-Do List:** denní a týdenní rutina a vlastní poznámky. Stav se ukládá v prohlížeči (`localStorage`) a maže se po resetu – denní každý den v 07:00 UTC, týdenní každou středu v 07:00 UTC.
- **Interaktivní mapa:** zóna Altgard (vložená z externí stránky).

## Pravidla obsahu
- Odyle Energy je vázaná na postavu, ne na účet.
- V endgame speed-runech se trash moby přeskakují; povinné progresní mechaniky (např. v Transcendence) přeskočit nejde.

## Nasazení
Stačí nahrát `index.html` do větve nasazené přes GitHub Pages. Stránka při běhu načítá Tailwind (`cdn.tailwindcss.com`), Chart.js (jsDelivr) a písmo Cinzel z Google Fonts, takže potřebuje připojení k internetu.

## Poznámky
- Tailwind se načítá přes CDN (vývojářský režim). Pro trvalý provoz je lepší vlastní build s vygenerovaným CSS.
- Mapa se vkládá přes `<iframe>`; pokud ji zdrojová stránka zakáže, funguje odkaz „Otevřít plnou mapu v novém okně“.

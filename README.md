# WFT Bieb

Doorzoekbare bibliotheek van wet- en regelgeving voor financiële dienstverleners, door Bureau DFO.

Live: https://jeroen-o.github.io/dfo-wft-bieb/

- `index.html`: de volledige pagina (standalone, geen build-step nodig)
- `robots.txt`, `sitemap.xml`, `llms.txt`: vindbaarheid voor zoekmachines en AI-assistenten

## Toegang

De pagina vraagt om een wachtwoord (niet hoofdlettergevoelig). Dit is een drempel in de browser en geen echte beveiliging: de inhoud staat in de broncode en in deze repository. Een ingelogde bezoeker blijft ingelogd tot het tabblad wordt gesloten.

Wachtwoord wijzigen: bereken de SHA-256 van het nieuwe wachtwoord in kleine letters, bijvoorbeeld met `printf '%s' 'nieuwwachtwoord' | sha256sum`, en vervang de waarde van `SLOT_HASH` in `index.html`.

## Onderhoudskalender

| Wanneer | Wat |
|---|---|
| Elk kwartaal | Peildatum bovenaan bijwerken; kaarten met "Verwijzing te verifiëren" nalopen; blok "Wat er dit jaar verandert" actualiseren |
| December/januari | TRHK (financieringslastpercentages), NHG Voorwaarden & Normen en Besluit kinderopvangtoeslag controleren op de nieuwe jaarversie |
| Bij nieuwe wetgeving | CCD II-implementatiewet, AMLR (vanaf 2027), AI-verordening en Wtp-transitie: beschrijving en link aanpassen |
| Jaarlijks | Links in "Kennis en praktijk" en "DFO Compliance" controleren op dode links; FAQ juridisch laten nalezen |

Na het wijzigen van de `WETTEN`- of `KENNIS`-data werkt de pagina direct. De voorgerenderde kaarten en de JSON-LD in `index.html` lopen dan achter tot ze opnieuw worden gegenereerd; dat raakt alleen crawlers zonder JavaScript.

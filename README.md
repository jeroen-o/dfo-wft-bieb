# WFT Bieb

Doorzoekbare bibliotheek van wet- en regelgeving voor financiële dienstverleners, door Bureau DFO.

Live: https://jeroen-o.github.io/dfo-wft-bieb/

- `index.html` — de volledige pagina (standalone, geen build-step nodig)
- `robots.txt`, `sitemap.xml`, `llms.txt` — vindbaarheid voor zoekmachines en AI-assistenten

Na het wijzigen van de `WETTEN`- of `KENNIS`-data werkt de pagina direct. De voorgerenderde kaarten en de JSON-LD in `index.html` lopen dan achter tot ze opnieuw worden gegenereerd; dat raakt alleen crawlers zonder JavaScript.

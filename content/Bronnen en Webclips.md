---
{"publish":true,"title":"Bronnen en Webclips","created":"2025-12-15","modified":"2025-12-15T11:40:02.775+01:00","cssclasses":""}
---

[[PKM Research Notes]]

Mijn verzameling bronnen is groot. De verzameling bestaat voornamelijk uit Webclips en teksten uit boeken en artikelen.  Ik maak vanuit de bronnen wikilinks naar verzamelpagina's zoals [[PKM Research Notes]] of naar meer specifieke notities over onderwerpen. 

## Webclips

Webclips verzamel ik met hulp van de "Obsidian Web Clipper", in mijn geval de officiële Safari Extension. Staat uitgebreid beschreven op de [Obsidian Help Website](https://help.obsidian.md/web-clipper)

Ik gebruik altijd #webclip als tag en voor heel algemene onderwerpen gebruik ik ook tags als \#politiek, \#koffiemerken, \#films enz. in de properties van mijn webclips.

De extensie komt met een aantal standaard templates die prima voor mij voldoen. Ik voeg alleen de tag "webclip" standaard toe een een wikilink naar de meest gebruikte "Inbox" notitie van dit moment. 

## Geschreven bronnen

Ik haal veel teksten uit papieren bronnen. Om dat te doen maak ik foto's van de pagina en maak ik van de teksten in de foto's een tekst in een notitie over die bron. Ik gebruik hiervoor mijn [[Paste Text from selected Images]]  Apple Shortcut. Werkt heel efficient op deze manier. 

- [ ] Toekomst nog eens een QuickAdd Macro samenstellen die een standaard notitie geneert adhv onderstaande template en die daarna mijn Shortcut aanroept om te tekst erin te zetten.

Ik gebruik de volgende template:

```
---
title  : <% tp.file.title %>
date   : <% tp.file.creation_date("YYYY-MM-DD") %>
source : "[[name-of-the-source]]"
author : "[[name-of-the-author]]"
summary: "My summary"
---
[[link-to-inbox]]

My own notes and links added

"Pasted text from photo's"
```

De template gaat er dus van uit dat ik voor elke Source en Author ook een verzamel notitie heb.  Daarin kun je informatie vinden en toon ik altijd aan het einde de backlinks via Bases of Dataview. 


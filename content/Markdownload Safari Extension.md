---
title: Markdownload Safari Extension
date: 2025-12-01
---
parent: [[Obsidian praktijktips]]

Ik maak veel gebruik van "knipsels" die ik van websites haal. En vaak wil ik ook hele artikelen opslaan uit kranten, tijdschriften enz.

De Safari EXtension "Markdownload" helpt daarbij enorm. Hij kan een heel artikel (webpagina) downloaden en maakt er tegelijkertijd "markdown" van. 

## Installeren

[Download hem hier](https://apps.apple.com/nl/app/markdownload/id1554029832?l=en-GB&mt=12)
Hij ondersteunt "Familiy sharing" dus je hoeft als lid van de Apple "Family" er niet voor te betalen.

## Gebruik

Er zijn verschillende manieren in Safari om de extensie op te roepen, je ziet ze uitgelegd als je de extensie aanklikt in Safari instellingen. Meest gebruikt door mij:

- download de complete pagina, maak zo nodig aanpassingen.
- copy current tab as markdown to clipboard (zonder aanpassingen)

## Instellingen

Je moet de extensie wel even instellen voordat je hem gebruikt in de instellingen van Safari
Ik denk dat de meeste instellinen wel standaard goed staan maar je moet het even goed controleren of anders er even mee experimenteren.

Mijn header ziet er als volgt uit:
```
---
title  : {pageTitle}
tags   : [webpage]
author : {byline}
date   : {date:YYYY-MM-DD}
---
[Source]({baseURI})

```

Op mijn Safari werkt de download prima maar de "Obsidian integratie" werkt niet in de zin dat het .md document in de downloads map terechtkomt en niet in mijn vault.  In Firefox werkt het wel goed. 

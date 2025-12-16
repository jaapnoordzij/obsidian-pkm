---
{"publish":true,"aliases":"YAML frontmatter frontmatter","title":"YAML Frontmatter","created":"2025-12-02","modified":"2025-12-15T22:43:31.911+01:00","cssclasses":""}
---

[[Concept teksten]]

Yet Another Meta Language (YAML) wordt vaak gebruikt om gegevens over een notitie (metadata) mee te geven in de tekst.  Alle Apps die met platte tekst kunnen werken negeren deze informatie bij opmaak en afdrukken.

## Syntax

De structuur van YAML is nogal simpel:

- Op de eerste regel van een notitie staan alleen 3 streepjes `---` (verder niets)
- Daarna een willekeurig aantal regels met `key: value`
- Als laatste weer een regel met alléén drie streepjes `---`

De waarde van de keys en van de value's mag je helemaal zelf weten. Obsidian kent een paar keys die standaard zijn: `tags: ` en `aliases: `
Values mogen hoofdletters bevatten en kleine letters. De meeste apps negeren het verschil maar het is netter om altijd kleine letters te gebruiken. Voor values maakt het niet uit.

Obsidian kent sinds versie 10.0 (?) de term "[properties](https://help.obsidian.md/properties)" voor YAML frontmatter / headers.
Wanneer je rechts bovenin kiest voor "All properties" zie je alle keys die je gebruikt in je vault en kun je daar ook op selecteren. Maar ik typ het altijd zelf in. Meestal zet ik ze in een template die ik toepas.

Hoewel de waarde formeel vrij te kiezen is kent Obsidian wel specifieke kenmerken toe, je ziet dat aan de iconen in de lijst:

- Datum velden
- Tekst verlden
- Numerieke velden
- Boolean velden
- Lijsten
- Geneste velden (komen weinig voor)

Nogmaals de keuze is vrij arbitrair en formeel kent de YAML standaar dat onderscheid nauwlijks. Het is wel van belang om een paar dingen te weten die specifiek voor Obsidian gelden zodat je er goed mee kunt werken in formules in "bases" bijvoorbeeld :

1. Je kúnt links opnemen in YAML headers. Zorg er dan voor dat de link tussen dubbele quotes staat. In dat geval ziet Obsidian het ook als een link. Dat is pas sinds kort, Hoera!
2. Voor `tags:` en `aliases:` geldt dat de waarde sinds kort uit een Lijst moet bestaan tenzij er maar één waarde is. Een lijst betekent dat de waarden tussen enkele haken moeten staan [a,b] of op meerder ingesprongen regels moeten volgen waarbij elke regel begint met een hyphen voor de waarde
3. Datums moeten in ISO formaat zijn: 2025-12-02 voldoet hieraan.

Een voorbeeld:
```
---
bookId: '50469'
title: Waardenloze politiek
author: "[[Tom van der Meer]]"
highlightsCount: 71
tags: [boeken, politiek]
date:
  - 2025-12-02
  - 2024-11-02
---
```
Tags en date zijn correcte lijsten.

## Gebruik

YAML is een manier om de informatie over je notities te structuren. Het is dus in hoge mate afhankelijk van de manier waarop je informatie organiseert en toepast en dat is erg persoonlijk.

Plugins als "Dataview" en de Obidian Core Plugin "Bases" gebruiken deze waarden om overzichten te maken, te sorteren en filters toe te passen.

Waar gebruik ik het voor ?

1. Ik vind het vaak belangrijk om te weten wat voor "soort" notitie het is. Gaat het over een boek, een film, een auteur, over wat dan maar ook. Ik gebruik daarvoor meestal de waarde `class:` (komt nog uit mijn object-oriented programmeer ervaring).
2. Ik gebruik zoveel mogelijk een `date:` veld. Dat maakt de notitie onafhankelijk van de systeem "file creation date". Er staat tegenover dat je de creation date niet makkelijk kunt veranderen maar deze datum natuurlijk wel. Datum velden zijn vooral vaak geweldig handig voor het sorteren van overzichten.
3. Ik gebruik ook vaak een `title:` veld. Boven de notitie staat alijd de filenaam (zonder .md extensie) maar er zijn best gevallen waar de naam van de pagina voor mij niet de naam van de file hoeft te zijn. "Inleiding" als `title` kan dan prima samengaan met "inleiding op mijn boek over planten" als filenaam.
4. De overige waarden zijn vaak gerelateerd aan de "soort" notitie. Een notitie over `boardgame` gebruikt numerieke waarden voor complexiteit en rating, een notitie over een `boek` bevat velden over het publicatie jaar, de auteur (link naar "auteur" notitie), het ISBN nummer, de pagecount enz. Al die waarden kun je weer nuttig gebruiken bij het genereren van overzichten van boardgames, boeken enz.

Het ideaal is natuurlijk dat je informatie perfect georganiseerd is. Dat alle notities over boeken dezelfde YAML indeling hebben enz.  Je kunt dat het makkelijkst voor elkaar krijgen door te werken met templates. Obsidian heeft templates als core pluging maar de de "community plugin" Templater kan veel meer. Ik gebruik die dus het meest. Je kunt dan bij het aanmaken van een notitie met een gespreksverslag de template voor een "Gespreksverlag" met alle bijbehorende (lege) velden direct meegeven.

Maar realiseer je ook dat dit een ideaal is. In mijn personal Vault met bijna 9000 notities, samengesteld over een periode van zo'n 20 jaar en na talloze conversies van andere apps, is deze ordening ver te zoeken en faal ik vaak jammerlijk in het samenstellen van mijn moooie overzichten.

Dat is niet erg. Je kunt altijd en vrij makkelijk bestaande files  / templates aanpassen zodat het allemaal weer iets beter wordt. Uiteindelijk is het allemaal maar gewoon "platte tekst" en een shell / python scriptje doet vaak wonderen over honderden files.

---
title: Gebruik van Tags, Folders en Metadata
date: 2023-01-23
---
parent: [[Obsidian praktijktips]]

Moet ik Links, Tags, Metadata of Folders gebruiken om aan te geven waar een notitie over gaat ?

## Het probleem

Ik heb de behoefte om het soort pagina vast te leggen in een notitie. Voor Boeken en Films is dat evident. Voor Auteur en Regisseur wat minder maar ook gewenst. Voor veel andere zaken niet zo duidelijk (Dagboek, Dataview, Workflow, ...)

Er zijn meerdere methodes denkbaar om dit voor elkaar te krijgen:
1. Gebruik een tag zoals \#boeken of \#films. Dat heb ik jarenlang gedaan met als gevolg een grote verzameling tags.
2. Gebruik folders.  Ik gebruik dat nu voor "dagboek" en "journal" meer niet.
3. Gebruik Metadata zoals xxx\:\: yyy in de tekst of in de YAML header.
4. Gebruik van (back) Wikilinks

## Overwegingen

**Folders**

Voordeel van het gebruik van folders is dat het netjes, duidelijk en standaard is als het gaat over het niveau van het filesysteem op de computer.

Folders hebben ook nogal wat nadelen:
- Een notitie kan maar in één folder tegelijk zitten. Wat doe ik met een "boek" over "filosofie"?
- Folders zijn niet beschikbaar op IOS en niet alle apps kennen het concept in de app, zelfs niet alle apps die met platte files werken: nvalt of The-Archive kennen het beide niet.
- Applicaties die de notities niet op het filesysteem opslaan (zoals Bear of Drafts) kennen het concept folder meestal niet of het is gefaket.
- Indeling in folders moet je met de hand onderhouden. Er zijn wel tools als Hazel die automatisch een bestand in de juiste folder kunnen zetten maar daarvan wil ik niet afhankelijk zijn.

**Hash-tags**

Het gebruik van Hash-tags is vrij algemeen geaccepteerd in platte tekst. Maar het is niet zo dat het helemaal gestandaardiseerd is.

Implementatie van tags verschilt nogal per app. In Bear mag veel, Obsidian tags mogen niet bestaan uit een nummer zoals 2023 en mogen geen spaties bevatten.

Geneste tags zijn bekend bij Bear en in Obsidian maar ze zijn lang niet overal bruikbaar. Niet-geneste tags zijn daarom een veiliger keuze.

Een nadeel van tags is dat ze meestal in de tekst zelf staan. Je kunt ze niet makkelijk onzichtbaar maken / negeren (voor een blog) en ze staan dus soms in de weg. 
In Obsidian kun je Tags ook opnemen in de YAML metadata.

**Metadata**

Een veilige en breed geaccepteerde manier om metadata over tekst op te nemen is in een YAML header. De implementatie verschilt nogal eens maar over het algemeen en als je niet alle features van de standaard gebruikt, werkt het goed.

Voordeel van YAML is dat de gegevens gewoon in de tekst staan maar dat ze niet gelden als onderdeel van de inhoud.  Dat werkt in vrijwel alle apps goed (maar weer niet in Bear die het concept niet kent). Het grootste voordeel van YAML is dat je de inhoud van de velden zelf kunt bepalen. Het hangt dus van je organisatiegraad af hoe efficient je ermee omgaat.

Het is ook mogelijk om metadata in de tekst zélf op te nemen maar de implementatie daarvan is absoluut niet gestandaardiseerd.  Ik kan m.b.v  de Obisidian plugin "Dataview" bijvoorbeeld iets zeggen over de Date\:\: 2023-01-23 maar geen enkele andere app kan dat lezen, zelfs Obsidian zelf ziet het niet.

Sommige apps zoals Obsidian staan toe om tags (zonder de hash) op te nemen in de (YAML) metadata als "tags". Dat werkt identiek aan het opnemen van de hash-tag in de tekst zelf. Je kunt dan de voordelen van beide combineren.

Obsidian noemt de YAML "frontmatter" overigens "Properties" en heeft daar handige overzichten van in de rechter kolom.

**Links**
Ik gebruik ook Wiki-links om naar pagina's te verwijzen. Ook dat is een goede en volgens "Zettelkasten" de beste manier.

Het moet natuurlijk allemaal handmatig dus het werkt bij mij alleen effectief voor situaties waarin ik een beperkt aantal specifieke pagina's bij elkaar wil hebben die ook echt bij elkaar horen.  Dat noem je meestal een MOC (Map of Contents). Het voordeel van handmatig werken is hier wel dat je gedwongen bent om zelf je informatie te structuren (althans, ik vind dat een voordeel).

## Conclusie

Het lijkt erop dat de beste alternatieven voor mij zijn:
1. Wikilinks om informatie te structureren voor Personal Knowledge Management.
2. Voor het overige: als Metadata in een Yaml header (géén DV "inline velden")

Beide alternatieven zijn wat mij betreft gelijkwaardig.
Dataview (inline) velden zijn heel (te) flexibel en vormen een Lock-In gevaar. Dus niet.

De consequentie is dat ik **geen** folders gebruik, alléén voor het dagboek wel.

Ik gebruik liever ook geen tags anders dan om ongestructureerde informatie te geven over of aan een notitie. Niet om notities onderling te verbinden dus en zeker niet om te structureren.

## Ter overweging

Andy Matushak
https://notes.andymatuschak.org/zF8xCU4BwXwbmSyp7tmff9i


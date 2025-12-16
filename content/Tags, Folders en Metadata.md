---
{"publish":true,"title":"Tags, Folders en Metadata","created":"2023-01-23","modified":"2025-12-16T18:43:31.348+01:00","tags":[null],"cssclasses":""}
---

parent: [[index]]

## De vraag

Ik wil in een notitie vastleggen waar hij over gaat, met welke andere notities hij verbonden is en welke andere notities eventueel op deze informatie betrekking hebben. Hoe breng ik verbanden aan tussen brokjes informatie ofwel tussen notities in Obsidian ?

Er zijn meerdere methodes om dit voor elkaar te krijgen:

1. Gebruik een tag zoals \#boeken of \#films. Dat heb ik jarenlang gedaan met als gevolg een grote verzameling tags.
2. Gebruik folders.  Ik heb dat veel gebruikt voor projecten en gebruik het nu nog voor "dagboek" en mijn week "journal".
3. Gebruik Metadata zoals xxx\:\: yyy in de tekst of in de YAML Frontmatter (Obsidian properties).
4. Gebruik van Wikilinks tussen notities.
5. Wanneer een app notities opslaat in een eigen database format zijn er meer mogelijkheden maar omdat ik alleen met "platte tekst" wil werken kijk ik daar verder niet naar.

## Folders

Voordeel van het gebruik van folders is dat het netjes, duidelijk en standaard is als het gaat over het niveau van het filesysteem op de computer.
- De meeste computes kennen een filesysteem met folders (maar IOS en Android niet)
- Je hoeft niets in de tekst zelf te veranderen.
- Sommige systemen als MacOS kunnen tags aan files geven die buiten de inhoud onzichtbaar voor de gebruiker worden opgeslagen (In die irritante .DS_Store files)
- Het aantal folders dat je kunt maken is meestal onbeperkt.

Folders hebben ook nogal wat nadelen:
- Een notitie kan maar in één folder tegelijk zitten. Wat doe ik met een "boek" over "filosofie"?
- Folders zijn niet beschikbaar op IOS en niet alle apps kennen het concept binnen de app zelfs niet alle apps die met platte files werken: [nvalt](https://brettterpstra.com/projects/nvalt/) of [The-Archive](https://zettelkasten.de/the-archive/) kennen het niet.
- Sommige applicaties pretenderen folders te gebruiken (zoals Bear of Drafts) slaan hun files niet op het filesysteem op maar in een min of meer gesloten database.
- Indeling in folders moet je met de hand onderhouden. Er zijn wel tools als Hazel die automatisch een bestand in de juiste folder kunnen zetten maar de vraag is of je daarvan afhankelijk wil zijn.

## Hash-tags

Het gebruik van Hash-tags is vrij algemeen geaccepteerd in platte tekst. Maar het is niet zo dat het helemáál gestandaardiseerd is. De werking van tags verschilt nogal per app. In Bear mag bijna alles, Obsidian tags mogen niet bestaan uit een nummer zoals 2023 en mogen geen spaties bevatten, erg handig als een paar duizend dagboek aantekeningen moet overzetten die geneste tags met jaar/maand/dag gebruiken om als organisatievorm.

Omdat hash-tags worden bijgehouden op het hoogste niveau van de app is het lastig om een fijnmazige structuur aan te brengen in de kennis. Dat kan wel maar dan krijg je al snel een enorme hoeveelheid tags.

Wanneer je onderlinge relaties wilt aanbrengen tussen tags kun je dat vaak doen met "geneste" tags zoals food/nagerecht. Geneste tags zijn bekend bij Bear en in Obsidian maar ze zijn lang niet overal bruikbaar. Niet-geneste tags zijn daarom een veiliger keuze en dat betekent dat het lastig is om (anders dan via de naam) structuur aan te brengen tussen tags onderling.

Een groter nadeel van tags is dat ze meestal in de tekst zelf staan. Je kunt ze niet makkelijk onzichtbaar maken / negeren voor een publicatie en ze staan dus soms in de weg. In Obsidian kun je Tags opnemen in de YAML metadata.

Je kunt hash-tags dus het best gebruiken wanneer je in het algemeen iets wilt zeggen over de notitie, waar het over gaat of waar het betrekking op heeft.

## Metadata

Een veilige en breed geaccepteerde manier om metadata over tekst op te nemen is in een YAML "frontmatter" of "properties" (Obsidian). De implementatie verschilt wel eens maar over het algemeen en als je niet alle features van de standaard gebruikt, werkt het goed. In de [[YAML Frontmatter]] kun je net zoveel key / value pairs bedenken als je wilt.

Voordeel van YAML is dat de gegevens gewoon in de tekst staan maar dat ze niet gelden als onderdeel van de inhoud.  Dat werkt in vrijwel alle apps goed (maar weer niet in Bear die het concept niet kent). Het grootste voordeel van YAML is dat je de inhoud van de velden zelf kunt bepalen. Het hangt dus van je organisatiegraad af hoe efficient je ermee omgaat.

Het is soms ook mogelijk om metadata in de tekst zélf op te nemen maar de implementatie daarvan is absoluut niet gestandaardiseerd.  Ik kan m.b.v  de Obisidian plugin "Dataview" bijvoorbeeld iets zeggen als `created:: 2023-01-23` maar geen enkele andere app kan dat lezen, zelfs Obsidian "core" ziet het niet. Alleen Dataview kan er leuke dingen mee doen. Ik gebruik het niet (meer).

Obsidian staan toe om tags (zonder de hash !) op te nemen in de [[YAML Frontmatter\|frontmatter]] als "tags". Dat werkt identiek aan het opnemen van de hash-tag in de tekst zelf. Je kunt dan de voordelen van beide combineren.

Obsidian noemt de YAML "frontmatter" overigens "Properties" en heeft daar handige overzichten van in de rechter kolom.

## Wikilinks

Ik gebruik ook Wiki-links om naar pagina's te verwijzen. Ook dat is een goede en volgens  de [Zettelkasten](https://zettelkasten.de/the-archive/) methode de beste manier.

Het moet natuurlijk allemaal handmatig dus het werkt bij mij vooral effectief voor situaties waarin je een relatief beperkt aantal specifieke pagina's bij elkaar wil hebben die ook echt bij elkaar horen.  Dat noem je meestal een MOC ([[Map of Content]]). Het grote voordeel van handmatig werken is hier wel dat je gedwongen bent om zelf je informatie te structuren. Voor mij heeft daarom het werken met Wikilinks de voorkeur.

Uiteindelijk wil je waarschijnlijk het netwerk van Wikilinks zoveel mogelijk sluitend hebben maar dit situatie bereik je meestal pas aan het eind van een proces van nadenken en structureren van notities. Een krachtig hulpmiddel daarbij is het toepassen van "backlinks" zoals omschreven bij de [[Map of Content]].  Dat betekent dat je vooral verwijst naar "parent" pagina's om aan te geven dat een notitie bij die anderen parent notitie "hoort" zonder op dat moment precies te weten hoe die relatie er uit ziet.

Met ingebouwde functie van Obsidian of met een Dataview script of met een obsidian "bases" definitie kun je aan het einde van een note een lijst generen van de "Backlinks" dus de notities die hiernaar verwijzen.  In je review proces kun je daarmee aan de slag om te categoriseren en te herschrijven.

## Conclusie

Het lijkt erop dat de beste alternatieven voor mij zijn:

1. Wikilinks om informatie te structureren voor Personal Knowledge Management.
2. Voor het overige: als Metadata in een Yaml header (géén DV "inline velden")

Ik gebruik liever geen hash-tags anders dan om ongestructureerde informatie te geven over of aan een notitie. Niet om notities onderling te verbinden dus en zeker niet om te kennis te structureren.

Ik gebruik vrijwel **geen** folders om kennis te structureren.

## Een andere aanpak

Andy Matushak
https://notes.andymatuschak.org/zF8xCU4BwXwbmSyp7tmff9i

Een lijstje met backlinks gegenereerd door Dataview (Bases werkt nog niet in Quartz):
#### Links to this note

|Link4|Date|
|---|---|
|[[PKM Mindmap\|PKM Mindmap]]|4 Dec 2025|
|[[Gebruik van Tags\|Gebruik van Tags]]|2 Dec 2025|
|[[dagboek/2023-01-23\|2023-01-23]]|2 Dec 2025|
|[[PR Obsidian Dataview\|PR Obsidian Dataview]]|1 Jan 2023|

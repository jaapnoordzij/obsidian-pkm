---
{"publish":true,"title":"Mindmaps","created":"2025-12-10","modified":"2025-12-16T13:29:23.884+01:00","cssclasses":""}
---

Wanneer ik een probleem van verschillende kanten wil bekijken en onderzoeken begin ik vrijwel altijd met een [Mindmap](https://en.wikipedia.org/wiki/Mind_map). Er zijn veel goede pakketten om Mindmaps te maken en er zijn Plugins in Obsidian voor. Maar eerlijk gezegd gaat mijn voorkeur uit naar (kleur) potlood en papier. Meerstal maak ik een paar schetsen en die vertaal ik dan uiteindelijk in een notitie per element met Wikilinks voor de verbindingen.

Obsidian biedt, naast een aantal plugins, de mogelijkheid om Mindmaps te genereren vanuit de ingebouwde [Mermaid](https://mermaid-js.github.io/) integratie:


```mermaid
mindmap
	id(("PKM"))
		def(definitie)
			[wat is PKM]
			[notetaking with Obsidian]
		str(structuur)
			dg(Digital garden)
			::icon(fas fa-tree)
			mc(Map of Content)
		res(research)
			(Research notes)
			(Concept teksten)
		tec(techniek)
			[Workflow]
			[Files en Vaults]

```

Helaas kan Mermaid (nog) niet Wikilinks opnemen in een mindmap dus in de praktijk is het meestal toch handiger om maar gewoon een de inhoud in tekst met indentatie weer te geven zoals in [[index\|Obsidian praktijktips]]

Of je kunt met Mermaid een "Graph" maken, dan heb je wél clickable links in Obsidian maar Quartz neemt ze niet over op de gegenereerde website :

```mermaid
graph LR

A["PKM"]
R[Research notes]
D[Definitie]
S[Structuur]
T[Techniek]

T1[Workflow in Obsidian]
T2[Files en Vaults]
T3[Apple Shortcuts]

DG[Digital Garden]
M[Mindmaps]

A --> R
A --> D
  D --> D1
A --> S
  S --> M
  S --> DG
A --> T
  T --> T1 
  T --> T3
  T --> T2


class R,D,D1,DG,M,T1,T2,T3 internal-link;
```




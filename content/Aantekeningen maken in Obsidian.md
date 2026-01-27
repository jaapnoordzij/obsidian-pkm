---
publish: true
title: Aantekeningen maken in Obsidian
created: 2025-12-16
cssclasses: ""
---

Aantekeningen maken Obsidian gaat probleemloos en snel.Je moet wel met een paar dingen rekening houden.

## Backups

Je kennisverzameling heeft een hoge waarde. Dus denk even goed na hoe je backups maakt. De makkelijkste en beste manier is een echte backup app zoals Apple Time Machine. 
Ik maakte dagelijks een kopie met `rsync` en dat werkt ook wel prima al maak ik geen incremental backups en heb geen vorige versies.
Tegenwoordig gebruik ik git. Daarmee heb ik een backup en een versie historie al is git daar niet specifiek voor bedoeld. 

## Synchronisatie

Je zult al snel in een situatie komen dat je kennis altijd en overal beschikbaar wilt hebben. Dat betekent dus ook op je telefoon of ipad. Daarvoor moet je een mechaniek hebben dat synchronisatie goed regelt.

Obsidian sync is hiervoor het meest geschikt maar is wel een betaalde dienst.

Synchronisatie iCloud wordt ondersteund maar werkt in mijn ervaring nogal onbetrouwbaar. Af en toe lijkt het alsof alles weg is hoewel dat nooit echt zo was. 

Dropbox, Onedrive worden formeel niet ondersteund al zijn er wel Plugins die dat oppakken.

## Vaults

Uiteindelijk hebben we het over een grote verzameling "platte tekst files" wellicht aangevuld met foto's en pdf's.  Die staan in een "Vault" van Obsidian. Een vault is alleen maar een map op je harde schijf op de computer. 

Obsidian staat toe dat je meerdere vaults maakt maar kent nauwelijks interactie tussen die vaults. Gezien de aard van mijn kennis verzameling geef ik er dan ook de voorkeur aan om alles in één vault te houden. Voor de performance hoef je het niet te laten.

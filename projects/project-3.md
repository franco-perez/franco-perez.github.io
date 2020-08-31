---
layout: project
type: project
image: images/Schaltschrank_portada.jpg
title: " Instationäre Temperaturberechnung im Inneren von Schaltschränken" 
permalink: projects/cotton
# All dates must be YYYY-MM-DD format!
date: 2018-10-22
labels:
  - Python
  - GitHub
  - Grobstrukturmodell

summary: Diese Arbeit stellt ein in Python® entwickeltes Modell zur Berechnung der transienten Temperaturverläufe innerhalb eines Schaltschrankes dar.
---

<img class="ui image" src="../images/Schaltschrank.png">

# Zusammenfassung

Im Betrieb weisen die elektronische Komponente eines Schaltschrankes eine Temperaturerhöhung aufgrund der entstehenden Wärme durch Dissipation von der elektrischen Energie auf. Diese Temperaturerhöhung kann schädlich für den Schaltschrank werden, daher werden diese in der Regel mit Klimatechnik ausgerüstet. Es wurde ein instationäres Modell zur Berechnung der zeitabhängigen Temperaturverläufe innerhalb eines Schaltschrankes entwickelt und in Python® umgesetzt. Das Modell hat zwei Betriebsweise:
1) **_Vorgegebene Kühlleistung_**: Die Kühlleistung des Dachkühlgeräts als eine Funktion der Zeit vorgegeben _Q(t)_
2) **_Regelung des Dachkühlgeräts_**: Die Kühlleistung wird als eine Funktion der Plattentemperatur berechnet. Dabei darf sie weder unterhalb 32,5 _°C_ noch oberhalb 37,5 _°C_ liegen.

# Wichtigste Ergebnisse

Generell lässt sich sagen, dass für den Fall der vorgegebener Kälteleitung, die modellierte Lufttemperatur und die gemessene Luft-temperatur ein ähnliches Verhalten vorzeigen, da die Spitzen der beiden Kurven zum fast selben Zeitpunkt erreicht werden konnten. Dabei ist wichtig festzuhalten, dass die Dauer der Aufheizphasen anhand des Modells gut dargestellt werden konnte (siehe Abb. 1). 


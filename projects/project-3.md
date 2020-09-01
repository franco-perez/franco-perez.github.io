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

<div class="ui medium rounded images">
  <img class="ui image" src="../images/nodes_schaltschrank.png">
  <img class="ui image" src="../images/Schaltschrank.png">
</div>



# Zusammenfassung
___
<br>
Im Betrieb weisen die elektronische Komponente eines Schaltschrankes eine Temperaturerhöhung aufgrund der entstehenden Wärme durch Dissipation von der elektrischen Energie auf. Diese Temperaturerhöhung kann schädlich für den Schaltschrank werden, daher werden diese in der Regel mit Klimatechnik ausgerüstet. Es wurde ein instationäres Modell zur Berechnung der zeitabhängigen Temperaturverläufe innerhalb eines Schaltschrankes entwickelt und in Python® umgesetzt. Das Modell hat zwei Betriebsweise:

1. **_Vorgegebene Kühlleistung_**: Die Kühlleistung des Dachkühlgeräts als eine Funktion der Zeit vorgegeben _Q(t)_.
<br>
<br>
2. **_Geregelte Kühlleistung des Dachkühlgeräts_**: Die Kühlleistung wird als eine Funktion der Plattentemperatur berechnet. Dabei darf sie weder unterhalb _32,5 °C_ noch oberhalb _37,5 °C_ liegen.
<br>
<br>

# Wichtigste Ergebnisse
___
### 1. Vorgegebene Kühlleistung
<img class="ui large rounded image" src="../images/comparisson_temperatures.png"> 

_Vergleich gemessene (Grün) und berechnete Lufttemperaturen (Blau)_
<br>
<br>
Generell lässt sich sagen, dass für den Fall der vorgegebener Kälteleitung, die modellierte Lufttemperatur und die gemessene Luft-temperatur ein ähnliches Verhalten vorzeigen, da die Spitzen der beiden Kurven zum fast selben Zeitpunkt erreicht werden konnten. Dabei ist wichtig festzuhalten, dass die Dauer der Aufheizphasen anhand des Modells gut dargestellt werden konnte.
<br>
<br>
Die Abweichungen zwischen den gemessenen und berechneten Werten aufgetreten sind von verschiedenen Faktoren abhängig u.a. durch die Auswahl der Lösungsverfahren, die am Modell getroffene Annahmen, der Stoffauswahl der Schaltschrankbestandteile sowie die Geometrie-modellierung des Schaltschrankes und die Wärmekapazitäten der Knotenelemente.
<br>
<br>
### 2. Geregelte Kühlleistung des Dachkühlgeräts
<img class="ui large rounded image" src="../images/controled_temperature.png">
 

_Geregelter zeitlicher Verlauf der Plattentemperatur_
<br>
<br>

Die modellierte Temperatur bleibt innerhalb des angegebenen gewünschten Betriebsintervalls  (_32.5 °C < Plattentemperatur < 37.5 °C_). Dabei ist es erwähnenswert, dass der Temperaturbereich leicht überschritten wird, was auf den Zeitvektor zurückzuführen ist, welcher durch den Solver erzeugt wird.

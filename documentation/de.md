<!-- ELUCENIA technical documentation · driving-pressure · de · no clinical/professional/rights approval -->

# Driving Pressure und statische Compliance

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/driving-pressure)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Atemzugvolumen

`vt`

mL · Bereich: 100–1500

### Plateaudruck (inspiratorische Pause)

`pplat`

cmH₂O · Bereich: 5–60

### Gesamt-PEEP

`peep`

cmH₂O · Bereich: 0–30

### Prädiziertes Körpergewicht

`pbw`

kg · optional · Bereich: 20–120

## Fassung der Methode

ΔP=Pplat−PEEP; Cstat=VT/ΔP; Amato 2015 bei passiver Beatmung

## Dokumentierte Formel

Driving Pressure (ΔP) = Plateaudruck − PEEP.

Statische Compliance = Atemzugvolumen ÷ ΔP (mL/cmH₂O).

## Grenzen und Population

Die Analyse von Amato 2015 untersuchte 3562 ARDS-Patienten aus neun früheren Studien bei Beatmung ohne aktive Atmung. Driving Pressure wurde als VT/CRS und als mit dem Überleben assoziierte Variable analysiert; diese Assoziation begründet allein weder einen universellen Schwellenwert noch eine durch die Berechnung gesteuerte therapeutische Intervention. Messtechnik und Beatmungsbedingungen müssen geprüft werden.

## Referenzen

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Driving pressure bis 15 cmH₂O

| Ergebnisdetails | |
| --- | --- |
| Statische Compliance | 28,0 mL/cmH₂O |


### 2

Driving pressure über 15 cmH₂O: mit höherer Mortalität beim ARDS assoziiert

| Ergebnisdetails | |
| --- | --- |
| Statische Compliance | 20,5 mL/cmH₂O |


### 3

Driving pressure bis 15 cmH₂O

| Ergebnisdetails | |
| --- | --- |
| Statische Compliance | 38,5 mL/cmH₂O |
| Atemzugvolumen | 7,1 mL/kg des vorhergesagten Körpergewichts |


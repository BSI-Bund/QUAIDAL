---
Name: QM-04 Genauigkeit
Title: QM-04 Genauigkeit
TitleGer: QM-04 Genauigkeit
shortdesc: Verhältnis korrekter Vorhersagen zur Gesamtzahl der Beobachtungen
tags:
  - Qualitätsmetrik
ID:
  - QM-04
ListMetricID: 
ListMeasureID:
  - "'MA-27'"
MID: "4"
type:
  - metric
CodeEx: true
share: true
lcstep: post
---
## QM-04 Genauigkeit

### Beschreibung

Die Accuracy, oder Genauigkeit, ist eine Metrik zur Bewertung von maschinellen Lernmodellen, besonders bei Klassifizierungsproblemen. Sie gibt an, wie gut ein Modell die Daten klassifiziert, indem sie das Verhältnis von korrekt vorhergesagten Beobachtungen zur Gesamtzahl der Beobachtungen misst.

Obwohl die Accuracy eine sehr intuitive und einfache Metrik ist, hat sie ihre Grenzen, besonders bei unausgewogenen Datensätzen (d.h., wenn einige Klassen viel häufiger als andere sind). In solchen Fällen können andere Metriken wie Precision, Recall (Sensitivität) und F1-Score ein vollständigeres Bild der Leistung des Modells bieten.

### Methode

- Zähle die richtigen Vorhersagen: Vergleiche für jede Vorhersage, ob sie mit dem tatsächlichen Ergebnis übereinstimmt. Wenn sie richtig ist, zähle sie als "korrekt". 
- Zähle die Gesamtanzahl der Vorhersagen: Bestimme, wie viele Vorhersagen insgesamt gemacht wurden, egal ob richtig oder falsch. 
- Vergleiche die Richtigen mit den Gesamten: Teile die Anzahl der richtigen Vorhersagen durch die Gesamtanzahl der Vorhersagen. Das Ergebnis gibt dir eine Zahl, die zwischen 0 und 1 liegt, wobei 1 die perfekte Accuracy ist.



### Pythoncode für "Accuracy"
| RefID | Verweis               |
| ----- | --------------------- |
| 4     | QM-04_Accuracy_python |




### Referenzen
| RefID | Verweis                                                                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                  |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 126   |  Statista - das Statistik-Portal: Statistiken, Marktdaten & Studien                                                                   | Statista ist eine Datenplattform, die Statistiken und Berichte aus verschiedenen Branchen und Märkten bereitstellt. Sie bietet Umfragen, Prognosen und Analysen zu Themen wie Wirtschaft, Gesellschaft und Technologie für Unternehmen, Forscher und Medien. |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance  | Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                                                                                                                 |

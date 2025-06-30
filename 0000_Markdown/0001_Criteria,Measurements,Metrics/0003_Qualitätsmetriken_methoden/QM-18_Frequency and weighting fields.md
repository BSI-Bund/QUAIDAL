---
Name: QM-18 Häufigkeits- und Gewichtungsfeldern
Title: QM-18 Häufigkeits- und Gewichtungsfeldern
TitleGer: QM-18 Häufigkeits- und Gewichtungsfeldern
shortdesc: Felder dienen der manuellen Gewichtung von Merkmalen oder Merkmalsgruppen
tags:
  - Qualitätsmetrik
ID:
  - QM-18
ListMetricID: 
ListMeasureID:
  - "'MA-10'"
MID: "102"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-18 Häufigkeits- und Gewichtungsfeldern

### Beschreibung

Häufigkeits- und Gewichtungsfelder werden in der Datenanalyse genutzt, um Datensätzen je nach Bedeutung unterschiedlich starkes Gewicht zu verleihen. Häufigkeitsfelder geben an, wie oft ein Datensatz in einem Trainingsset vorkommt (nur positive ganze Zahlen). Gewichtungsfelder bestimmen die Bedeutung eines Datensatzes (positive Werte, keine Ganzzahlen erforderlich). Beim Modelltraining sind diese Felder wichtig, aber beim Scoring und der Modellbewertung werden sie ignoriert, um einen direkten Vergleich zwischen Modellen zu ermöglichen. Eine präzise Bewertung erfolgt mit Testdaten, die die Population ohne Gewichtung genau repräsentieren.

### Methoden

#### Häufigkeitsfelder

- Quantifizierung der Erscheinung: Häufigkeitsfelder halten fest, wie oft ein bestimmtes Ereignis oder ein Merkmal in einem Datensatz auftritt.
- Klassenverteilung: In einem klassenbasierten Kontext zeigen sie die Verteilung der verschiedenen Klassen an und können bei Unausgewogenheit aufzeigen, welche Klassen über- oder unterrepräsentiert sind.
- Einfluss auf Modellleistung: Die Informationen aus den Häufigkeitsfeldern sind kritisch für die Modellleistung, da Modelle, die auf unausgewogenen Daten trainiert werden, eine Verzerrung aufweisen können.


#### Gewichtungsfelder

- Anpassung der Bedeutung: Gewichtungsfelder erlauben die Zuweisung eines Gewichts oder einer Wichtigkeit zu einzelnen Beobachtungen oder Merkmalen im Trainingsdatensatz.
- Korrektur von Unausgewogenheiten: Durch Anwendung unterschiedlicher Gewichte können Ungleichheiten in den Trainingsdaten ausgeglichen werden, sodass das Modell nicht zugunsten der überrepräsentierten Klassen verzerrt wird. 
- Fokus auf spezifische Daten: Gewichtungsfelder können genutzt werden, um dem Modell beizubringen, bestimmte Muster oder Eigenschaften zu priorisieren, die als wichtiger angesehen werden, basierend auf dem Anwendungsfall. 
- Feinabstimmung des Trainings: Sie ermöglichen eine Feinabstimmung des Lernprozesses, indem sie den Einfluss bestimmter Datenpunkte auf die Aktualisierung der Modellparameter während des Trainings erhöhen oder verringern.
- Kontextabhängigkeit: Die Gewichte können kontextabhängig sein, d.h., sie können auf der Grundlage externer Kriterien wie Expertenwissen, zeitlicher Relevanz oder spezifischen Geschäftsregeln festgelegt werden.
- Dynamische Anpassung: Gewichtungen können dynamisch angepasst werden, um im Laufe der Zeit Änderungen in den Datenquellen oder im zugrundeliegenden Problem zu reflektieren.
- Risiko von Overfitting: Unangemessen hohe Gewichte können zu Overfitting führen, insbesondere wenn bestimmte Datenpunkte zu stark hervorgehoben werden.
- Implementierung: In den meisten Fällen werden die Gewichte direkt in den Trainingsalgorithmen über Parameter berücksichtigt, die bestimmen, wie stark jede Beobachtung in die Loss-Funktion eingeht.


### Beispiele 

#### Beispiel 1 - Häufigkeitstabelle

Notenspiegel einer Klasse

|Note|Häufigkeit (f)|
|---|---|
|5|3|
|6|3|
|7|3|
|8|5|
|9|3|
|10|3|



#### Beispiel 2 - Gewichtungsfeld

Angenommen, wir haben eine Umfrage durchgeführt, in der Menschen nach ihrer Zufriedenheit mit einem neuen Produkt gefragt wurden. Die Antworten wurden auf einer Skala von 1 bis 5 gesammelt:

- **1** = Sehr unzufrieden
- **2** = Unzufrieden
- **3** = Neutral
- **4** = Zufrieden
- **5** = Sehr zufrieden

Zusätzlich haben wir entschieden, dass Antworten von "Sehr zufrieden" (5) und "Sehr unzufrieden" (1) doppelt so viel Gewicht haben sollten wie die anderen, da extreme Meinungen wichtiger sind.

Hier sind die gesammelten Antworten von 20 Teilnehmern:  
1, 2, 3, 5, 4, 3, 2, 4, 5, 1, 3, 4, 2, 1, 5, 4, 5, 3, 2, 4

#### Gewichtungsfeld:

|Bewertung|Häufigkeit (f)|Gewichtung (w)|Gewichtete Häufigkeit (f * w)|
|---|---|---|---|
|1|3|2|6|
|2|4|1|4|
|3|4|1|4|
|4|5|1|5|
|5|4|2|8|

Die Gewichtete Häufigkeit zeigt die Gesamtbedeutung oder den Einfluss jeder Kategorie auf die Gesamtzufriedenheit der Umfrageteilnehmer unter Berücksichtigung der festgelegten Gewichtungen.

### Referenzen
| RefID | Verweis                                                                 | Kurzbeschr.                                                                                                                                                                                                                                                                                          |
| ----- | ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 104   |  Verwenden von Häufigkeits- und Gewichtungsfeldern - IBM Dokumentation  | Die Seite erklärt, wie Häufigkeits- und Gewichtungsfelder in SPSS Modeler verwendet werden, um bestimmten Datensätzen mehr Bedeutung beim Modelltraining zu verleihen, wobei Häufigkeitsfelder identische Fälle repräsentieren und Gewichtungsfelder die Relevanz einzelner Datensätze beeinflussen. |

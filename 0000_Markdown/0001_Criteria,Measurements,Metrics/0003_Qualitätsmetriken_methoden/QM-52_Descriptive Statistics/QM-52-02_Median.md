---
Name: QM-52-02_Median
Title: QM-52-02 Median
TitleGer: QM-52-02 Median
shortdesc: mittlerer Wert in einer sortierten Liste von Daten
tags:
  - Qualitätsmetrik
  - "#ML-Desc-Basics"
  - ML-Desc-Basics
ID:
  - QM-52-02
ListMetricID: 
ListMeasureID:
  - "'MA-9'"
  - "'QM-52'"
  - "'MA-09'"
MID: "80"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-52-02 Median

### Beschreibung

Der Median ist der mittlere Wert in einer sortierten Liste von Daten. Im Gegensatz zum Mittelwert ist der Median extremwertresistent.

### Methode

- Ungerade Anzahl von Datenpunkten (n): Median = Beobachtung an Position $(n+1)/2$.
- Gerade Anzahl von Datenpunkten (n): Median = (Beobachtung an Position $n/2$ + Beobachtung an Position $((n/2 + 1)) / 2$.


### Sourcecode "Median"
| RefID | Verweis                |
| ----- | ---------------------- |
| 55    | QM-52-02_Median_python |



### Referenzen
| RefID | Verweis                                                     | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 217   |  Introduction to Probability and Statistics \| Mathematics  | Der MIT-Kurs Introduction to Probability and Statistics bietet eine grundlegende Einführung in Wahrscheinlichkeitstheorie und Statistik, behandelt Themen wie Kombinatorik, Zufallsvariablen, Wahrscheinlichkeitsverteilungen, Bayessche Inferenz, Hypothesentests, Konfidenzintervalle und lineare Regression und ermöglicht durch interaktive Materialien in der Open Learning Library eine praxisorientierte und flexible Lernerfahrung. |



---
Name: QM-42 QQ-Diagramm
Title: QM-42 QQ-Diagramm
TitleGer: QM-42 QQ-Diagramm
shortdesc: Grafische Vergleich von Quantilen zweier statistischer Variablen.
tags:
  - Qualitätsmetrik
  - ChartTypes
ID:
  - QM-42
ListMetricID: 
ListMeasureID:
  - "'MA-14'"
MID: 
type:
  - method
ListCritID: 
lcstep: pre
CodeEx: true
share: true
---
## QM-42 QQ-Diagramm

### Beschreibung

Ein Quantil-Quantil-Diagramm, kurz Q-Q-Diagramm (englisch quantile-quantile plot, kurz Q-Q-Plot) ist ein exploratives, grafisches Werkzeug, in dem die Quantile zweier statistischer Variablen gegeneinander in einem parametrischen Plot aufgetragen werden, um ihre Verteilungen zu vergleichen.

Ein P-P-Diagramm bzw. Probability-Probability-Plot ist ein exploratives, grafisches Werkzeug, in dem die Verteilungsfunktionen zweier statistischer Variablen gegeneinander abgetragen werden, um ihre Verteilungen zu vergleichen.

### Methode

- Daten sammeln und vorbereiten:
    - Erfassen Sie Ihre Daten und sortieren Sie sie in aufsteigender Reihenfolge.
    - Entfernen Sie fehlende oder fehlerhafte Werte.

- Empirische Quantile bestimmen:
    - Berechnen Sie die Quantile Ihrer empirischen Daten. Dies entspricht oft der einfachen Reihenfolge der Datenpunkte in Ihrer sortierten Liste.

- Theoretische Quantile berechnen:
    - Wenn Sie mit einer theoretischen Verteilung vergleichen (z.B. Normalverteilung), berechnen Sie die entsprechenden theoretischen Quantile.
    - Verwenden Sie die inverse kumulative Verteilungsfunktion (auch Quantilfunktion genannt) der theoretischen Verteilung.

- Diagramm erstellen:
    - Zeichnen Sie ein Streudiagramm mit den theoretischen Quantilen auf der x-Achse und den empirischen Quantilen auf der y-Achse.
    - Fügen Sie optional eine Referenzlinie hinzu (eine 45-Grad-Linie), um Abweichungen leichter zu erkennen.


### Sourcecode "QQ-Diagramm"

| RefID | Verweis                  |
| ----- | ------------------------ |
| 35    | QM-42_QQ-Diagramm_python |



### Referenzen

| RefID | Verweis                                                     | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 217   |  Introduction to Probability and Statistics \| Mathematics  | Der MIT-Kurs Introduction to Probability and Statistics bietet eine grundlegende Einführung in Wahrscheinlichkeitstheorie und Statistik, behandelt Themen wie Kombinatorik, Zufallsvariablen, Wahrscheinlichkeitsverteilungen, Bayessche Inferenz, Hypothesentests, Konfidenzintervalle und lineare Regression und ermöglicht durch interaktive Materialien in der Open Learning Library eine praxisorientierte und flexible Lernerfahrung. |



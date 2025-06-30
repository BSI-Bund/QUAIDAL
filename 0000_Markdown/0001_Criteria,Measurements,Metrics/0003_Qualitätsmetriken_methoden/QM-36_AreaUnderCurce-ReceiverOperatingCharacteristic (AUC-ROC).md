---
Name: QM-36_AreaUnderCurce (AUC)
Title: QM-36 Area Under Curce (AUC)
TitleGer: QM-36 Area Under Curce (AUC)
shortdesc: Messung der Modellperformance; Bewertung der Klassifizierungsgenauigkeit
tags:
  - Qualitätsmetrik
ID:
  - QM-36
ListMetricID: 
ListMeasureID:
  - "'MA-14'"
MID: "45"
lcstep: post
CodeEx: true
share: true
type:
  - method
---
## QM-36 AreaUnderCurve (AUC)

### Beschreibung

Die Area Under Curve (AUC), speziell im Kontext von Receiver Operating Characteristic (ROC) Kurven, ist eine Metrik zur Bewertung der Leistungsfähigkeit von Klassifizierungsmodellen. Die ROC-Kurve stellt die True Positive Rate (TPR) oder Sensitivität gegen die False Positive Rate (FPR) oder 1-Spezifität für verschiedene Schwellenwerte dar. Die AUC misst die gesamte zwei dimensionale Fläche unter der gesamten ROC-Kurve von (0,0) bis (1,1) und bietet damit ein Maß für die Gesamtleistung des Modells über alle Klassifizierungsschwellen hinweg. Eine AUC von 1 bedeutet eine perfekte Klassifizierung, während eine AUC von 0,5 auf ein Modell hindeutet, das nicht besser als zufälliges Raten ist. Um die AUC zu berechnen, gibt es verschiedene methodische Ansätze.

### Methode

#### Numerische Integration

Die einfachste Methode ist die numerische Integration, bei der die Fläche unter der ROC-Kurve durch Aufsummieren der Flächen unter jedem Segment der Kurve approximiert wird. Dies kann durch einfache Methoden wie die Trapezregel erfolgen, bei der die ROC-Kurve in eine Serie von Trapezen unterteilt wird, deren individuelle Flächen dann summiert werden.

#### Verwendung einer Softwarebibliothek

In der Praxis wird die AUC häufig mit statistischer Software oder Bibliotheken für maschinelles Lernen berechnet, die spezialisierte Funktionen für diese Aufgabe bieten. Beispiele solcher Bibliotheken sind Scikit-learn in Python, ROCR in R, und viele andere:

#### Analytische Lösungen

Für bestimmte Arten von Modellen oder unter bestimmten Annahmen kann die AUC auch analytisch berechnet werden, basierend auf den Eigenschaften des Modells und der Verteilung der Daten. Diese Ansätze sind jedoch spezifisch für das Modell und nicht allgemein anwendbar.


### Sourcecode "AreaUnderCurce-ReceiverOperatingCharacteristic (AUC-ROC)"

| RefID | Verweis                                                             |
| ----- | ------------------------------------------------------------------- |
| 29    | QM-36_AreaUnderCurce-ReceiverOperatingCharacteristic AUC-ROC_python |



### Referenzen

| RefID | Verweis                 | Kurzbeschr.                                                                                                                                                                                                                                 |
| ----- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 285   |  ROC-Kurve – Wikipedia  | Die ROC-Kurve ist ein Diagramm, das die Sensitivität eines binären Klassifikationsmodells gegenüber der Falsch-Positiv-Rate für verschiedene Schwellenwerte darstellt und dessen Gesamtgüte über die Fläche unter der Kurve (AUC) bewertet. |


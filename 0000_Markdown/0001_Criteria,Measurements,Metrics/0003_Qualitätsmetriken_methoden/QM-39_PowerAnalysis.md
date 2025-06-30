---
Name: QM-39 Power Analyse
Title: QM-39 Power Analyse
TitleGer: QM-39 Power Analyse
shortdesc: Poweranalyse bestimmt benötigte Stichprobengröße für statistisch signifikanten Effekt.
tags:
  - Qualitätsmetrik
ID:
  - QM-39
ListMetricID: 
ListMeasureID:
  - "'MA-11'"
  - "'MA-10'"
MID: "48"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-39 Power-Analyse

### Beschreibung

Vor der Datenerhebung kann eine Poweranalyse durchgeführt werden, um die erforderliche Stichprobengröße zu bestimmen, die notwendig ist, um einen statistisch signifikanten Effekt mit einer bestimmten Wahrscheinlichkeit (Power) zu entdecken. Die Power hängt von der Effektgröße, dem Signifikanzniveau (üblicherweise 0,05) und der Variabilität in der Population ab. Das bedeutet zugleich, dass wir bereits ein grundlegendes Wissen über die zu nutzende Gesamtpopulation besitzen müssen um daraus eine Information zur Stichprobe ableiten zu können. 

### Methode 

- **Effektgröße festlegen**: Zunächst muss die minimale Effektgröße definiert werden, die das Modell erkennen soll. Dies hängt von der spezifischen Anwendung und den Zielen des Projekts ab. Ein größerer Effekt erfordert weniger Daten, um erkannt zu werden, während ein kleinerer Effekt eine größere Stichprobe erfordert.
- **Signifikanzniveau bestimmen**: Üblicherweise wird ein Signifikanzniveau von 0,05 (5%) gewählt, kann aber je nach Anforderungen angepasst werden.
- **Gewünschte statistische Power festlegen**: Typischerweise wird eine Power von 0,8 (80%) angestrebt, was bedeutet, dass das Modell mit 80%iger Wahrscheinlichkeit einen tatsächlich vorhandenen Effekt erkennen kann.
- **Varianz der Daten schätzen**: Die Varianz der Zielvariable in der Gesamtpopulation muss geschätzt oder aus Vorstudien ermittelt werden.
- **Berechnung der Stichprobengröße**: Mit diesen Parametern wird die erforderliche Stichprobengröße berechnet. Hierfür können spezielle Software-Tools oder statistische Formeln verwendet werden.
- **Anpassung für maschinelles Lernen**: Für ML-Anwendungen sollte die berechnete Stichprobengröße möglicherweise erhöht werden, um komplexere Muster und Zusammenhänge zu erfassen.



### Pythoncode "Power-Analyse"
| RefID | Verweis                    |
| ----- | -------------------------- |
| 32    | QM-39_PowerAnalysis_python |




### Referenzen
| RefID | Verweis                                                  | Kurzbeschr.                                                                                                                                                                                                         |
| ----- | -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 294   |  Statistical power analysis for the behavioral sciences  | Cohens Standardwerk erklärt die Zusammenhänge zwischen Effektgröße, Signifikanzniveau, Stichprobengröße und Power und bietet eine fundierte Grundlage für die statistisch abgesicherte Planung empirischer Studien. |



---
Name: QM-10-3_RobustPrincipalComponentAnalysis
Title: QM-10-3_RobustPrincipalComponentAnalysis
TitleGer: QM-10-3 RobustPrincipalComponentAnalysis
shortdesc: Robust Principal Component Analysis (RPCA) erweitert die klassische PCA, um robuster gegenüber Ausreißern und Störungen zu sein.
tags:
  - Qualitätsmetrik
ID:
  - QM-10-3
ListMetricID: 
ListMeasureID:
  - "'QB-0'"
  - "'MA-08'"
  - "'QB-12'"
  - "'MA-12'"
MID: 
type:
  - metrik
  - method
share: true
CodeEx: true
lcstep: pre
---
## QM-10-3 Robust Principal Component Analysis

### Beschreibung
Robust Principal Component Analysis (RPCA) erweitert die klassische PCA, um robuster gegenüber Ausreißern und Störungen zu sein. Während PCA Daten in Hauptkomponenten zerlegt und anfällig für Verzerrungen ist, trennt RPCA die Datenmatrix in eine niedrigrangige und eine spärliche Komponente, was zu präziseren Ergebnissen bei verrauschten oder fehlerhaften Daten führt und besonders in der Bild- und Signalverarbeitung nützlich ist.


### Sourcecode "RobustPrincipalComponentAnalysis"
| RefID | Verweis                                         |
| ----- | ----------------------------------------------- |
| 98    | QM-10-3_RobustPrincipalComponentAnalysis_python |



### Referenzen
| RefID | Verweis                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                         |
| ----- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 264   |  Robust Principal Component Analysis: Two Analyses in One  | Home-Telematik ist ein wachsendes Feld in der Versicherungsbranche, bei dem Sensoren in Häusern Daten über deren Nutzung liefern, um zukünftige Versicherungsschäden besser vorherzusagen. Diese hochfrequenten, hochdimensionalen Daten erfordern jedoch eine Vorverarbeitung, um Ausreißer zu identifizieren und die Anzahl der Prädiktorvariablen zu reduzieren. |

---
Name: QM-56-6 Batch Normalization
Title: QM-56-6 Batch Normalization
TitleGer: QM-56-6 Batch Normalization
shortdesc: Die Batch-Normalisierung stabilisiert die Aktivierungen in neuronalen Netzwerken, indem sie für jede Schicht den Mittelwert und die Standardabweichung der Aktivierungen über einen Mini-Batch berechnet.
tags:
  - Qualitätsmetrik
  - Normalization
ID:
  - QM-56-6
ListMetricID: 
ListMeasureID:
  - "'MA-33'"
lcstep: post
CodeEx: true
share: true
type:
  - method
---
## QM-56-6 Batch Normalization

### Beschreibung

Batch-Normalisierung normalisiert die Eingaben jeder Schicht in einem neuronalen Netz, indem sie den Mittelwert und die Standardabweichung der Aktivierungen über einen Mini-Batch berechnet. Dies führt zu einer stabileren Verteilung der Aktivierungen in verschiedenen Schichten.

Beim Einsatz von Regularisierungsmethoden ist es unerlässlich, genau auf mögliche Verzerrungen (Biases) zu achten, die sich unbemerkt durch die Transformation in die Daten einschleichen können.
### Methode

- Berechnung des Mittelwerts und der Varianz für jeden Mini-Batch
- Normalisierung der Eingaben
- Skalierung und Verschiebung der normalisierten Werte

### Sourcecode "Batch Normalization"
| RefID | Verweis                            | Inhalt                         |
| ----- | ---------------------------------- | ------------------------------ |
| 77    | QM-56-6_Batch Normalization_python | Batch Normalisierung in Python |


### Referenzen
| RefID | Verweis                                                                                        | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ----- | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 79    |  Batch Normalization: Accelerating Deep Network Training by Reducing Internal Covariate Shift  | Die Batch-Normalisierung begegnet der internen Kovariatenverschiebung, indem sie die Eingaben der Schichten in jedem Trainings-Mini-Batch normalisiert. Dies ermöglicht höhere Lernraten, verringert die Notwendigkeit einer sorgfältigen Initialisierung, wirkt als Regularisator und verbessert signifikant die Trainingsgeschwindigkeit und Genauigkeit. Sie erreicht Spitzenergebnisse bei der ImageNet-Klassifizierung mit weniger Schritten und übertrifft die menschliche Genauigkeit. |



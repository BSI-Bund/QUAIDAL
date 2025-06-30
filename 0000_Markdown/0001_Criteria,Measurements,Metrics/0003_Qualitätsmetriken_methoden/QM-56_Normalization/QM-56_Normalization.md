---
Name: QM-56 Normalisierung
Title: QM-56 Normalisierung
TitleGer: QM-56 Normalisierung
shortdesc: Die Normalisierung von Daten ist der Prozess, bei dem Daten so transformiert werden, dass sie einem bestimmten Standard oder statistischen Eigenschaften entsprechen—wie Werte zwischen 0 und 1 oder einem Mittelwert von 0—um Konsistenz und Vergleichbarkeit in der Datenverarbeitung und -analyse sicherzustellen.
tags:
  - Qualitätsmetrik
ID:
  - QM-56
ListMetricID: 
ListMeasureID:
  - "'MA-23'"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-56 Normalisierung

### Beschreibung

Die Normalisierung von Daten bezieht sich auf den Prozess, Daten so zu transformieren, dass sie einem bestimmten Standard oder Format entsprechen oder aber einer bestimmten statistischen Eigenschaft entsprechen, z.B. liegen alle Werte zwischen 0 und 1 und/oder der Mittelwert beträgt 0. Dies ist besonders wichtig in der Datenverarbeitung und Analyse, um sicherzustellen, dass die Daten konsistent und vergleichbar sind. 

### Normalisierungsmethoden

| Tool                                  | Kurzbeschr.                                                                                                                                                                                                                                                          |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-56-3 L1-Normalization              | ist eine Methode, bei der die Werte eines Vektors so skaliert werden, dass die Summe der absoluten Werte aller Elemente 1 beträgt                                                                                                                                    |
| QM-56-1 Min/Max Skalierung            | Skalierung der Dateninhalt anhand des minimalen und maximalen Wertes.                                                                                                                                                                                                |
| QM-56-2 Z-Score Normalization         | Die Z-Score-Normalisierung transformiert Daten zu einem Mittelwert von 0 und einer Standardabweichung von 1.                                                                                                                                                         |
| QM-56-4 Logarithmische Transformation | Die logarithmische Transformation ist eine Technik zur Datenvorverarbeitung, die verwendet wird, um Daten zu normalisieren, Varianzen zu stabilisieren, den Einfluss von Ausreißern zu reduzieren und exponentielle Beziehungen in lineare zu überführen.            |
| QM-56-5 L2-Normalisierung             | Die L2-Normalisierung skaliert Vektoren auf eine euklidische Norm von 1 und betont größere Abweichungen stärker als die L1-Normalisierung, was sie besonders für Anwendungen geeignet macht, bei denen die geometrische Beziehung zwischen Datenpunkten wichtig ist. |
| QM-56-6 Batch Normalization           | Die Batch-Normalisierung stabilisiert die Aktivierungen in neuronalen Netzwerken, indem sie für jede Schicht den Mittelwert und die Standardabweichung der Aktivierungen über einen Mini-Batch berechnet.                                                            |


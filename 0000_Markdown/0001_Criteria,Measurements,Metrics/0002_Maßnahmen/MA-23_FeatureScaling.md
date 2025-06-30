---
Name: MA-23 Merkmalsskalierung
Title: MA-23 Merkmalsskalierung
TitleGer: MA-23 Merkmalsskalierung
shortdesc: Feature Scaling passt die Merkmale eines Datensatzes an einen einheitlichen Bereich an, um Unterschiede in den Skalierungen zu reduzieren und sicherzustellen, dass maschinelle Lernalgorithmen effizienter arbeiten und genauere Vorhersagen liefern können.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-23
ListMetricID: 
ListMeasureID:
  - "'QB-12'"
  - "'QB-13'"
  - "'QB-06'"
share: true
---
## MA-23 Merkmalsskalierung

### Beschreibung

Feature Scaling ist eine Methode der Datenvorverarbeitung, bei der die Merkmale (Features) eines Datensatzes in einen einheitlichen Bereich gebracht werden, um die Unterschiede in den Skalierungen der verschiedenen Merkmale zu reduzieren. Dies ist besonders wichtig in maschinellen Lernalgorithmen, die auf Abständen basieren, wie z. B. bei K-Nearest Neighbors oder beim Gradient Descent in linearen Modellen, wo unterschiedlich skalierte Features zu unerwünschten Ergebnissen führen können.

Feature Scaling ist entscheidend, weil viele maschinelle Lernmodelle und Algorithmen empfindlich auf die Größenordnung der Features reagieren. Ohne Feature Scaling könnten Features mit größeren Werten die Algorithmen dominieren und die Vorhersagegenauigkeit verringern. Indem alle Features auf eine ähnliche Skala gebracht werden, kann der Algorithmus effizienter arbeiten und bessere Ergebnisse liefern.

### Beispiele 

#### Beispiel 1 - Notwendigkeit für K-Nearest Neighbors (KNN): 

- Berechnet Entfernungen zwischen Datenpunkten. Wenn die Skalen der verschiedenen Features in verschiedenen Größenordnungen liegen, wird die Berechnung ohne Skalierung von den Features mit großen Skalen dominiert.


#### Beispiel 2 - Notwendigkeit für Gradient Descent (ML-Trainingsprozess)

- Große Unterschiede in der Skalierung der Features können beim Training von KI-Modellen zu einer langsamen oder gar nicht konvergierenden Optimierung führen.


### Metriken & Methoden

| ID                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                           |
| ------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-10 Dimension Reduction             | hochdimensionale Trainingsdaten werden handhabbarer und interpretierbarer                                                                                                                                                                                                                                             |
| QM-10-1_PrincipalComponentAnalysis    | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                                                                                                                                                                                                 |
| QM-10-2_Clustergraph Analysis         | Ein Verfahren zur Darstellung globaler Beziehungen zwischen Datenclustern                                                                                                                                                                                                                                             |
| QM-56 Normalisierung                  | Die Normalisierung von Daten ist der Prozess, bei dem Daten so transformiert werden, dass sie einem bestimmten Standard oder statistischen Eigenschaften entsprechen—wie Werte zwischen 0 und 1 oder einem Mittelwert von 0—um Konsistenz und Vergleichbarkeit in der Datenverarbeitung und -analyse sicherzustellen. |
| QM-56-1 Min/Max Skalierung            | Skalierung der Dateninhalt anhand des minimalen und maximalen Wertes.                                                                                                                                                                                                                                                 |
| QM-56-2 Z-Score Normalization         | Die Z-Score-Normalisierung transformiert Daten zu einem Mittelwert von 0 und einer Standardabweichung von 1.                                                                                                                                                                                                          |
| QM-56-3 L1-Normalization              | ist eine Methode, bei der die Werte eines Vektors so skaliert werden, dass die Summe der absoluten Werte aller Elemente 1 beträgt                                                                                                                                                                                     |
| QM-56-4 Logarithmische Transformation | Die logarithmische Transformation ist eine Technik zur Datenvorverarbeitung, die verwendet wird, um Daten zu normalisieren, Varianzen zu stabilisieren, den Einfluss von Ausreißern zu reduzieren und exponentielle Beziehungen in lineare zu überführen.                                                             |
| QM-56-5 L2-Normalisierung             | Die L2-Normalisierung skaliert Vektoren auf eine euklidische Norm von 1 und betont größere Abweichungen stärker als die L1-Normalisierung, was sie besonders für Anwendungen geeignet macht, bei denen die geometrische Beziehung zwischen Datenpunkten wichtig ist.                                                  |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                           | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 89    |  Feature Engineering and Selection: A Practical Approach for Predictive Models: by Max Kuhn and Kjell Johnson. Boca Raton, FL: Chapman & Hall/CRC Press, 2019, xv + 297 pp., $79.95(H), ISBN: 978-1-13-807922-9.  | Der Prozess der Entwicklung prädiktiver Modelle umfasst viele Phasen. Die meisten Ressourcen konzentrieren sich auf Modellierungsalgorithmen, vernachlässigen jedoch andere entscheidende Aspekte des Prozesses. Dieses Buch beschreibt Techniken zur optimalen Darstellung von Prädiktoren für die Modellierung und zur Auswahl der besten Teilmenge von Prädiktoren, um die Modellleistung zu verbessern. |
| 157   |  It Is All about Data: A Survey on the Effects of Data on Adversarial Robustness                                                                                                                                  | Adversarial examples sind absichtlich gestaltete Eingaben, die maschinelle Lernmodelle verwirren, und dieses Survey untersucht, wie Eigenschaften von Trainingsdaten die Anfälligkeit für solche Angriffe beeinflussen sowie Methoden zur Verbesserung der adversarialen Robustheit durch verbesserte Datenrepräsentation und Lernverfahren.                                                                |

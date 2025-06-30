---
Name: MA-10_ManualWeights
Title: MA-10 ManualWeights
TitleGer: MA-10 Gewichtung der Daten
shortdesc: Manuelle Gewichtung reduziert Bias und verbessert Generalisierung.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-10
ListMetricID: 
ListMeasureID:
  - "'QB-14'"
  - "'QB-04'"
  - "'QB-03'"
  - "'QB-06'"
share: true
---
## MA-10 Gewichtung der Daten

### Beschreibung

Die Daten - genauer die Features des Modells - werden manuell gewichtet, um eine angemessene Gewichtung sicherzustellen. Manuelle Gewichtung dient zur Reduktion des Bias, einer Verbesserung der Modellleistung und kann bei der Anpassung an spezifische Anforderungen genutzt werden. Sie steigert auch die Generalisierung der Modelle. 

Die Neugewichtung eines Datensatzes ist ein komplexes Unterfangen, das je nach Anwendungsfall unterschiedliche Metriken und Maßnahmen vorsehen kann. 
### Metriken & Methoden
| Metric                                          | Kurzbeschr.                                                                                                                                                          |
| ----------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-10-1_PrincipalComponentAnalysis              | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                                                |
| QM-18 Häufigkeits- und Gewichtungsfeldern       | Felder dienen der manuellen Gewichtung von Merkmalen oder Merkmalsgruppen                                                                                            |
| QM-28 Koeffizienten linearer Modelle            | Gewichtungen für Merkmale in linearer Regressionsanalyse                                                                                                             |
| QM-29 SHAP Feature Importance                   | SHAP misst den individuellen Beitrag jedes Features zur Modellvorhersage.                                                                                            |
| QM-37_Area Under Precision-Recall Curve (AUPRC) | Misst Gesamtleistung bei Präzision und Recall zusammen.                                                                                                              |
| QM-38_GewichteteMetriken                        | Gewichtete Metriken in ML passen Bedeutung von Klassen und Proben an. Jede Metrik lässt sich auch in einer gewichteten Variante darstellen. Bspw.: Weighted Accuracy |
| QM-39 Power Analyse                             | Poweranalyse bestimmt benötigte Stichprobengröße für statistisch signifikanten Effekt.                                                                               |


### Referenzen
| RefID | Verweis                                                                 | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 81    |  The Shapley Value in Machine Learning                                  | In diesem Paper werden die grundlegenden Konzepte der kooperativen Spieltheorie und die axiomatischen Eigenschaften des Shapley-Werts diskutiert sowie dessen Anwendungen in der maschinellen Lernpraxis, einschließlich Merkmalsauswahl, Erklärbarkeit und Multi-Agenten-Verstärkungslernen, sowie die wichtigsten Einschränkungen und zukünftige Forschungsrichtungen aufgezeigt.                                                                                                       |
| 104   |  Verwenden von Häufigkeits- und Gewichtungsfeldern - IBM Dokumentation  | Die Seite erklärt, wie Häufigkeits- und Gewichtungsfelder in SPSS Modeler verwendet werden, um bestimmten Datensätzen mehr Bedeutung beim Modelltraining zu verleihen, wobei Häufigkeitsfelder identische Fälle repräsentieren und Gewichtungsfelder die Relevanz einzelner Datensätze beeinflussen.                                                                                                                                                                                      |
| 176   |  Principal component analysis                                           | Die Hauptkomponentenanalyse (PCA) ist eine wichtige Technik der multivariaten Datenanalyse.                                                                                                                                                                                                                                                                                                                                                                                               |
| 228   |  Functional relevance based on the continuous Shapley value             | Die Studie untersucht die Interpretierbarkeit von Modellen mit funktionalen Daten, die unendlich dimensionale Merkmale verwenden. Sie schlägt eine Methode basierend auf dem Shapley-Wert für kontinuierliche Spiele vor, um die Bedeutung der Prädiktoren fair zu verteilen. Im Fokus steht Scalar-on-Function-Regression. Experimente mit simulierten und realen Datensätzen zeigen die Anwendbarkeit der Methode. Zudem wird die Open-Source-Python-Bibliothek ShapleyFDA vorgestellt. |

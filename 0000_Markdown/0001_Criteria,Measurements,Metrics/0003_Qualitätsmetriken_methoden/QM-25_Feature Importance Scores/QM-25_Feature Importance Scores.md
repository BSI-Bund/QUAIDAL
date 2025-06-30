---
Name: QM-25 Feature Importance Scores (diverse)
Title: QM-25 Feature Importance Scores (diverse)
TitleGer: QM-25 Feature Importance Scores (diverse)
shortdesc: Bewertet die Bedeutung für Merkmalen für ein bestimmtes Ergebnis
tags:
  - Qualitätsmetrik
ID:
  - QM-25
ListMetricID: 
ListMeasureID:
  - "'MA-12'"
  - "'MA-14'"
  - "'QM-10'"
MID: "34"
lcstep: pre
CodeEx: true
share: true
type:
  - metrik
---
## QM-25 Feature-Importance-Scores (diverse)

### Beschreibung

Ein Feature Importance Score ist eine Bewertung oder eine Kennzahl, die im maschinellen Lernen und der statistischen Modellierung verwendet wird, um die Bedeutung von Merkmalen (Features) in einem Datensatz für die Vorhersage oder Klassifikation zu messen. Die Feature Importance Scores sind nützlich, um zu verstehen, welche Merkmale die größte Auswirkung auf die Modellleistung haben. Es gibt verschiedene Arten von Feature Importance Scores, darunter:


### Metriken

| ImpScore                             | Kurzbeschr.                                                                                                                                                                                                   |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-25-1_Variance-Treshold            | Merkmale mit einer Varianz unter einem bestimmten Schwellenwert (Threshold) werden aus dem Datensatz entfernt.                                                                                                |
| QM-26 Gini-Importance                | Die Gini-Importance gibt an, wie viel eine Variable im Durchschnitt zur Verringerung der Gini-Unreinheit über alle Splits und alle Bäume eines Modells beiträgt und quantifiziert so ihre relative Bedeutung. |
| QM-27 Permutation Feature Importance | Methode zur Bestimmung der Bedeutung von Merkmalen                                                                                                                                                            |
| QM-28 Koeffizienten linearer Modelle | Gewichtungen für Merkmale in linearer Regressionsanalyse                                                                                                                                                      |
| QM-29 SHAP Feature Importance        | SHAP misst den individuellen Beitrag jedes Features zur Modellvorhersage.                                                                                                                                     |



### Referenzen

| RefID | Verweis                                                      | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 62    |  Kaggle - Feature Selection Techniques in Machine Learning   | Die Webseite erläutert verschiedene Methoden der Merkmalsauswahl im maschinellen Lernen, wie Filter-, Wrapper- und eingebettete Methoden, und zeigt Python-Codebeispiele zur Verbesserung der Modellleistung.                                                                                                                                                               |
| 102   |  Kaggle - Feature Importance - Beispiele                     | Das Kaggle-Notebook zur Feature Importance bietet einen Überblick über verschiedene Methoden zur Bewertung von Feature-Bedeutungen in Machine-Learning-Modellen, einschließlich Permutationsbedeutung, baumbasierten Modellen und SHAP-Werten, und richtet sich mit praxisnahen Beispielen und Visualisierungen an Praktiker, die das Modellverständnis verbessern möchten. |
| 103   |  Kaggle - Feature Importance. How not fool yourself          | Das Kaggle-Notebook Feature Importance: How Not to Fool Yourself zeigt häufige Fehler bei der Interpretation von Feature-Importance in Machine-Learning-Modellen auf und bietet alternative Ansätze wie SHAP-Werte, um verlässlichere Einblicke zu erhalten.                                                                                                                |
| 135   |  Feature Selection from Differentially Private Correlations  | Der Text beschreibt die Untersuchung einer neuen Methode zur privaten Merkmalsauswahl, die auf Korrelations-basierten Statistiken basiert und im Vergleich zu einer etablierten Methode unter Differential Privacy bessere Ergebnisse bei realen Datensätzen liefert.                                                                                                       |
| 162   |  Confident Feature Ranking                                   | Das Paper stellt eine Methode vor, die Unsicherheiten in Feature-Rankings von maschinellen Lernmodellen durch simultane Konfidenzintervalle quantifiziert, um stabilere und zuverlässigere Interpretationen der globalen Feature-Bedeutung zu ermöglichen.                                                                                                                  |



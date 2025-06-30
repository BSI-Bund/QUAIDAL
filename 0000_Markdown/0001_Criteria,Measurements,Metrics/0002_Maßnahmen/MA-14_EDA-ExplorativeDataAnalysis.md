---
Name: MA-14 EDA-Explorative Daten Analyse
Title: MA-14 EDA-Explorative Daten Analyse
TitleGer: MA-14 EDA-Explorative Daten Analyse
shortdesc: Die Explorative Datenanalyse (EDA) dient dazu, Hauptmerkmale, Muster und Anomalien in Datensätzen zu entdecken, um ein tiefes Verständnis der Daten für fundierte weitere Analyseschritte zu entwickeln.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-14
ListMetricID: 
ListMeasureID:
  - "'QB-12'"
  - "'QB-13'"
  - "'QB-14'"
  - "'QB-04'"
  - "'QB-06'"
share: true
---
## MA-14 EDA: Explorative Daten Analyse

### Beschreibung

Die Explorative Datenanalyse (EDA) ist ein Ansatz zur Analyse von Datensätzen, bei dem der Fokus darauf liegt, die Hauptmerkmale, Muster, Anomalien und Strukturen der Daten zu entdecken, ohne dabei von festen Hypothesen oder vordefinierten Modellen auszugehen. Ziel der EDA ist es, ein tiefes Verständnis der Daten zu entwickeln, um fundierte Entscheidungen über weitere Analyse- oder Modellierungsschritte zu treffen. Bereits trainierte Modelle können wertvolle Hinweise und Erkenntnisse liefern, die eine explorative Datenanalyse (EDA) ergänzen und vertiefen. 

EDA ist besonders nützlich in den frühen Phasen eines Datenanalyseprojekts, bevor formelle Modellierungs- oder Hypothesentests durchgeführt werden. Sie hilft, den weiteren Analyseprozess zu lenken, indem sie wichtige Fragen aufwirft und Erkenntnisse liefert, die ansonsten möglicherweise unentdeckt geblieben wären. Aber durch den KI-Lebenszyklus können das Modelltraining und die Verbesserung des Trainingsdatensatzes durch gewonnene Erkenntnisse der EDA zu weiteren Verbesserungen führen.

#### Hauptmerkmale der EDA:

- **Visuelle Darstellung**:
   - Ein zentraler Bestandteil der EDA ist die visuelle Inspektion der Daten. Dies umfasst das Erstellen von Diagrammen wie Streudiagrammen, Histogrammen, Boxplots und Heatmaps, um Muster, Trends und Ausreißer in den Daten sichtbar zu machen.
   - Visualisierungen helfen dabei, Beziehungen zwischen Variablen zu erkennen, die in rein numerischen Darstellungen möglicherweise übersehen werden.

- **Deskriptive Statistik**:
   - EDA beinhaltet die Berechnung grundlegender statistischer Kennzahlen wie Mittelwert, Median, Modus, Standardabweichung, Quantile und andere deskriptive Maße.
   - Diese Kennzahlen bieten erste Einblicke in die Verteilung und Streuung der Daten sowie in potenzielle Anomalien.

- **Datenbereinigung und -vorbereitung**:
   - Während der EDA werden oft fehlende Werte, Ausreißer oder inkonsistente Daten identifiziert und behandelt.
   - Diese Schritte sind entscheidend, um die Daten für nachfolgende Analysen oder Modellierungen vorzubereiten.

- **Untersuchung von Zusammenhängen**:
   - Die EDA dient dazu, Korrelationen und Zusammenhänge zwischen Variablen aufzudecken. Dies hilft zu verstehen, welche Variablen möglicherweise wichtige Prädiktoren in späteren Modellierungen sein könnten.
   - Paarweise Korrelationsanalysen oder Kreuztabellen sind typische Werkzeuge in diesem Kontext.

- **Hypothesengenerierung**:
   - Ein wichtiger Aspekt der EDA ist das Generieren von Hypothesen. Durch die Untersuchung der Daten können potenzielle Hypothesen für tiefergehende, inferenzstatistische Analysen formuliert werden.
   - EDA ist nicht hypothesengeleitet, sondern explorativ: Man geht offen an die Daten heran, um interessante Muster oder Probleme zu entdecken, die vorher nicht erwartet wurden.

- **Identifikation von Anomalien und Ausreißern**:
   - Die EDA ermöglicht es, ungewöhnliche Datenpunkte oder Muster zu erkennen, die auf Fehler, besondere Bedingungen oder wichtige Datenmerkmale hinweisen könnten.
   - Diese Anomalien müssen oft genauer untersucht werden, um ihre Bedeutung zu verstehen und angemessen darauf zu reagieren.




### Metriken & Methoden

| ID                                                 | Kurzbeschr.                                                                                                                                                                                                   |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-10 Dimension Reduction                          | hochdimensionale Trainingsdaten werden handhabbarer und interpretierbarer                                                                                                                                     |
| QM-10-1_PrincipalComponentAnalysis                 | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                                                                                         |
| QM-10-2_Clustergraph Analysis                      | Ein Verfahren zur Darstellung globaler Beziehungen zwischen Datenclustern                                                                                                                                     |
| QM-12_Prozent fehl. Variablen                      | Durch die Analyse fehlender Informationen in einem Merkmal werden die entsprechenden Prozentzahlen für fehlende Element berechnet.                                                                            |
| QM-24 Bi-Plot                                      | häufig eingesetzt um die Ergebnisse der PCA zu visualisieren                                                                                                                                                  |
| QM-25 Feature Importance Scores (diverse)          | Bewertet die Bedeutung für Merkmalen für ein bestimmtes Ergebnis                                                                                                                                              |
| QM-26 Gini-Importance                              | Die Gini-Importance gibt an, wie viel eine Variable im Durchschnitt zur Verringerung der Gini-Unreinheit über alle Splits und alle Bäume eines Modells beiträgt und quantifiziert so ihre relative Bedeutung. |
| QM-27 Permutation Feature Importance               | Methode zur Bestimmung der Bedeutung von Merkmalen                                                                                                                                                            |
| QM-28 Koeffizienten linearer Modelle               | Gewichtungen für Merkmale in linearer Regressionsanalyse                                                                                                                                                      |
| QM-29 SHAP Feature Importance                      | SHAP misst den individuellen Beitrag jedes Features zur Modellvorhersage.                                                                                                                                     |
| QM-36_AreaUnderCurce (AUC)                         | Messung der Modellperformance; Bewertung der Klassifizierungsgenauigkeit                                                                                                                                      |
| QM-42 QQ-Diagramm                                  | Grafische Vergleich von Quantilen zweier statistischer Variablen.                                                                                                                                             |
| QM-54_ChartTypes                                   | Sammlung von verschiedenen Plottypen nach Einsatzzweck                                                                                                                                                        |
| QM-54-1_SHAP-Summaryplot                           | Visualisiert den Einfluss von Features auf die Vorhersagen des Modells.                                                                                                                                       |
| QM-54-2_SHAP-Dependence-Plot                       | Visualisiert den Einfluss einzelner Variablen auf das Modell.                                                                                                                                                 |
| QM-54-3_SHAP-Force-Plot                            | Visualisiert Auswirkungen von Merkmalen auf das Modell                                                                                                                                                        |
| QM-57-1 Synthetic Minority Over-sampling Technique | eine Methode zur Erzeugung synthetischer Beispiele der Minderheitsklasse in einem unausgeglichenen Datensatz, um die Klassenverteilung auszugleichen und die Modellleistung zu verbessern.                    |
| QM-61 Datenpunkt-Einflussanalyse                   | Verschiedene Methoden die den Einfluss von Datenpunkten auf das Ergebnis eines Modells bewerten.                                                                                                              |
| QM-61-1 Marginal Contribution Approach             | Bewertung des Datenbeitrags in Modellen.                                                                                                                                                                      |
| QM-61-2 Data Re-weighting Strategies               | Anpassung von Datenpunkten zur Modellverbesserung und Fairness.                                                                                                                                               |
| QM-61-3_Neural Dynamic Data Valuation              | Bewertung mit neuronalen Werkzeugen von Datenpunkten in dynamischem Kontext.                                                                                                                                  |



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                      |
| ----- | ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 97    |  Robust statistics                                     | Die zweite Auflage von Robust Statistics liefert eine aktualisierte, praxisorientierte Einführung in qualitative und quantitative Robustheit inklusive neuer Kapitel zu robusten Tests, Small-Sample-Asymptotik, Breakdown-Punkt und Bayesianischer Robustheit sowie erweiterter robuster Regression.                                                                            |
| 98    |  Exploratory Data Analysis                             | Explorative Datenanalyse untersucht Daten ohne vorgegebene Modelle auf ihre Merkmale und Auffälligkeiten, typischerweise vor der Modellauswahl, um Abweichungen von erwarteten Strukturen zu erkennen.                                                                                                                                                                           |
| 159   |  Robust Statistics: Theory and Methods                 | Das Buch Robust Statistics bietet eine Einführung in die Theorie und Anwendung robuster statistischer Methoden, die Abweichungen von Standardverteilungen berücksichtigen, um die Genauigkeit statistischer Modelle zu verbessern, und richtet sich an Forscher, Praktiker und Studierende in verschiedenen wissenschaftlichen Disziplinen.                                      |
| 256   |  A Unified Approach to Interpreting Model Predictions  | SHAP (SHapley Additive exPlanations) ist ein einheitliches Rahmenwerk zur Interpretation von Modellvorhersagen, das einzelnen Merkmalen Wichtigkeitswerte zuweist, eine neue Klasse additiver Maße mit einer einzigartigen Lösung und erwünschten Eigenschaften einführt, bestehende Methoden vereinheitlicht und zudem die Rechenleistung sowie Interpretierbarkeit verbessert. |

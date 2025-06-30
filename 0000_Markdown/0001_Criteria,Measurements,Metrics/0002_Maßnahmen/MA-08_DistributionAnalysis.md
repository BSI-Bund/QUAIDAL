---
Name: MA-08_DistributionAnalysis
Title: MA-08 DistributionAnalysis
TitleGer: MA-08 Verteilungsanalyse
shortdesc: Analyse der Trainingsdaten für bessere Modellleistung und hilft Muster, Trends und mögliche Anomalien zu finden.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-08
ListMetricID: 
ListMeasureID:
  - "'QB-04'"
  - "'QB-03'"
  - "'QB-06'"
share: true
---
## MA-08 Verteilungsanalyse

### Beschreibung

Die Verteilungsanalyse beschreibt die manuelle Überprüfung der Verteilung der Datenpunkte über verschiedene Kategorien oder Gruppen hinweg. Diese Maßnahme ist (ähnlich wie die MA-06 Expertenanalyse) extrem vom Anwendungsfall abhängig und kann sehr aufwendig umzusetzen sein. 

Die Verteilungsanalyse beinhaltet die Untersuchung, wie die verschiedenen Datenpunkte innerhalb des Datensatzes über bestimmte Kategorien, Bereiche oder Klassen verteilt sind. Das Ziel ist es, ein tiefgreifendes Verständnis für die Struktur und die Eigenschaften der Daten zu entwickeln, um sicherzustellen, dass das Modell auf einer robusten Datenverteilung basiert und generalisierbare Vorhersagen treffen kann.

Die Verteilungsanalyse hilft Muster, Trends und mögliche Anomalien in den Trainingsdaten zu identifizieren. Im Zusammenhang mit Maßnahmen wie die "MA-06 Expert-Evaluation" kann dies Aufschluss darüber geben, ob die Daten repräsentativ für das reale zu lösende Problem sind. 

Zum Beispiel kann eine ungleichmäßige Verteilung in Klassifikationsdatensätzen zu einem Modell führen, das in Bezug auf die überrepräsentierte Klasse voreingenommen ist, was die Genauigkeit der Vorhersagen für unterrepräsentierte Klassen beeinträchtigt.

Zudem ermöglicht die Verteilungsanalyse die Identifikation von Ausreißern, die die Modellleistung beeinflussen können, sowie die Erkennung von Mustern, die für die Feature-Engineering-Phase von Bedeutung sein könnten. Die Analyse kann auch dazu beitragen, Entscheidungen über notwendige Datentransformationen (Data/Feature Engineering) zu treffen, um eine bessere Modellanpassung zu erreichen, wie z.B. Normalisierung oder Standardisierung der Daten.

Im Kern unterstützt die Verteilungsanalyse von Trainingsdaten die Entwicklung robuster, effizienter und gerechter Machine-Learning-Modelle, indem sie sicherstellt, dass die zugrundeliegenden Daten gut verstanden (qualitative Information) und angemessen (quantitative Information) vorbereitet sind. 


### Metriken & Methoden

| ID                                                  | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                            |
| --------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-10-1_PrincipalComponentAnalysis                  | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                                                                                                                                                                                                                                                                                                  |
| QM-11 Korrelationskoeffizient(diverse)              | Maß für lineare Beziehung zwischen Variablen.                                                                                                                                                                                                                                                                                                                                                                          |
| QM-11-1_Pearson-Korrelationskoeffizient             | Der Pearson-Korrelationskoeffizient ist ideal für kontinuierliche Daten auf einer Intervall- oder Verhältnisskala, um die Stärke und Richtung eines linearen Zusammenhangs zwischen zwei Variablen auf einer Skala von -1 bis 1 zu messen.                                                                                                                                                                             |
| QM-11-2_Spearman-Rangkorrelationskoeffizient        | Der Spearman-Rangkorrelationskoeffizient ist ein nichtparametrisches Maß für die Stärke und Richtung einer monotonen Beziehung zwischen zwei Rangreihen von Variablen, besonders geeignet für ordinal oder kontinuierlich skalierte Daten mit Ausreißern oder ohne Normalverteilung.                                                                                                                                   |
| QM-11-3_Kendalls Tau                                | Kendall's Tau ist ideal für die Analyse monotone Beziehungen zwischen ordinalen oder rangbasierten Variablen, insbesondere bei nichtlinearen Zusammenhängen, Ausreißern, kleinen Stichproben oder Ties.                                                                                                                                                                                                                |
| QM-11-4_Koeffizient der punktbiserialen Korrelation | Der punktbiseriale Korrelationskoeffizient ist geeignet, um die Stärke und Richtung des Zusammenhangs zwischen einer dichotomen (binären) Variable und einer kontinuierlichen Variable zu messen, wie etwa den Einfluss des Geschlechts auf das Einkommen.                                                                                                                                                             |
| QM-11-5 Phi-Koeffizient                             | ist ein statistisches Maß für die Stärke des Zusammenhangs zwischen zwei dichotomen (binären) Variablen in einer 2x2-Kreuztabelle.                                                                                                                                                                                                                                                                                     |
| QM-51-10_Kolmogorov Smirnov Test                    | Der Kolmogorov-Smirnov-Test (KS-Test) ist ein statistischer Test, der die Übereinstimmung zwischen einer Stichprobe und einer theoretischen Verteilung oder zwischen zwei Stichproben vergleicht, indem er die maximale Differenz zwischen ihren kumulativen Verteilungsfunktionen misst. Er hilft dabei zu bestimmen, ob die Stichproben aus der gleichen Verteilung stammen oder signifikante Unterschiede bestehen. |
| QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS)        | Ausprägung des klassischen Kolmogorov Smirnow Tests auf höherdimensionalen Datensätzen.                                                                                                                                                                                                                                                                                                                                |


### Sourcecode "DistributionAnalysis"

| RefID | Verweis                           | Inhalt                                                 |
| ----- | --------------------------------- | ------------------------------------------------------ |
| 85    | MA-08_DistributionAnalysis_python | Versch. Python Implementierung für Verteilungsanalysen |



### Referenzen

| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                             |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 100   |  An Introduction to Statistical Learning: with Applications in Python  | Präsentiert im wesentlichen ein statistisches Lernwerkzeug für Praktiker in Wissenschaft, Industrie und anderen Bereichen. Demonstriert die Anwendung der statistischen Lernmethoden in Python. Behandelt Regression, Klassifizierung, Baummethoden, SVM, Clustering, Überlebensanalyse, Deep Learning. |

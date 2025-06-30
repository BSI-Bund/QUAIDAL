---
Name: QM-44_Data Imputation Methods
Title: QM-44 Data Imputation Methods
TitleGer: QM-44 Data Imputation Methoden
shortdesc: Datenvervollständigungs-Methoden
tags:
  - Qualitätsmetrik
ID:
  - QM-44
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "53"
CodeEx: true
share: true
lcstep: pre
type:
  - method
---
## QM-44 Data-Imputation-Methoden

### Beschreibung

Daten-Imputation vervollständigt fehlende Daten auf Basis eines bestimmten Algorithmus. Je nach Anwendungsfall muss eine spezifische Vorgehensweise gewählt werden um die optimale Vervollständigungstechnik zu finden. 

 Dies wird typischerweise durch den Einsatz spezifischer Algorithmen erreicht, die auf die Natur der Daten und den Kontext der fehlenden Informationen abgestimmt sind. Der Prozess der Daten-Imputation ist besonders wichtig in Szenarien, in denen das Fehlen von Daten die Analyseergebnisse verzerren oder die Aussagekraft statistischer Modelle einschränken könnte.
 

| Baustein                        | Kurzbeschr.                                                                                         |
| ------------------------------- | --------------------------------------------------------------------------------------------------- |
| QM-44-1 Mittelwert Imputation   | Ersetzung fehlender Werte durch den Mittelwert der beobachteten Werte der entsprechenden Variablen. |
| QM-44-2 Median Imputation       | Ersetzen fehlender Werte durch den Median der beobachteten Werte.                                   |
| QM-44-3 Modus-Imputation        | Nutzung des am häufigsten vorkommenden Wertes (Modus) für kategoriale Daten.                        |
| QM-44-4_Multiple Imputation     | Generiert mehrere vervollständigte Datensätze zur Behandlung von fehlenden Daten.                   |
| QM-44-5 KNN Imputation          | K-Nearest Neighbors ersetzt fehlende Daten mit Werten nächster Nachbarn.                            |
| QM-44-6 Hot Deck Imputation     | Fehlende Werte mit ähnlichen Fällen ermitteln                                                       |
| QM-44-7 LLM-basierte Imputation | LLM Modelle sagen fehlende Werte anhand der Umgebungsvariablen voraus                               |
| QM-44-8 Regression Imputation   | Regressionsmodelle sagen fehlende Werte durch Variablenbeziehungen vorher.                          |


### Referenzen

| RefID | Verweis                                                                       | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ----- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 83    |  A survey on missing data in machine learning                                 | Der Text hebt die Bedeutung der korrekten Behandlung fehlender Werte im maschinellen Lernen hervor, da ignorierte Fehlwerte zu verzerrten Analysen führen können. Er bietet einen Überblick über bestehende Methoden, vergleicht zwei Ansätze (k-nächste Nachbarn und missForest) anhand von Experimenten auf dem Iris- und einem Fan-Datensatz mit 5–20% künstlichen Fehlwerten und zeigt erfolgreiche Imputationsergebnisse sowie zukünftige Forschungsrichtungen auf. |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation         | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können.                                                                                                                                                                                                                                                |
| 171   |  Inference and missing data                                                   | Fehlende Daten können ignoriert werden, wenn sie zufällig fehlen und entweder die beobachteten Daten oder die Parameter der fehlenden Daten unabhängig vom geschätzten Parameter sind.                                                                                                                                                                                                                                                                                   |
| 204   |  Schätzen von Statistiken und Imputieren fehlender Werte - IBM Dokumentation  | Auf der Webseite werden Methoden zur Schätzung von Statistiken und zur Imputation fehlender Werte bei der Datenanalyse mit SPSS erörtert. Es behandelt Techniken wie das listenweise und paarweise Löschen, die EM-Methode (Expectation-Maximization) und die Regressionsimputation für den Umgang mit fehlenden Daten. Auf der Seite wird auch der MCAR-Test erläutert, mit dem festgestellt werden kann, ob Daten völlig zufällig fehlen.                              |
| 212   |  Kaggle - All Imputation Techniques with Pros and Cons                        | Auf der Kaggle-Seite werden Imputationstechniken für fehlende Daten wie Mittelwert, Median, Modusimputation, KNN, Regression und Mehrfachimputation besprochen und die Vor- und Nachteile jeder Methode im Hinblick auf Einfachheit, Verzerrung und Komplexität hervorgehoben.                                                                                                                                                                                           |
| 252   |  Imputation (statistics)                                                      | In der Statistik ersetzt die Imputation fehlende Daten durch geschätzte Werte, um Verzerrungen und Ineffizienzen durch fehlende Daten zu vermeiden. Dies wird eine vollständige Datenanalyse ermöglicht, z. B. durch Methoden wie Mittelwertimputation, Regression und multiple Imputation.                                                                                                                                                                              |




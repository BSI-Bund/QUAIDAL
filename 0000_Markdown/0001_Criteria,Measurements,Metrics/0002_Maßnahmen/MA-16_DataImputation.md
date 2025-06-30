---
Name: MA-16 Daten Imputation
Title: MA-16 Daten Imputation
TitleGer: MA-16 Daten Imputation
shortdesc: Imputation ist die Vervollständigung fehlender Daten in einem Datensatz, um die Integrität für den Lernprozess von ML-Modellen zu gewährleisten, wobei der Grund für das Fehlen der Daten entscheidend für die Wahl des Imputationsverfahrens ist.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-16
ListMetricID: 
ListMeasureID:
  - "'QB-13'"
  - "'QB-06'"
share: true
---
## MA-16 Daten Imputation

### Beschreibung

Als Imputation bezeichnet man die Vervollständigung unvollständiger Datenpunkte in einem größeren Datensatz. In natura erzeugte Datensätze haben die Eigenschaft nicht vollständig zu sein, sei es durch Erfassungsfehler, Nichtantworten in Umfragen etc. Fehlende Daten können den Lernprozess von ML-Modellen beeinflussen und müssen im Vorfeld betrachtet und korrigiert oder entfernt werden. 

Eine wichtige Information ist die Antwort auf die Frage, warum die Daten fehlen, denn der Grund kann Hinweise auf das beste Imputationsverfahren liefern. (Siehe auch MA-13 Vollständige Information). Es gibt zahlreiche Imputationsverfahren, welche je nach Ausgangssituation unterschiedliche Möglichkeiten bieten. 

### Metriken & Methoden
| ID                                        | Kurzbeschr.                                                                                                                           |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| QM-10 Dimension Reduction                 | hochdimensionale Trainingsdaten werden handhabbarer und interpretierbarer                                                             |
| QM-10-1_PrincipalComponentAnalysis        | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                 |
| QM-10-2_Clustergraph Analysis             | Ein Verfahren zur Darstellung globaler Beziehungen zwischen Datenclustern                                                             |
| QM-22 Rekonstruktionsfehler               | Der Rekonstruktionsfehler misst den Unterschied zwischen den ursprünglichen Daten und den durch die (bspw.) PCA rekonstruierten Daten |
| QM-44_Data Imputation Methods             | Datenvervollständigungs-Methoden                                                                                                      |
| QM-44-1 Mittelwert Imputation             | Ersetzung fehlender Werte durch den Mittelwert der beobachteten Werte der entsprechenden Variablen.                                   |
| QM-44-2 Median Imputation                 | Ersetzen fehlender Werte durch den Median der beobachteten Werte.                                                                     |
| QM-44-3 Modus-Imputation                  | Nutzung des am häufigsten vorkommenden Wertes (Modus) für kategoriale Daten.                                                          |
| QM-44-4_Multiple Imputation               | Generiert mehrere vervollständigte Datensätze zur Behandlung von fehlenden Daten.                                                     |
| QM-44-5 KNN Imputation                    | K-Nearest Neighbors ersetzt fehlende Daten mit Werten nächster Nachbarn.                                                              |
| QM-44-6 Hot Deck Imputation               | Fehlende Werte mit ähnlichen Fällen ermitteln                                                                                         |
| QM-44-7 LLM-basierte Imputation           | LLM Modelle sagen fehlende Werte anhand der Umgebungsvariablen voraus                                                                 |
| QM-44-8 Regression Imputation             | Regressionsmodelle sagen fehlende Werte durch Variablenbeziehungen vorher.                                                            |
| QM-44-9_Diffusion Imputation/Augmentation | Daten Imputation mittels stochastischer Rauschprozesse                                                                                |
| QM-53 Regression Methoden                 | Analyse Beziehung zwischen abhängigen und unabhängigen Variablen.                                                                     |
| QM-53-1 Logistische Regression            | Modelliert Wahrscheinlichkeit binärer oder mehrklassiger Ereignisse.                                                                  |
| QM-53-3 Lineare Regression                | Modelliert lineare Beziehung zwischen abhängiger und unabhängiger Variable.                                                           |


### Referenzen
| RefID | Verweis                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 97    |  Robust statistics                                                                    | Die zweite Auflage von Robust Statistics liefert eine aktualisierte, praxisorientierte Einführung in qualitative und quantitative Robustheit inklusive neuer Kapitel zu robusten Tests, Small-Sample-Asymptotik, Breakdown-Punkt und Bayesianischer Robustheit sowie erweiterter robuster Regression.                                                                                                                                                    |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation                 | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können.                                                                                                                                                                                                                                |
| 188   |  Flexible imputation of missing data                                                  | Das Buch erklärt die Methode der multiplen Imputation zur Handhabung fehlender Daten und bietet praktische Beispiele mit dem MICE-Paket. Es liefert verständliche Anleitungen, um unverzerrte Schätzungen zu erstellen, vermeidet technische Details und unterstützt Leser bei der Anwendung dieser Methoden in der Datenanalyse.                                                                                                                        |
| 195   |  Multiple Imputation in der Praxis : ein sozialwissenschaftliches Anwendungsbeispiel  | Multiple Imputation ist eine bewährte Methode zum Umgang mit fehlenden Daten, es gibt jedoch kaum praktische Anleitungen, was sie für Benutzer zu einer Herausforderung macht. Dieses Papier bietet einen schrittweisen Ansatz, der auf häufige Schwierigkeiten eingeht und Lösungen bereitstellt, wobei der Schwerpunkt auf der Datenqualität liegt. Die Methode wird anhand der Imputation des Gesamtvermögens wohlhabender Haushalte veranschaulicht. |
| 252   |  Imputation (statistics)                                                              | In der Statistik ersetzt die Imputation fehlende Daten durch geschätzte Werte, um Verzerrungen und Ineffizienzen durch fehlende Daten zu vermeiden. Dies wird eine vollständige Datenanalyse ermöglicht, z. B. durch Methoden wie Mittelwertimputation, Regression und multiple Imputation.                                                                                                                                                              |

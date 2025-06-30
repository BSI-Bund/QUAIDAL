---
Name: MA-27 StatisticalBasics
Title: MA-27 StatisticalBasics
TitleGer: MA-27 Statistische Grundlagenthemen
shortdesc: Sammelobjekt für statistische Grundlagen
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-27
ListMetricID: 
ListMeasureID:
  - "'QB-01'"
  - "'QB-02'"
  - "'QB-03'"
  - "'QB-04'"
  - "'QB-05'"
  - "'QB-06'"
  - "'QB-07'"
  - "'QB-12'"
  - "'QB-13'"
MID: 
share: true
---
## MA-27 Statistische Grundlagenthemen

### Beschreibung

Es gibt eine Reihe wichtiger Methoden und Metriken, die keiner spezifischen Maßnahme eindeutig zugeordnet werden können, jedoch von grundlegender Bedeutung für die Analyse und Qualitätssicherung im KI-Lebenszyklus sind. Hierzu zählen auch Metriken und statistische Verfahren, die in vielen verschiedenen Bausteinen grundlegend als Teil von Berechnungen zum Einsatz kommen. Um diese Elemente strukturiert in dieses Dokument einzubinden, werden sie unter der Kategorie „Statistische Grundlagenthemen“ zusammengefasst.

Diese Zusammenführung ermöglicht es, die Metriken und Methoden systematisch darzustellen und ihren Wert für übergeordnete Qualitätsaspekte hervorzuheben, selbst wenn sie nicht direkt auf eine einzelne Maßnahme verweisen. So wird eine umfassende Abdeckung statistischer Basisprinzipien erreicht, die als Fundament für fundierte Qualitätsanalysen und Entscheidungen dienen. 


### Metriken & Methoden

| ID                                      | Kurzbeschr.                                                                                                                |
| --------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| QM-01 MeanAbsoluteError                 | Misst den mittleren absoluten Fehler                                                                                       |
| QM-02 Mittlerer quadratischer Fehler    | Der Root Mean Square Error (RMSE) misst die durchschnittliche Abweichung zwischen vorhergesagten und tatsächlichen Werten. |
| QM-03_F-Measure                         | F-Maß vereint Präzision und Trefferquote für Vorhersageleistung.                                                           |
| QM-04 Genauigkeit                       | Verhältnis korrekter Vorhersagen zur Gesamtzahl der Beobachtungen                                                          |
| QM-06 Recall                            | Anteil wahrer Positiver an allen tatsächlichen Positiven.                                                                  |
| QM-07 Spezifität                        | Misst die Fähigkeit echte Positivwerte zu erkennen                                                                         |
| QM-09 KonfidenzNiveau                   | Wahrscheinlichkeit, dass ein Konfidenzintervall den wahren Wert enthält.                                                   |
| QM-23 Mittlerer quadratische Abweichung | Maß für mittlere quadratischen Abweichung zwischen geschätzten und wahren Werten.                                          |
| QM-51 Verteilungstypen                  | Liste verschiedener Wahrscheinlichkeitsverteilungen und Analysen.                                                          |
| QM-51-1 Normalverteilung                | Symmetrische Verteilung mit Schwerpunkt um Mittelwert                                                                      |
| QM-51-2 Binomialverteilung              | Wahrscheinlichkeitsverteilung für Anzahl von Erfolgen in Experimenten.                                                     |
| QM-51-3 Exponentialverteilung           | Verteilung für Wartezeit bis zum Zufallereignis Eintritt.                                                                  |
| QM-51-4 Gleichverteilung                | Gleiche Wahrscheinlichkeit für alle möglichen Ergebnisse im Intervall.                                                     |
| QM-51-5 Chi-Quadrat Verteilung          | Verteilung zur Beschreibung quadratischer Abhängigkeiten von Zufallsvariablen                                              |
| QM-51-6 t-Verteilung                    | Verteilung für Stichprobenmittelwerte bei kleinen Stichprobengrößen                                                        |
| QM-51-7 F-Verteilung                    | Verteilung für Test der Varianzhomogenität und Signifikanzbewertung                                                        |
| QM-51-8_Gamma Verteilung                | Verteilung für Wartezeiten zwischen unabhängigen, zufälligen Ereignissen                                                   |
| QM-51-9 Weibull Verteilung              | Modelliert Lebensdauer, Zuverlässigkeit; flexibel durch Formparameter bestimmt                                             |



### Referenzen

| RefID | Verweis                                                                                                                                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 100   |  An Introduction to Statistical Learning: with Applications in Python                                                                                                                  | Präsentiert im wesentlichen ein statistisches Lernwerkzeug für Praktiker in Wissenschaft, Industrie und anderen Bereichen. Demonstriert die Anwendung der statistischen Lernmethoden in Python. Behandelt Regression, Klassifizierung, Baummethoden, SVM, Clustering, Überlebensanalyse, Deep Learning.                                                                                                                                                            |
| 177   |  Was ist Anomaly Detection? \| IBM                                                                                                                                                     | Die IBM-Webseite erklärt Anomalieerkennung als Methode zur Identifizierung von ungewöhnlichen Daten mithilfe von maschinellem Lernen. Anwendungen sind unter anderem in Cybersicherheit und Betrugserkennung zu finden.                                                                                                                                                                                                                                            |
| 180   |  The elements of statistical learning: data mining, inference, and prediction                                                                                                          | Dieses Buch bietet einen umfassenden Überblick über Schlüsselkonzepte des Data Mining in Bereichen wie Medizin und Finanzen und konzentriert sich dabei auf überwachtes und unüberwachtes Lernen. Es behandelt Themen wie neuronale Netze, Boosting und fügt neue Inhalte zu Random Forests, Ensemble-Methoden und dem Umgang mit „großen“ Daten hinzu. Es ist nützlich für Statistiker und diejenigen, die in der Wissenschaft oder Industrie tätig sind.         |
| 183   |  Statistik: Der Weg zur Datenanalyse                                                                                                                                                   | Das Lehrbuch bietet eine Einführung in deskriptive und induktive Statistik sowie explorative Datenanalyse. Es enthält zahlreiche Grafiken, Anwendungsbeispiele mit realen Daten, R-Codes und Datensätze. Eine Einführung in die Programmiersprache R ist ebenfalls enthalten. Die 9. Auflage bietet überarbeitete Inhalte und Zugriff auf über 100 Lernfragen in der Springer-Nature-Flashcards-App.                                                               |
| 194   |  Statistik für Human- und Sozialwissenschaftler: extras online                                                                                                                         | Das Lehrbuch bietet eine klare Einführung in die Statistik mit Beispielen und Übungen, besonders aus der Psychologie. Die 7. Auflage verbessert die Verständlichkeit und bietet eine neue Website mit SPSS-Anleitungen, Lerntools und Lehrmaterialien.                                                                                                                                                                                                             |
| 196   |  Pattern recognition and machine learning                                                                                                                                              | Die Mustererkennung entstand aus dem Ingenieurwesen und maschinelles Lernen aus der Informatik, aber beide haben sich gemeinsam weiterentwickelt. Bayesianische Methoden, grafische Modelle und Kernel-basierte Modelle haben mit verbesserten Algorithmen wie Variations-Bayes eine zentrale Bedeutung erlangt. Dieses Lehrbuch stellt diese Themen für fortgeschrittene Studierende und Forscher vor, die Kenntnisse in Analysis und linearer Algebra erfordern. |
| 201   |  Statistics for Applications \| Mathematics                                                                                                                                            | Der Kurs vermittelt eine vertiefte theoretische Basis statistischer Methoden und beleuchtet die Rolle der Mathematik bei deren Forschung und Entwicklung.                                                                                                                                                                                                                                                                                                          |
| 202   |  Statistical Thinking and Data Analysis \| Sloan School of Management                                                                                                                  | Einführung in grundlegende statistische Methoden von Wahrscheinlichkeit und Stichproben über Hypothesentests bis Regression, ANOVA sowie kategoriale und nichtparametrische Verfahren.                                                                                                                                                                                                                                                                             |
| 215   |  ISO/IEC 19795-10:2024 - Information technology — Biometric performance testing and reporting — Part 10: Quantifying biometric system performance variation across demographic groups  | Informationstechnologie – Biometrische Leistungstests und Berichterstattung – Teil 10: Quantifizierung der Leistungsschwankungen biometrischer Systeme zwischen demografischen Gruppen                                                                                                                                                                                                                                                                             |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                   | Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                                                                                                                                                                                                                                                                                                                       |

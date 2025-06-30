---
Name: MA-09_CompareGroundtruth
Title: MA-09 CompareGroundtruth
TitleGer: MA-09 VergleichGrundgesamtheit
shortdesc: '"Ground Truth"-Test überprüft Modellqualität mit eindeutigen Referenzdaten.'
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - unsicher
ID:
  - MA-09
ListMetricID: 
ListMeasureID:
  - "'QB-04'"
  - "'QB-03'"
  - "'QB-06'"
share: true
---
## MA-9 Vergleich Grundgesamtheit

### Beschreibung

Von der Ground Truth (Grundgesamtheit) spricht man im Machine Learning Zusammenhang von Daten, die es erlauben, die Qualität von Modellen zu überprüfen. D. h. man hat z.B. Daten, von denen man weiß, wie das Modell sie auszuwerten hätte, weil z. B. ein Mensch sie vorher per Hand (und mit hoher Sicherheit) ausgewertet hat. Die Ground Truth kann aber auch das Wissen über bestimmte Verteilungsfunktionen von Daten beinhalten. Ein ähnliches Konzept ist der „Gold-Standard-Test“. Es handelt sich hier um eine Überprüfung, ob die Datenstichprobe (der Trainingsdatensatz) die tatsächliche Grundgesamtheit widerspiegelt.

### Metriken & Methoden

Alle Metriken müssen entsprechend der Vergleichsmaßnahme angepasst werden und dann gegen verschiedene ähnliche Datensätze validiert werden. Die folgenden Metriken liefern Einblicke in die Qualität und Charakteristika des Datensatzes bevor er für das Training genutzt wird. 


| Metric                                       | Kurzbeschr.                                                                             |
| -------------------------------------------- | --------------------------------------------------------------------------------------- |
| QM-51 Verteilungstypen                       | Liste verschiedener Wahrscheinlichkeitsverteilungen und Analysen.                       |
| QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS) | Ausprägung des klassischen Kolmogorov Smirnow Tests auf höherdimensionalen Datensätzen. |
| QM-52-01 Durchschnittswert                   | Durchschnittlicher Wert einer Anzahl an Datenpunkte eines Merkmals                      |
| QM-52-02_Median                              | mittlerer Wert in einer sortierten Liste von Daten                                      |
| QM-52-03 Modus                               | Häufigster Wert oder Werte in einem Datensatz                                           |
| QM-52-04 Standardabweichung                  | Maß für die Streuung von Daten um Durchschnittswert.                                    |



### Referenzen

| RefID | Verweis                                                                                              | Kurzbeschr.                                                                                                                                                                                                                                                                                             |
| ----- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 73    |  Cheap and Fast – But is it Good? Evaluating Non-Expert Annotations for Natural Language Tasks       | Das Paper untersucht den Einsatz von Amazons Mechanical Turk für kostengünstige und schnelle linguistische Annotationen durch Laien, wobei die Annotationen in mehreren Aufgaben eine hohe Übereinstimmung mit Experten-Labels erreichen und effektiv für maschinelles Lernen genutzt werden können.    |
| 197   |  Distributional Ground Truth: Non-Redundant Crowdsourcing Data Quality Control in UI Labeling Tasks  | Das Papier präsentiert ein nicht-redundantes Verfahren zur Vorhersage der Qualität von Crowdworker-Labels bei Web-UI-Annotationen, das Verteilungen per Kolmogorov-Smirnov-Test vergleicht und so bei einer Trusted-Set-Größe von 17–27 % R²-Werte über 0,8 erreicht und redundante Kontrollen ersetzt. |

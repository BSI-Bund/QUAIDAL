---
Name: MA-03_Range Check
Title: MA-03 Range Check
TitleGer: MA-03 Bereichsprüfung
shortdesc: Bereichsprüfung erkennt Ausreißer und falsche Daten in Merkmalen
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - validation
ID:
  - MA-03
ListMetricID: 
ListMeasureID:
  - "'QB-12'"
  - "'QB-13'"
  - "'QB-01'"
  - "'QB-08'"
  - "'QB-06'"
share: true
---
## MA-03 Bereichsprüfung

### Beschreibung

Diese Maßnahme stellt sicher, dass alle verfügbaren Informationen des Datensatzes außerhalb erwarteter Bereiche liegen (sog. Outlier Detection). Der Hauptzweck dieser Überprüfung besteht darin, die Integrität und Zuverlässigkeit der Daten zu gewährleisten, bevor sie für weitere Analysen verwendet werden.

Neben der Identifikation von Ausreißern hilft die Bereichsprüfung auch dabei, falsche oder ungültige Elemente zu erkennen. Solche Elemente können Datenwerte sein, die aufgrund von Typografiefehlern, falschen Einheiten oder unplausiblen Werten als nicht gültig angesehen werden. Durch das Erkennen und Ausschließen oder Korrigieren dieser fehlerhaften Datenpunkte kann die Qualität der Daten verbessert werden.

Ausreißer können auf verschiedene Ursachen zurückgeführt werden, wie z.B. Eingabefehler, fehlerhafte Datenerfassungsmethoden oder ungewöhnliche Ereignisse, die nicht repräsentativ für den typischen Datenkontext sind. 


### Beispiele 

- Geschwindigkeiten > 400 km/h bei "normalen" PKW
- Negative Werte für das Attribut "Alter" 



### Metriken & Methoden

| ID                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                            |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-51 Verteilungstypen           | Liste verschiedener Wahrscheinlichkeitsverteilungen und Analysen.                                                                                                                                                                                                                                                                                                                                                      |
| QM-51-10_Kolmogorov Smirnov Test | Der Kolmogorov-Smirnov-Test (KS-Test) ist ein statistischer Test, der die Übereinstimmung zwischen einer Stichprobe und einer theoretischen Verteilung oder zwischen zwei Stichproben vergleicht, indem er die maximale Differenz zwischen ihren kumulativen Verteilungsfunktionen misst. Er hilft dabei zu bestimmen, ob die Stichproben aus der gleichen Verteilung stammen oder signifikante Unterschiede bestehen. |
| QM-52_Descriptive-Statistics     | Grundlagen der deskriptiven Statistik                                                                                                                                                                                                                                                                                                                                                                                  |
| QM-52-07 Interquartilsabstand    |  Breite der mittleren 50% der Datenverteilung.                                                                                                                                                                                                                                                                                                                                                                         |



### Referenzen

| RefID | Verweis                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                  |
| ----- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods  | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                          |
| 161   |  ECS: an interactive tool for data quality assurance                                                       | Der Journal Artikel stellt einen neuartigen Ansatz zur Gewährleistung hoher Datenqualität in sicherheitskritischen ML-Systemen vor, erklärt dessen mathematische Grundlagen und zeigt anhand von Beispielen, wie potenziell schädliche Datenpunkte erkannt werden können.    |
| 173   |  OWASP - Development-time threats – AI Exchange                                                            | Die OWASP-Seite beschreibt Risiken während der Entwicklung von KI-Systemen, wie Datenvergiftung, geistigen Diebstahl und Supply-Chain-Angriffe. Sie empfiehlt Schutzmaßnahmen wie Verschlüsselung, Datenisolation und Integritätsprüfungen, um Modelle und Daten zu sichern. |

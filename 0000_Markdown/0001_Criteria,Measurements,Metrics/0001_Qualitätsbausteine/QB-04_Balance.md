---
Name: QB-04_Balance
Title: QB-04_Balance
TitleGer: QB-04 Ausgewogenheit
shortdesc: Ausgewogenheit sichert gleichmäßige Verteilung, Vielfalt maximiert Varianz.
tags:
  - Qualitätsbaustein
ID:
  - QB-04
ListCritID:
  - "'QKB-01'"
share: true
---
## QB-04 Ausgewogenheit

### Beschreibung 

Bei der Erstellung eines Trainingsdatensatzes ist die **quantitative Verteilung** sehr wichtig: Datenpunkte, Kategorien und Merkmale sollten in ihrem Auftreten proportional zur angestrebten Realität abgebildet sein, sodass keine Gruppe über- oder unterrepräsentiert wird. Eine möglichst gleichgewichtete Verteilung aller relevanten Klassen – idealerweise mit gleichem Anteil je Kategorie – verhindert, dass einzelne Klassen dominieren und das Modell einseitig lernt. 

Gleichzeitig wirkt diese Vorgehensweise als Schutz gegen Bias und Overfitting, denn eine ausgewogene Datenbasis verringert systematische Verzerrungen und beugt einer Überanpassung an häufig vorkommende Muster vor. 

Wichtig ist dabei die Abgrenzung zur Vielfalt im engeren Sinne: Anders als das Ziel, möglichst viele unterschiedliche Merkmalsausprägungen (Heterogenität) abzubilden, liegt der Schwerpunkt hier auf einer statistisch gleichmäßigen Verteilung. Denn nur so wird gewährleistet, dass das Modell nicht im Training seltene Klassen vernachlässigt und seine Fähigkeit zur Generalisation – also zur Verallgemeinerung auf neue, ungesehene Daten – nicht durch eine Unterrepräsentation seltener Fälle beeinträchtigt wird.

### Beispiele

#### Ausgewogene gegen unausgewogene binäre Klassifikation 

##### Ausgewogener Datensatz:

- Klasse A: 500 Beispiele
- Klasse B: 500 Beispiele


##### Unausgewogener Datensatz

- Klasse A: 900 Beispiele
- Klasse B: 100 Beispiele

Hier ist Klasse A stark überrepräsentiert. Ein Modell, das mit diesem Datensatz trainiert wird, könnte eine Verzerrung zugunsten von Klasse A entwickeln.

#### Ausgewogene gegen unausgewogene Multiklassenklassifikation

##### Ausgewogener Datensatz

- Klasse A: 300 Beispiele
- Klasse B: 300 Beispiele
- Klasse C: 300 Beispiele

Jede Klasse hat die gleiche Anzahl von Beispielen, was zu einer ausgewogenen Verteilung führt.

##### Unausgewogener Datensatz

- Klasse A: 600 Beispiele
- Klasse B: 300 Beispiele
- Klasse C: 100 Beispiele

In diesem Fall ist Klasse A stark überrepräsentiert und Klasse C stark unterrepräsentiert, was zu einer Verzerrung des Modells führen kann.



### Maßnahmen

| Maßnahme                            | Kurzbeschr.                                                                                                                                                                                              |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MA-08_DistributionAnalysis          | Analyse der Trainingsdaten für bessere Modellleistung und hilft Muster, Trends und mögliche Anomalien zu finden.                                                                                         |
| MA-09_CompareGroundtruth            | "Ground Truth"-Test überprüft Modellqualität mit eindeutigen Referenzdaten.                                                                                                                              |
| MA-10_ManualWeights                 | Manuelle Gewichtung reduziert Bias und verbessert Generalisierung.                                                                                                                                       |
| MA-12 Abdeckung relevanter Merkmale | Abdeckung aller wichtigen Merkmale im Datensatz zur Modellierung.                                                                                                                                        |
| MA-14 EDA-Explorative Daten Analyse | Die Explorative Datenanalyse (EDA) dient dazu, Hauptmerkmale, Muster und Anomalien in Datensätzen zu entdecken, um ein tiefes Verständnis der Daten für fundierte weitere Analyseschritte zu entwickeln. |
| MA-27 StatisticalBasics             | Sammelobjekt für statistische Grundlagen                                                                                                                                                                 |


### Referenzen

| RefID | Verweis                                                                                                                                                              | Kurzbeschr.                                                                                                                                                                                                                                                                                                                          |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 17    |  ISO/IEC 5259-1:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 1: Overview, terminology, and examples                  | Dieser Standard bietet eine Übersicht und definiert die Terminologie sowie Beispiele zur Datenqualität im Kontext von Analytik und maschinellem Lernen. Er adressiert die Bedeutung der Ausgewogenheit von Trainingsdaten als Teil der Datenqualitätsanforderungen.                                                                  |
| 19    |  ISO/IEC 5259-3:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 3: Data quality management requirements and guidelines  | Dieses Dokument definiert allgemeine Anforderungen und Leitlinien für die Verbesserung, Implementierung und Aufrechterhaltung der Datenqualität in Analytik und maschinellem Lernen, anwendbar auf alle Organisationen unabhängig von Art, Größe oder Beschaffenheit, ohne detaillierte Prozesse, Methoden oder Metriken vorzugeben. |
| 20    |  ISO/IEC 5259-4:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 4: Data quality process framework                       | Standardisiertes Verfahren und Rahmenwerk zur Sicherstellung der Datenqualität für Analytik und maschinelles Lernen einschließlich spezifischer Prozesse und Leitlinien gemäß den ISO/IEC 5259-Standards.                                                                                                                            |
| 28    |  ISO/IEC 22989:2022 - Information technology — Artificial intelligence — Artificial intelligence concepts and terminology                                            | Dieser Standard definiert die grundlegenden Konzepte und die Terminologie im Bereich der künstlichen Intelligenz, einschließlich der Aspekte der Datenqualität und Ausgewogenheit von Trainingsdaten.                                                                                                                                |
| 230   |  ISO/IEC TS 12791 - Information technology — Artificial intelligence — Treatment of unwanted bias in classification and regression machine learning tasks            | Information Technology – Artificial Intelligence – Behandlung unerwünschter Verzerrungen bei Klassifizierungs- und Regressionsaufgaben des maschinellen Lernens                                                                                                                                                                      |





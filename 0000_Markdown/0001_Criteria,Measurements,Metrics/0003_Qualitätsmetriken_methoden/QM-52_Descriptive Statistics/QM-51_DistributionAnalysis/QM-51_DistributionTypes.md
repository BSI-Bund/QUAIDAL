---
Name: QM-51 Verteilungstypen
Title: QM-51 Verteilungstypen
TitleGer: QM-51 Verteilungstypen
shortdesc: Liste verschiedener Wahrscheinlichkeitsverteilungen und Analysen.
tags:
  - Qualitätsmetrik
ID:
  - QM-51
ListMetricID: 
ListMeasureID:
  - MA-3
  - "'MA-9'"
  - "'MA-27'"
  - "'MA-03'"
  - "'MA-09'"
MID: "68"
CodeEx: true
share: true
lcstep: pre
type:
  - method
---
## QM-51 Verteilungstypen

### Beschreibung

Wahrscheinlichkeitsverteilungen sind mathematische Funktionen, die die Wahrscheinlichkeitsverteilung von Zufallsvariablen beschreiben. Sie sind von entscheidender Bedeutung in der Statistik und Wahrscheinlichkeitstheorie, da sie es ermöglichen, die Wahrscheinlichkeit verschiedener Ereignisse in einem probabilistischen System zu quantifizieren.

Es gibt verschiedene Arten von Wahrscheinlichkeitsverteilungen, darunter diskrete und stetige Verteilungen. Diskrete Verteilungen modellieren die Wahrscheinlichkeiten von diskreten Ereignissen, während stetige Verteilungen die Wahrscheinlichkeiten von kontinuierlichen Ereignissen modellieren. Folgende Tabelle zeigt einige gebräuchliche Verteilungstypen und Analyseverfahren. 

#### Diskrete & stetige Verteilungen 

- Eine **diskrete Wahrscheinlichkeitsverteilung** beschreibt, mit welcher Wahrscheinlichkeit bestimmte **abzählbare** Ergebnisse eines Zufallsexperiments eintreten.
- Bei **stetigen Wahrscheinlichkeitsverteilungen** kann die Zufallsvariable **beliebige Werte in einem Intervall** annehmen (z. B. Körpergröße, Temperatur).
#### Univariate & multivariate Verteilungen

- **Univariate Verteilungen** beschreiben die Wahrscheinlichkeitsverteilung **einer einzigen** Zufallsvariable. Sie sind die Grundlage vieler statistischer Methoden, zum Beispiel bei der Analyse von Mittelwerten, Varianzen oder bei Hypothesentests. Klassische Beispiele sind die **Normalverteilung**, die **Binomialverteilung** oder die **Exponentialverteilung**.
- **Multivariate Verteilungen** hingegen modellieren die Wahrscheinlichkeiten für **mehrere Zufallsvariablen gleichzeitig**. Sie erlauben nicht nur die Beschreibung der einzelnen Variablen, sondern auch deren **gegenseitigen Abhängigkeiten und Korrelationen**. Die **multivariate Statistik** spielt insbesondere im **maschinellen Lernen** (ML) und der **Datenanalyse** eine zentrale Rolle, da viele realweltliche Datensätze mehrere korrelierte Merkmale enthalten (z. B. Bildpixel, Sensordaten, Textmerkmale). Die Kenntnis und das Modellieren solcher Verteilungen ermöglicht Verfahren wie Dimensionsreduktion, Klassifikation, Clustering und Bayessche Inferenz.

### Auszug möglicher Verteilungstypen

| Metric                                       | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                            |
| -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-51-1 Normalverteilung                     | Symmetrische Verteilung mit Schwerpunkt um Mittelwert                                                                                                                                                                                                                                                                                                                                                                  |
| QM-51-10_Kolmogorov Smirnov Test             | Der Kolmogorov-Smirnov-Test (KS-Test) ist ein statistischer Test, der die Übereinstimmung zwischen einer Stichprobe und einer theoretischen Verteilung oder zwischen zwei Stichproben vergleicht, indem er die maximale Differenz zwischen ihren kumulativen Verteilungsfunktionen misst. Er hilft dabei zu bestimmen, ob die Stichproben aus der gleichen Verteilung stammen oder signifikante Unterschiede bestehen. |
| QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS) | Ausprägung des klassischen Kolmogorov Smirnow Tests auf höherdimensionalen Datensätzen.                                                                                                                                                                                                                                                                                                                                |
| QM-51-2 Binomialverteilung                   | Wahrscheinlichkeitsverteilung für Anzahl von Erfolgen in Experimenten.                                                                                                                                                                                                                                                                                                                                                 |
| QM-51-3 Exponentialverteilung                | Verteilung für Wartezeit bis zum Zufallereignis Eintritt.                                                                                                                                                                                                                                                                                                                                                              |
| QM-51-4 Gleichverteilung                     | Gleiche Wahrscheinlichkeit für alle möglichen Ergebnisse im Intervall.                                                                                                                                                                                                                                                                                                                                                 |
| QM-51-5 Chi-Quadrat Verteilung               | Verteilung zur Beschreibung quadratischer Abhängigkeiten von Zufallsvariablen                                                                                                                                                                                                                                                                                                                                          |
| QM-51-6 t-Verteilung                         | Verteilung für Stichprobenmittelwerte bei kleinen Stichprobengrößen                                                                                                                                                                                                                                                                                                                                                    |
| QM-51-8_Gamma Verteilung                     | Verteilung für Wartezeiten zwischen unabhängigen, zufälligen Ereignissen                                                                                                                                                                                                                                                                                                                                               |
| QM-51-9 Weibull Verteilung                   | Modelliert Lebensdauer, Zuverlässigkeit; flexibel durch Formparameter bestimmt                                                                                                                                                                                                                                                                                                                                         |


### Referenzen

| RefID | Verweis                                             | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                          |
| ----- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 120   |  Univariate (statistics)                            | Unter univariaten Daten versteht man Daten, die aus Beobachtungen zu einem einzelnen Merkmal oder Attribut bestehen. Nachdem sie erfasst und analysiert wurden, können sie mithilfe von Diagrammen und anderen Tools visualisiert werden, wobei ein häufiges Beispiel die Gehälter von Arbeitnehmern sind.                                                                           |
| 259   |  Liste univariater Wahrscheinlichkeitsverteilungen  | Die Liste univariater Wahrscheinlichkeitsverteilungen gibt einen Überblick über eindimensionale Verteilungen, die entweder diskret durch ihre Zähldichte oder stetig durch eine Dichtefunktion beschrieben werden, wobei Wahrscheinlichkeiten stetiger Verteilungen über Integrale dargestellt werden.                                                                               |
| 298   |  Multivariate (statistics)                          | Multivariate Statistik untersucht mehrere Ergebnisvariablen gleichzeitig, um Zusammenhänge zu erkennen und zu analysieren. Sie umfasst verschiedene Analyseformen und nutzt multivariate Wahrscheinlichkeitsverteilungen zur Modellierung und statistischen Schlussfolgerung. Methoden wie die multiple Regression zählen meist nicht dazu, da sie nur eine Zielvariable betrachten. |



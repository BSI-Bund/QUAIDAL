---
Name: MA-25 Differential Privacy
Title: MA-25 Differential Privacy
TitleGer: MA-25 Differential Privacy
shortdesc: Schutz individueller Daten durch zufällige Rauschzusätze.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - unsicher
ID:
  - MA-25
ListMetricID: 
ListMeasureID:
  - "'QB-13'"
MID: 
lcstep: 
share: true
---
## MA-25 Differential Privacy

### Beschreibung

Differenzielle Privatsphäre ist ein Konzept und eine Methode, die darauf abzielt, die Privatsphäre der Teilnehmer in einem Datensatz zu schützen, während statistische Analysen ermöglicht werden. Sie bietet eine formale Garantie dafür, dass die Hinzufügung oder Entfernung eines einzelnen Datensatzes aus einem Datensatz das Ergebnis einer Abfrage nur minimal beeinflusst. Dadurch wird sichergestellt, dass aus dem Ergebnis einer Analyse keine Rückschlüsse auf die An- oder Abwesenheit einzelner Datensätze im Datensatz gezogen werden können.

#### Kernkonzepte

- **Zufälligkeit**: Differenzielle Privatsphäre wird oft durch das Hinzufügen von Zufälligkeit (Rauschen) zu den Antworten einer Abfrage oder zu den Daten selbst erreicht. Das Rauschen wird so gewählt, dass es die Genauigkeit der Gesamtergebnisse nur geringfügig beeinträchtigt, aber ausreichend ist, um die Privatsphäre der Einzeldaten zu schützen.
- **Epsilon (ε)**: Ein zentraler Parameter in der differenziellen Privatsphäre ist Epsilon (ε), der das Maß an Privatsphäre und das Risiko eines Informationslecks bestimmt. Ein kleineres ε bedeutet eine höhere Privatsphäre (und mehr Rauschen), während ein größeres ε weniger Privatsphäre (und weniger Rauschen) bedeutet.

#### Anwendungen

Differenzielle Privatsphäre kann in vielen Bereichen eingesetzt werden, einschließlich, aber nicht beschränkt auf:

- **Datenerhebungen**: Schutz der Privatsphäre von Teilnehmenden bei Umfragen und Zensusdaten.
- **Maschinelles Lernen**: Schutz von Trainingsdaten beim Trainieren von maschinellen Lernmodellen.
- **Statistische Abfragen**: Schutz der Privatsphäre bei der Beantwortung von Abfragen auf Datensätzen, wie zum Beispiel Durchschnittswerten, Summen oder Zählungen.

### Metriken & Methoden

| ID                                         | Kurzbeschr.                                                              |
| ------------------------------------------ | ------------------------------------------------------------------------ |
| QM-58 Differential Privacy Methods         | Zusammenfassung der Differential Privacy Methoden                        |
| QM-58-1 Laplacescher Mechanismus           | Fügt Rauschen hinzu, um differenzielle Privatsphäre zu gewährleisten.    |
| QM-58-2 Exponentialmechanismus             | Methode zur Gewährleistung der "Differential Privacy"                    |
| QM-58-3 Lokale differentielle Privatsphäre | Methoden der differentiellen Privatsphäre, umgesetzt bereits beim Nutzer |



### Referenzen

| RefID | Verweis                                                                            | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ---------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 77    |  A Survey on Differentially Private Machine Learning                               | Diese Arbeit untersucht Differential Privacy im maschinellen Lernen, konzentriert sich auf Methoden zur Rauschzugabe zu Modellen und Zielfunktionen zum Schutz der Privatsphäre und hebt zukünftige Forschungsschwerpunkte hervor.                                                                                                                                                                                                                                         |
| 172   |  How to DP-fy ML: A Practical Guide to Machine Learning with Differential Privacy  | Die Übersichtsarbeit bietet Forschenden und Praktiker:innen einen kompakten Leitfaden zu Differential Privacy in Machine Learning, erklärt gängige Herausforderungen (z. B. Hyperparameter-Tuning, Architekturänderungen) und Best Practices für strenge Datenschutzgarantien bei gleichzeitig akzeptabler Modellgüte.                                                                                                                                                     |
| 198   |  Deep Learning with Differential Privacy                                           | ML-Modelle, die neuronale Netzwerke verwenden, benötigen große Datensätze, die oft sensible Informationen enthalten. Um die Privatsphäre zu schützen, werden innerhalb des Rahmens der differentiellen Privatsphäre neue Techniken entwickelt. Dieser Ansatz ermöglicht das Training von tiefen neuronalen Netzwerken mit nicht-konvexen Zielen, während Privatsphäre, Softwarekomplexität, Trainingseffizienz und Modellqualität ausbalanciert werden.                    |
| 292   |  The Algorithmic Foundations of Differential Privacy                               | The Algorithmic Foundations of Differential Privacy definiert das Konzept der differentiellen Privatsphäre, erläutert zentrale Mechanismen wie den Laplaceschen und Exponentialmechanismus, führt Kompositionstheoreme für wiederholte Abfragen an, diskutiert die Balance zwischen Datenschutz und Genauigkeit und bietet damit sowohl eine fundierte theoretische Grundlage als auch praxisrelevante Einsichten für die Entwicklung datenschutzfreundlicher Algorithmen. |



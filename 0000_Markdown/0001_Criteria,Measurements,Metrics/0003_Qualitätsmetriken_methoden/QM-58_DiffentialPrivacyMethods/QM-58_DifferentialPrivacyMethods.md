---
Name: QM-58 Differential Privacy Methods
Title: QM-58 DifferentialPrivacyMethods
TitleGer: QM-58 Methoden der "Differential Privacy"
shortdesc: Zusammenfassung der Differential Privacy Methoden
tags:
  - Qualitätsmetrik
ID:
  - QM-58
ListMetricID: 
ListMeasureID:
  - "'MA-25'"
MID: "98"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-58_Methoden der Differential Privacy

### Beschreibung

- **Laplacescher Mechanismus**: Hinzufügen von Laplace-verteiltem Rauschen zu den Ergebnissen einer Abfrage, basierend auf der Sensitivität der Abfrage.
- **Exponentialmechanismus**: Auswahl einer Antwort aus einer Menge möglicher Antworten mit einer Wahrscheinlichkeit, die von der Genauigkeit der Antwort und einem Rauschparameter abhängt.
- **Lokale differenzielle Privatsphäre**: Anwenden differenzieller Privatsphäre direkt auf die Daten der Nutzenden, bevor sie gesammelt oder analysiert werden.

### Ansätze
| Tool                                       | Kurzbeschr.                                                              |
| ------------------------------------------ | ------------------------------------------------------------------------ |
| QM-58-1 Laplacescher Mechanismus           | Fügt Rauschen hinzu, um differenzielle Privatsphäre zu gewährleisten.    |
| QM-58-2 Exponentialmechanismus             | Methode zur Gewährleistung der "Differential Privacy"                    |
| QM-58-3 Lokale differentielle Privatsphäre | Methoden der differentiellen Privatsphäre, umgesetzt bereits beim Nutzer |


### Referenzen
| RefID | Verweis                                                                            | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 77    |  A Survey on Differentially Private Machine Learning                               | Diese Arbeit untersucht Differential Privacy im maschinellen Lernen, konzentriert sich auf Methoden zur Rauschzugabe zu Modellen und Zielfunktionen zum Schutz der Privatsphäre und hebt zukünftige Forschungsschwerpunkte hervor.                                                                                                                                                                                                                      |
| 117   |  Differential Privacy                                                              | Differential Privacy maximiert die Genauigkeit von Datenbankabfragen, während gleichzeitig das Risiko minimiert wird, individuelle Datensätze zu identifizieren. Dies wird erreicht, indem verhindert wird, dass Angreifer feststellen können, ob eine bestimmte Person in der Datenbank enthalten ist.                                                                                                                                                 |
| 135   |  Feature Selection from Differentially Private Correlations                        | Der Text beschreibt die Untersuchung einer neuen Methode zur privaten Merkmalsauswahl, die auf Korrelations-basierten Statistiken basiert und im Vergleich zu einer etablierten Methode unter Differential Privacy bessere Ergebnisse bei realen Datensätzen liefert.                                                                                                                                                                                   |
| 172   |  How to DP-fy ML: A Practical Guide to Machine Learning with Differential Privacy  | Die Übersichtsarbeit bietet Forschenden und Praktiker:innen einen kompakten Leitfaden zu Differential Privacy in Machine Learning, erklärt gängige Herausforderungen (z. B. Hyperparameter-Tuning, Architekturänderungen) und Best Practices für strenge Datenschutzgarantien bei gleichzeitig akzeptabler Modellgüte.                                                                                                                                  |
| 198   |  Deep Learning with Differential Privacy                                           | ML-Modelle, die neuronale Netzwerke verwenden, benötigen große Datensätze, die oft sensible Informationen enthalten. Um die Privatsphäre zu schützen, werden innerhalb des Rahmens der differentiellen Privatsphäre neue Techniken entwickelt. Dieser Ansatz ermöglicht das Training von tiefen neuronalen Netzwerken mit nicht-konvexen Zielen, während Privatsphäre, Softwarekomplexität, Trainingseffizienz und Modellqualität ausbalanciert werden. |




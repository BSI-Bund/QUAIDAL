---
Name: QM-45 Prior Ermittlung
Title: QM-45 Prior Ermittlung
TitleGer: QM-45 Prior Ermittlung
shortdesc: Prozess zur Bewertung von Vorwissen vor statistischer Datenanalyse.
tags:
  - Qualitätsmetrik
ID:
  - QM-45
ListMetricID: 
ListMeasureID:
  - "'MA-6'"
  - "'MA-06'"
MID: 
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-45 Prior Ermittlung

### Beschreibung

Prior Elicitation bezeichnet einen Prozess in der Statistik und Datenwissenschaft, bei dem systematisch Expertenwissen gesammelt wird, um Vorabinformationen (sogenannte "Priors") für bayes-statistischen Analysen zu definieren. Diese Priori repräsentieren die anfänglichen Annahmen über die Wahrscheinlichkeitsverteilungen der zu untersuchenden Parameter, bevor neue Daten betrachtet werden. Der Prozess hilft, subjektive Einschätzungen quantitativ in die Analyse einzubeziehen, um die Unsicherheiten in Modellen zu verringern und die Interpretation von Daten zu verbessern.

Methoden zur Sammlung von Expertenwissen: 
- **Expertenbefragung**: Durch Interviews oder Fragebögen werden Experten nach ihrer Einschätzung über Unsicherheiten und Parameterwerte befragt. Ihre Antworten helfen, subjektive Prior-Verteilungen zu formen.
- **Historische Datenanalyse:** Vorherige Studien oder historische Daten werden genutzt, um Prior-Verteilungen abzuleiten. Dies basiert auf der Annahme, dass vergangene Muster oder Ergebnisse relevante Informationen für zukünftige Ereignisse liefern.
- **Literaturbasierte Elicitation**: Analyse von veröffentlichten Forschungsarbeiten oder Meta-Analysen, um Priors zu extrahieren, die auf bereits gesammeltem Wissen basieren.
- **Verwendung von computergestützten Tools**: Spezielle Software kann verwendet werden, um Expertenurteile systematisch zu erfassen und zu quantifizieren, welche dann in Prior-Verteilungen umgesetzt werden.
- **Workshops und Gruppendiskussionen**: In interaktiven Sitzungen diskutieren Experten gemeinsam über die Parameter und deren Verteilungen, um zu einem Konsens zu kommen.
- **Delphi-Methode**: Eine strukturierte Kommunikationstechnik, oft als eine Reihe von Fragebögen, bei der Experten ihre Meinungen anonym äußern. Nach jeder Runde werden die aggregierten Ergebnisse den Teilnehmern zurückgemeldet, und sie haben die Möglichkeit, ihre Antworten zu überdenken und zu verfeinern.

Diese Methoden können je nach Kontext und Verfügbarkeit von Informationen und Experten kombiniert oder einzeln verwendet werden.

### Methode

#### 1. Identifizierung der Parameter
Zunächst werden die Parameter, für die Prior-Informationen benötigt werden, identifiziert. Dies kann sich auf alles von Mittelwerten über Standardabweichungen bis hin zu Prozentsätzen erstrecken.

#### 2. Sammlung von Vorinformationen
Vorinformationen können aus verschiedenen Quellen gesammelt werden:
- Experteneinschätzungen: Expertenwissen wird durch Befragungen oder Interviews erfasst.
- Historische Daten: Frühere Studienergebnisse oder statistische Daten liefern Anhaltspunkte für plausible Werte und deren Variabilität.
- Literatur: Veröffentlichte Forschungsergebnisse, Meta-Analysen oder Fachbücher.

#### 3. Wahl des Typs der Prior-Verteilung
Abhängig von der Natur des Parameters und der verfügbaren Information wird ein geeigneter Verteilungstyp ausgewählt. Beispiele für häufig verwendete Prior-Verteilungen sind:
- Normalverteilung: Geeignet für viele kontinuierliche Parameter.
- Beta-Verteilung: Nützlich für Parameter, die Wahrscheinlichkeiten darstellen.
- Gamma-Verteilung: Häufig verwendet für Skalenparameter und Raten.
- Uniformverteilung: Wenn sehr wenig spezifische Vorinformation vorhanden ist und alle Werte als gleich wahrscheinlich angesehen werden.

#### 4. Parametrisierung der Verteilung
Die ausgewählte Verteilung muss mit spezifischen Parametern versehen werden, die auf den gesammelten Informationen basieren. Dies beinhaltet:
- Bestimmung von Lage- und Skalenparametern: Zum Beispiel Mittelwert und Varianz für eine Normalverteilung.
- Nutzung statistischer Methoden: Techniken wie Maximum Likelihood oder Methoden der kleinsten Quadrate können genutzt werden, um Parameter zu schätzen.

#### 5. Verwendung von Elicitation-Tools
Spezielle Softwaretools können dabei helfen, die Meinungen mehrerer Experten zu aggregieren und zu quantifizieren, um eine konsistente Prior-Verteilung zu erstellen. Tools wie SHELF (Sheffield Elicitation Framework) oder MATCH (Method for Elicitation of Expert Judgment) sind hierbei hilfreich.

#### 6. Validierung und Anpassung
Die erstellten Prior-Verteilungen sollten auf Plausibilität geprüft und gegebenenfalls angepasst werden. Dies kann durch Diskussionen mit Experten oder durch Überprüfung der Implikationen der Priori in vorläufigen Analysemodellen erfolgen.

#### 7. Dokumentation
Die Entscheidungen und Annahmen, die bei der Erstellung der Prior-Verteilungen getroffen wurden, sollten sorgfältig dokumentiert werden, um Transparenz und Nachvollziehbarkeit zu gewährleisten.

Durch diesen Prozess wird sichergestellt, dass die verwendeten Priors gut begründet und für die jeweilige analytische Aufgabe geeignet sind.


### Beispiel - Prior Elicitation zur Augmentierung von Trainingsdaten für ein medizinisches Diagnosemodell

Angenommen, wir entwickeln ein maschinelles Lernmodell zur Diagnose einer bestimmten Krankheit basierend auf medizinischen Bilddaten. Wir möchten die Trainingsdaten durch Augmentierung verbessern und benötigen dafür Prior-Informationen, um geeignete Augmentierungsmethoden und -parameter zu bestimmen.

#### Schritt 1: Identifizierung der Parameter

Wir identifizieren die Parameter, die für die Augmentierung der Trainingsdaten wichtig sind. Diese Parameter könnten folgende sein:

- Drehwinkel (Rotation) der Bilder zur Erhöhung der Modellrobustheit gegen unterschiedliche Bildausrichtungen.
- Helligkeit und Kontrast zur Anpassung an variierende Aufnahmebedingungen.
- Skalierung (Zoom) zur Simulation unterschiedlicher Aufnahmedistanzen.

#### Schritt 2: Sammlung von Vorinformationen

Wir sammeln Vorinformationen zu diesen Parametern aus mehreren Quellen:

- Experteneinschätzungen: Radiologen und Bildverarbeitungsexperten werden zu optimalen Rotationswinkeln und Helligkeits-/Kontrastveränderungen befragt, die diagnostische Merkmale nicht verfälschen.
- Historische Daten: Frühere Studien zu ähnlichen Modellen und deren Daten-Augmentierungsstrategien werden analysiert, um übliche Parameterbereiche zu identifizieren.
- Literatur: Veröffentlichungen über bewährte Praktiken in der Bildaugmentierung für medizinische Modelle werden untersucht, um die Häufigkeit und den Effekt verschiedener Augmentierungstechniken zu verstehen.

#### Schritt 3: Wahl des Typs der Prior-Verteilung

Basierend auf den gesammelten Informationen wählen wir geeignete Prior-Verteilungen für die Parameter:

- Drehwinkel: Wir wählen eine Normalverteilung mit einem Mittelwert von 0 Grad und einer Standardabweichung, die auf Expertenmeinungen basiert, um die Wahrscheinlichkeit kleiner und mittlerer Rotationen zu modellieren.
- Helligkeit und Kontrast: Eine Beta-Verteilung wird verwendet, da diese Wahrscheinlichkeiten für die Anpassung von Helligkeit und Kontrast modelliert, die auf einem Intervall zwischen 0 und 1 liegen.
- Skalierung (Zoom): Eine Gamma-Verteilung wird ausgewählt, da sie positiv-skaliert ist und die Varianz im Zoomfaktor modelliert.

#### Schritt 4: Parametrisierung der Verteilung

Wir parametrisieren die Verteilungen mit den gesammelten Informationen:

- Drehwinkel (Rotation): Mittelwert = 0 Grad, Standardabweichung = 15 Grad (basierend auf Expertenmeinungen, dass Rotationen bis zu 30 Grad noch diagnostische Merkmale erhalten).
- Helligkeit und Kontrast: Alpha und Beta der Beta-Verteilung werden basierend auf historischen Daten und Expertenmeinungen gesetzt (z.B., Alpha = 2, Beta = 5).
- Skalierung (Zoom): Die Form- und Skalenparameter der Gamma-Verteilung werden durch Methoden der kleinsten Quadrate geschätzt (z.B., Formparameter = 2, Skalenparameter = 0.5).

####  Schritt 5: Verwendung von Elicitation-Tools

Wir nutzen das SHELF-Tool (Sheffield Elicitation Framework), um die Expertenmeinungen quantitativ zu aggregieren. Die Experten geben ihre Einschätzungen zu den Wahrscheinlichkeiten und Verteilungsparametern, die im Tool verarbeitet und in eine konsistente Prior-Verteilung integriert werden.

####  Schritt 6: Validierung und Anpassung

Die Prior-Verteilungen werden anhand von Diskussionen mit den Experten überprüft. Die Experten bewerten die Plausibilität der gewählten Verteilungen in Bezug auf ihre Erfahrung und das Zielmodell. Bei Abweichungen werden die Parameter und Verteilungen entsprechend angepasst. Anschließend führen wir vorläufige Analysen mit einem kleinen Testdatensatz durch, um sicherzustellen, dass die Augmentierung nicht zu unrealistischen oder unbrauchbaren Daten führt.

####  Schritt 7: Dokumentation

Alle Annahmen, die Auswahl der Verteilungstypen und deren Parametrisierung sowie die Ergebnisse der Validierungsanalysen werden sorgfältig dokumentiert. Dies umfasst:

- Die verwendeten Expertenmeinungen und ihre Aggregation.
- Die herangezogenen historischen Daten und Literaturquellen.
- Die genauen Parameter der Prior-Verteilungen und die Methoden ihrer Bestimmung.


### Referenzen

| RefID | Verweis                                                      | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                  |
| ----- | ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 174   |  Prior Knowledge Elicitation: The Past, Present, and Future  | Die Spezifikation der Prior-Verteilung im Bayes'schen Workflow ist wichtig, aber oft schwierig. Prior-Elicitation soll domänenspezifisches Wissen in Prior-Verteilungen umwandeln, doch es fehlen effiziente Tools und eine theoretische Grundlage. Der Text analysiert den Stand der Forschung, identifiziert Schwächen und schlägt neue Ansätze zur Verbesserung der Prior-Elicitation vor |
| 305   |  Sheffield Elicitation Framework                             | SHELF ist ein Paket für die Erhebung von Wahrscheinlichkeitsverteilungen unsicherer Größen durch Experten, wenn Daten knapp sind.                                                                                                                                                                                                                                                            |


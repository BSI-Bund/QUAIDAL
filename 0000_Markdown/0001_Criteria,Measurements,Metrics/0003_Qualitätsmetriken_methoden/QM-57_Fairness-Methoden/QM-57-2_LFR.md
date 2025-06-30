---
Name: QM-57-2_LFR
Title: QM-57-2 LFR
TitleGer: QM-57-2 LFR
shortdesc: Methode des Representation Learning, die Bias bereits während des Modelltrainings reduziert
tags:
  - Qualitätsmetrik
ID:
  - QM-57-2
ListMetricID: 
ListMeasureID:
  - "'MA-30'"
MID: 
type:
  - metrik
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-57-2 Learning Fair Representation

Der Inprozessierungsbaustein **QM-57-2 Learning Fair Representation** erläutert den Algorithmus **Learning Fair Representations (LFR)**, eine Methode des Representation Learning, die Bias bereits während des Modelltrainings reduziert. LFR lernt eine Menge von **Prototypen**, auf die alle Datenpunkte projiziert werden. Dabei optimiert der Algorithmus simultan zwei Ziele:

- **Vorhersageleistung maximieren**: Die latent erzeugten Repräsentationen sollen möglichst viel der ursprünglichen Information zum Label („eingestellt“ vs. „nicht eingestellt“) behalten.
- **Statistische Parität erzwingen**: Die Wahrscheinlichkeit, mit der Bewerbende verschiedener Gruppen auf die einzelnen Prototypen verteilt werden, wird angeglichen. So wird sichergestellt, dass keine Gruppe bevorzugt oder benachteiligt wird.

Technisch geschieht dies über einen alternierenden Optimierungsprozess, in dem einerseits die Prototyp-Positionen und andererseits die Zuordnungsgewichte aktualisiert werden. Häufig kommen hier Regularisierungsgewichte zum Einsatz, um den Kompromiss zwischen Fairness und Genauigkeit zu steuern. Ergänzend kann ein **adversariales Training** integriert werden: Ein zweites Netzwerk versucht, aus den gelernten Repräsentationen Gruppenunterschiede zu erkennen, während das Hauptnetzwerk lernt, diese Detektion zu verhindern. So wird die Fairness weiter erhöht.

Synonyme für Learning Fair Representations sind unter anderem **„Faire Repräsentationslernen“**, **„Latent Paritäts-Projektionen“** oder kurz **„LFR“**. Allen Begriffen gemeinsam ist die Erzeugung fairer, latenter Datenabbildungen für diskriminierungsfreie Modellentscheidungen.

Abzugrenzen ist LFR gegenüber anderen Bias-Methoden:
- **Präprozessierung** verändert nur die Rohdaten vor dem Training, während LFR direkt in den Lernprozess eingreift.
- **Postprozessierung** passt nur die Modelloutputs an, statt die inneren Repräsentationen zu transformieren.
- **Adversarial Debiasing** als eigenständige Methode nutzt zwar ebenfalls Gegnernetzwerke, verfolgt aber nicht den Prototypen-Ansatz zur latenten Gruppenausgleichung.



### Sourcecode "LFR 1"
| RefID | Verweis            |
| ----- | ------------------ |
| 95    | QM-57-2_LFR_python |



### Referenzen
| RefID | Verweis                                            | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----- | -------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 302   |  Papers with Code - Learning Fair Representations  | Der vorgeschlagene Lernalgorithmus erzielt sowohl Gruppenfairness als auch individuelle Fairness, indem er eine Repräsentation lernt, die einerseits die Daten gut abbildet und andererseits Informationen über geschützte Gruppen verschleiert. Diese Zwischenrepräsentation ist vielseitig einsetzbar (z. B. für Transferlernen) und hilft dabei, wichtige Klassifikationsdimensionen im Datensatz zu identifizieren. |


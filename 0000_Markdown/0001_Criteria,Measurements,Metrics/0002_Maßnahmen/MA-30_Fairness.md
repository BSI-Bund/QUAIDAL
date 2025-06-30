---
Name: MA-30_Fairness
Title: MA-30 Fairness
TitleGer: MA-30 Fairness
shortdesc: Fairness im Machine Learning bezeichnet Techniken (z. B. SMOTE, LFR), die systematische Verzerrungen in Daten und Modellen korrigieren, um gerechte, gleichbehandelte Vorhersagen für alle demografischen Gruppen zu gewährleisten.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-30
ListMetricID: 
ListMeasureID:
  - "'QB-15'"
MID: 
share: true
---
## MA-30 Fairness

### Beschreibung
Fairness bezeichnet in datengetriebenen Systemen die Eigenschaft, Entscheidungen und Vorhersagen so zu gestalten, dass sie keine systematischen Benachteiligungen oder Privilegierungen bestimmter Gruppen (z. B. nach Geschlecht, Ethnie oder Alter) aufweisen. Ein faires Modell strebt danach, verschiedene demografische Gruppen gleichbehandelt zu behandeln und unerwünschte Verzerrungen in den Daten oder im Lernprozess zu korrigieren. Die Maßnahme „Fairness“ umfasst sowohl präventive Schritte bei der Datenerhebung und -aufbereitung als auch nachgelagerte Techniken zur Bias-Korrektur während oder nach dem Training.

In der Vorverarbeitung können Techniken wie SMOTE (Synthetic Minority Over-sampling Technique) eingesetzt werden, um unterrepräsentierte Subgruppen künstlich aufzustocken und dem Modell ausreichend Beispiele beider Gruppen zur Verfügung zu stellen. In-Algorithmus-Ansätze wie LFR (Learning Fair Representations) transformieren die Merkmalsräume so, dass die sensiblen Merkmale (z. B. Geschlecht) möglichst wenig Rückschluss auf die Klassenzugehörigkeit zulassen, während die prädiktive Leistungsfähigkeit weitgehend erhalten bleibt. 

Im Kontext von Fairness bezeichnet man auch verschiedene Metriken zur Quantifizierung von Gleichbehandlung, etwa **Demographic Parity** (gleiche positive Vorhersagewahrscheinlichkeiten) oder **Equalized Odds** (gleiche Fehlerraten). Die Auswahl der passenden Metrik und Technik hängt dabei stets von den konkreten Anwendungsbedingungen und regulatorischen Vorgaben ab.

Synonyme für Fairness sind unter anderem **Unvoreingenommenheit**, **Gleichbehandlung** oder **Bias-Reduktion**. In der Fachliteratur findet man gelegentlich auch den Begriff **Fair Machine Learning**, der den ganzheitlichen Prozess der Bias-Erkennung und -Behebung in ML-Modellen bezeichnet.

Abzugrenzen ist Fairness insbesondere von **Diversität** (Vielfalt in den Daten, z. B. verschiedene Merkmalswerte) und **Inklusion** (aktive Einbindung aller Gruppen), da Fairness vor allem auf die gerechte Verteilung von Modellentscheidungen abzielt, während Diversität und Inklusion breiter angelegte Organisations- und Datenstrategien umfassen.



### Beispiele 

#### Beispiel 1: Einsatz von SMOTE (QM-57-1)

Ein Kreditbewilligungssystem weist in den historischen Daten eine Unterrepräsentation von Bewerberinnen auf. Um eine faire Behandlung sicherzustellen, wendet man vor dem Modelltraining die SMOTE-Technik an, um synthetisch zusätzliche Beispiele für den weiblichen Teil der Trainingsdaten zu erzeugen. Anschließend wird das Modell auf dem ausgeglichenen Datensatz trainiert, wodurch die Decision-Score-Verteilung für beide Geschlechter vergleichbarer wird und die Rate falscher Ablehnungen für Frauen sinkt.

#### Beispiel 2: Anwendung von LFR (Learning Fair Representations)(QM-57-2) 

Bei der automatisierten Personalauswahl sollen keine Rückschlüsse auf das Geschlecht der Bewerbenden möglich sein. Mit dem LFR-Algorithmus transformiert man die ursprünglichen Bewerberdaten in einen neuen Repräsentationsraum, in dem die Distanz zwischen den Gruppenmerkmalen minimiert wird, aber die Trennfähigkeit für die Auswahlkriterien erhalten bleibt. Das resultierende Modell trifft Entscheidungen auf Basis der fairen Repräsentation und zeigt geringere Unterschiede in den Vorhersagequoten zwischen Männern und Frauen.


### Metriken & Methoden

| ID                                                 | Kurzbeschr.                                                                                                                                                                                |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-57-1 Synthetic Minority Over-sampling Technique | eine Methode zur Erzeugung synthetischer Beispiele der Minderheitsklasse in einem unausgeglichenen Datensatz, um die Klassenverteilung auszugleichen und die Modellleistung zu verbessern. |
| QM-57-2_LFR                                        | Methode des Representation Learning, die Bias bereits während des Modelltrainings reduziert                                                                                                |



### Referenzen

| RefID | Verweis                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                           |
| ----- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 306   |  Certifying and Removing Disparate Impact  | Die Autoren definieren algorithmische Voreingenommenheit über das Prinzip des „disparate impact“, schlagen einen Test vor, der anhand der Vorhersagbarkeit geschützter Merkmale aus anderen Attributen diskriminierende Effekte ermittelt, beschreiben Verfahren zur Entbiasierung der Daten und untermauern ihre Methoden empirisch. |
| 296   |  Bias in der künstlichen Intelligenz       | Das Dokument Bias in der künstlichen Intelligenz befasst sich mit den Grundlagen und zeigt Detektion und Mitigationsmechanismen auf um Bias in den eigenen Datensätzen auf die Spur zu kommen.                                                                                                                                        |

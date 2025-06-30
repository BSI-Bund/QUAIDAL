---
Name: QM-44-6 Hot Deck Imputation
Title: QM-44-6 Hot Deck Imputation
TitleGer: QM-44-6 Hot Deck Imputation
shortdesc: Fehlende Werte mit ähnlichen Fällen ermitteln
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-6
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: 
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-6 Hot-Deck-Imputation

### Beschreibung

Die Hot-Deck-Imputation ist eine Methode der Daten-Imputation, die in der Statistik und Datenanalyse verwendet wird, um fehlende Werte in Datensätzen zu schätzen. Bei dieser Methode werden fehlende Werte durch Werte aus ähnlichen Fällen (auch bekannt als "Decks") im gleichen Datensatz ersetzt.

Der Begriff "Hot-Deck" stammt ursprünglich aus der Umfrageforschung, wo es darum geht, fehlende Antworten in Umfrageergebnissen zu behandeln. Die Idee ist im Fall fehlender Werte, einen ähnlichen Fall zu nutzen, um die fehlenden Werte zu ersetzen.

#### Sequentielle Hot-Deck-Imputation

Die **Sequential Hot-Deck-Imputation** ersetzt fehlende Werte durch Spenderwerte aus vorherigen, vollständig vorhandenen Beobachtungen im Datensatz, basierend auf einer logischen Reihenfolge (z. B. zeitlich). Diese Methode eignet sich besonders für geordnete Datensätze, wie Zeitreihen, kann aber verzerrt sein, wenn die Reihenfolge nicht sinnvoll ist.

#### Zufällige Hot-Deck-Imputation

Die **Zufällige Hot-Deck-Imputation** wählt für jede fehlende Beobachtung zufällig einen Spenderwert aus einer Gruppe ähnlicher, vollständiger Beobachtungen aus. Diese Methode ist einfach anzuwenden, kann aber zu hoher Variabilität in den imputierten Werten führen.

#### Nearest-Neighbor Hot-Deck-Imputation

Die **Nearest-Neighbor Hot Deck Imputation** ersetzt fehlende Werte durch den Wert einer Beobachtung, die der Zielbeobachtung in den ausgewählten Variablen am ähnlichsten ist, basierend auf Distanzmetriken wie der euklidischen Distanz. Diese Methode maximiert die Ähnlichkeit zwischen Spender und Zielbeobachtung, kann jedoch Verzerrungen verursachen, wenn es Unterschiede in nicht berücksichtigten Variablen gibt.

Zu den Vorteilen gehören die einfache Implementierung und die Berücksichtigung der Ähnlichkeit zwischen den Fällen. 

Zu den Nachteilen gehören die potenzielle Verzerrung der Ergebnisse, wenn die Ähnlichkeit zwischen den Fällen nicht angemessen berücksichtigt wird, sowie die Unsicherheit bei der Schätzung der fehlenden Werte. 

### Methode 

- **Fehlende Werte identifizieren**: Bestimme die Positionen der fehlenden Daten im Datensatz.
- **Relevante Variablen auswählen**: Wähle Variablen aus, die zur Bestimmung ähnlicher Beobachtungen dienen.
- **Ähnliche Beobachtungen gruppieren**: Gruppiere Beobachtungen mit ähnlichen Werten (z. B. mittels Clustering oder Matching).
- **Spender auswählen**: Bestimme für jede fehlende Beobachtung einen Spender, entweder zufällig oder basierend auf Ähnlichkeit.
- **Fehlende Werte imputieren**: Ersetze die fehlenden Werte durch die entsprechenden Spenderwerte.
- **Ergebnisse überprüfen**: Überprüfe den Datensatz auf Unstimmigkeiten oder Verzerrungen nach der Imputation.

### Sourcecode "Hot Deck Imputation"
| RefID | Verweis                              |
| ----- | ------------------------------------ |
| 42    | QM-44-6_Regression Imputation_python |
| 41    | QM-44-6_Hot Deck Imputation_python   |



### Referenzen
| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 83    |  A survey on missing data in machine learning                          | Der Text hebt die Bedeutung der korrekten Behandlung fehlender Werte im maschinellen Lernen hervor, da ignorierte Fehlwerte zu verzerrten Analysen führen können. Er bietet einen Überblick über bestehende Methoden, vergleicht zwei Ansätze (k-nächste Nachbarn und missForest) anhand von Experimenten auf dem Iris- und einem Fan-Datensatz mit 5–20% künstlichen Fehlwerten und zeigt erfolgreiche Imputationsergebnisse sowie zukünftige Forschungsrichtungen auf. |
| 84    |  Statistical Approaches for Epidemiology: From Concept to Application  | Dieses Lehrbuch vermittelt die grundlegenden Konzepte der Epidemiologie und bereitet den Leser gleichzeitig auf die Fähigkeiten vor, statistische Instrumente in realen Situationen anzuwenden.                                                                                                                                                                                                                                                                          |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können.                                                                                                                                                                                                                                                |
| 248   |  Multiple Imputation: A Review of Practical and Theoretical Findings   | Der Artikel gibt einen Überblick über Multiple Imputation zur Behandlung fehlender Daten, diskutiert theoretische Ergebnisse, verschiedene Strategien zur Generierung von Imputationen und vergleicht unterschiedliche Methoden, bevor es zukünftige Forschungsperspektiven aufzeigt.                                                                                                                                                                                    |

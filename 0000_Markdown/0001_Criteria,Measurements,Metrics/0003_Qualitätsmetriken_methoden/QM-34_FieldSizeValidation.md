---
Name: QM-34 Validierung der Feldgröße
Title: QM-34 Validierung der Feldgröße
TitleGer: QM-34 Validierung der Feldgröße
shortdesc: Textfelder und Variablen auf erwartete Länge überprüfen. Automatisiert/expertengesteuert.
tags:
  - Qualitätsmetrik
ID:
  - QM-34
ListMetricID: 
ListMeasureID:
  - "'MA-5'"
  - "'MA-4'"
  - "'MA-2'"
  - "'MA-05'"
  - "'MA-04'"
  - "'MA-02'"
  - "'MA-01'"
MID: "43"
CodeEx: true
share: true
lcstep: pre
type:
  - method
---
## QM-34 Validierung der Feldgröße

### Beschreibung

Überprüfung der Länge oder Größe von Textfeldern oder anderen Variablen, um sicherzustellen, dass sie innerhalb der erwarteten Grenzen liegen. Dies kann sicherstellen, dass keine ungewöhnlich langen oder kurzen Werte vorhanden sind, die möglicherweise auf Datenqualitätsprobleme hinweisen. Dies kann automatisiert oder per Expertenanalyse erfolgen. Die Metainformationen der Validierungsqualität macht eine Reihe von Kriterien relevant.

#### Kriterien für die Validierung

##### 1. Fehlerrate (Error Rate)

Misst den Prozentsatz der Fälle, in denen die Validierung fehlschlägt, weil die Daten die Feldgrößenanforderungen nicht erfüllen. Eine niedrige Fehlerrate deutet darauf hin, dass die meisten Daten korrekt validiert werden.

##### 2. Erfassungsrate (Capture Rate)

Die Erfassungsrate misst, wie gut das Validierungssystem fehlerhafte Eingaben erkennt und abfängt. Eine hohe Erfassungsrate bedeutet, dass das System effektiv unzulässige Daten, die die Feldgrößenbeschränkungen nicht einhalten, identifiziert.

##### 3. False Positive Rate

Gibt an, wie oft gültige Daten fälschlicherweise als ungültig markiert werden. Eine niedrige Rate an Falschpositiven ist wünschenswert, da sie darauf hinweist, dass korrekte Daten selten durch die Validierung abgelehnt werden.

##### 4. False Negative Rate

Misst die Häufigkeit, mit der ungültige Daten irrtümlich als gültig durchgelassen werden. Eine niedrige Rate an Falschnegativen zeigt an, dass das System effektiv darin ist, ungültige Daten zu erkennen und abzulehnen.

##### 5. Präzision und Recall

Präzision gibt den Anteil der korrekten positiven Vorhersagen im Verhältnis zu allen positiven Vorhersagen an. Hohe Präzision bedeutet, dass wenn eine Eingabe als ungültig markiert wird, sie wahrscheinlich tatsächlich ungültig ist. Recall (auch Sensitivität genannt) misst den Anteil der korrekt identifizierten positiven Fälle im Verhältnis zu allen tatsächlich positiven Fällen. Ein hoher Recall zeigt, dass das System effektiv darin ist, alle ungültigen Eingaben zu erkennen.

##### 6. F1-Score

Der F1-Score ist das harmonische Mittel von Präzision und Recall und bietet eine einzelne Metrik, die beide Aspekte ausbalanciert. Ein hoher F1-Score deutet darauf hin, dass das Validierungssystem sowohl präzise als auch sensitiv ist.

Diese Metriken zusammen bieten ein umfassendes Bild der Leistung der Field Size Validation. Die Auswahl der spezifischen Metriken hängt von den spezifischen Anforderungen und Zielen des jeweiligen Systems oder Projekts ab.


### Referenzen
| RefID | Verweis                               | Kurzbeschr.                                                                                                                                                              |
| ----- | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 218   |  False positives and false negatives  | Ein False Positive liegt vor, wenn ein Test fälschlich das Vorhandensein einer Bedingung signalisiert, ein False Negative, wenn er fälschlich deren Abwesenheit anzeigt; |

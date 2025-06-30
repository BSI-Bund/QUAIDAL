---
Name: QM-43 Kreuzabgleich
Title: QM-43 Kreuzabgleich
TitleGer: QM-43 Kreuzabgleich
shortdesc: Ergebnisprüfung durch Kreuzabgleich verschiedener Quellen.
tags:
  - Qualitätsmetrik
ID:
  - QM-43
ListMetricID: 
ListMeasureID:
  - "'MA-22'"
  - "'MA-06'"
  - "'MA-02'"
  - "'MA-07'"
MID: 
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-43 Quellenübergreifende Konsistenzprüfung

### Beschreibung

Zur Prüfung und Beurteilung der Vertrauenswürdigkeit einer Quelle sollte eine Abgleich zu alternativen Datenquellen gemacht werden. Für die Analyse von Daten sollten im Vorfeld Toleranzgrenzen definiert werden.

Quellenübergreifende Konsistenzprüfung ist ein Prozess, bei dem Daten aus verschiedenen Quellen miteinander verglichen werden, um Gemeinsamkeiten, Unterschiede oder mögliche Korrelationen zu identifizieren. Dieser Prozess wird auch verwendet, um die Genauigkeit von Daten zu überprüfen oder um Muster und Trends zu erkennen, die durch die Kombination verschiedener Datenquellen entstehen können.

### Methode

- Datenvorbereitung: Bereinigen und Standardisieren der Daten, um sie vergleichbar zu machen.
- Merkmalsauswahl: Auswahl relevanter Merkmale, die in beiden Datensätzen verglichen werden sollen.
- Vergleichsmethoden:
    - Direkter Abgleich: Verwendung eines gemeinsamen Schlüssels oder Merkmalvergleichs.
    - Fuzzy Matching: Identifikation ähnlicher, aber nicht identischer Einträge.
    - Statistische Methoden: Nutzung von Korrelation, Clustering oder Anomalieerkennung, um Muster zu erkennen.
- Analyse und Validierung: Identifizieren von Übereinstimmungen, Visualisieren der Ergebnisse und Überprüfen auf Richtigkeit


### Beispiel

Es liegen zwei Kundendatensätze aus unterschiedlichen Abteilungen eines Unternehmens vor, und es soll ermittelt werden, welche Kunden in beiden Datensätzen enthalten sind. Dazu könnten folgende Schritte durchgeführt werden:

- Die Kundendaten werden bereinigt und standardisiert (z.B. Namensformatierung, Angleichung der Adressen).
- Anschließend werden Kunden anhand identischer E-Mail-Adressen oder Telefonnummern zusammengeführt.
- Fuzzy-Matching-Verfahren kommen zum Einsatz, um ähnliche, aber nicht identische Namen zu identifizieren.
- Schließlich kann ein Clustering angewandt werden, um Kunden nach ähnlichen Attributen zu gruppieren.

### Referenzen
| RefID | Verweis                                                                                               | Kurzbeschr.                                                                                                                                                                                     |
| ----- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 293   |  A systematic literature review of cross-domain model consistency checking by model management tools  | Der Artikel untersucht, wie bestehende Modellmanagement-Tools die Konsistenz zwischen Modellen unterschiedlicher Domänen prüfen und zeigt dabei bestehende Schwächen und Forschungsbedarfe auf. |



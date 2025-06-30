---
Name: QM-22 Rekonstruktionsfehler
Title: QM-22 Rekonstruktionsfehler
TitleGer: QM-22 Rekonstruktionsfehler
shortdesc: Der Rekonstruktionsfehler misst den Unterschied zwischen den ursprünglichen Daten und den durch die (bspw.) PCA rekonstruierten Daten
tags:
  - Qualitätsmetrik
ID:
  - QM-22
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
  - "'QM-10'"
MID: "31"
type:
  - metrik
CodeEx: true
lcstep: pre
share: true
---
## QM-22 Rekonstruktionsfehler

### Beschreibung

Der Rekonstruktionsfehler misst den Unterschied zwischen den ursprünglichen Daten und den durch die, (bspw.) PCA, rekonstruierten Daten. Ein geringer Rekonstruktionsfehler deutet darauf hin, dass die Hauptkomponenten die Daten gut repräsentieren. Der Rekonstruktionsfehler wird über einen mittleren quadratischen Fehler ermittelt. 

### Methode

- **Dimensionsreduktion durchführen:** Die ursprünglichen Daten werden auf eine geringere Anzahl an Dimensionen reduziert, indem beispielsweise nur die Hauptkomponenten beibehalten werden, die den größten Anteil der Varianz erklären.
- **Datenrekonstruktion:** Aus den reduzierten Dimensionen werden die Daten in den ursprünglichen Raum zurückprojiziert, basierend auf den Hauptkomponenten.
- **Vergleich der rekonstruierten und originalen Daten:** Mittels des Vergleichs zwischen rekonstruierten und originalen Daten wird der Unterschied gemessen.
- **Bestimmung des Fehlers:** Der Durchschnitt des Unterschieds über alle Datenpunkte wird berechnet. Dieser Wert zeigt an, wie viel Information durch die Dimensionsreduktion verloren gegangen ist.
- **Interpretation:** Ein niedriger Rekonstruktionsfehler weist darauf hin, dass die reduzierte Darstellung die wesentliche Struktur der Daten gut beibehält, während ein hoher Fehler auf einen Verlust wichtiger Informationen hindeutet.


### Pythoncode "Rekonstruktionsfehler"
| RefID | Verweis                          |
| ----- | -------------------------------- |
| 23    | QM-22_ReconstructionError_python |


### Referenzen
| RefID | Verweis                   | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                    |
| ----- | ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 115   |  Hauptkomponentenanalyse  | Die Hauptkomponentenanalyse (HKA) ist ein Verfahren der multivariaten Statistik, das große Datensätze durch Eigenvektoren der Kovarianzmatrix vereinfacht, indem viele Variablen zu wenigen aussagekräftigen Hauptkomponenten zusammengefasst werden. Sie findet Anwendung unter anderem in der Signal- und Bildverarbeitung und ist von der Faktorenanalyse zu unterscheiden. |

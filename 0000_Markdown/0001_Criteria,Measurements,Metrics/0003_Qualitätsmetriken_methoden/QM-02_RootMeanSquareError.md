---
Name: QM-02 Mittlerer quadratischer Fehler
Title: QM-02 Mittlerer quadratischer Fehler
TitleGer: QM-02 Mittlerer quadratischer Fehler
shortdesc: Der Root Mean Square Error (RMSE) misst die durchschnittliche Abweichung zwischen vorhergesagten und tatsächlichen Werten.
tags:
  - Qualitätsmetrik
ID:
  - QM-02
ListMetricID: 
ListMeasureID:
  - MA-8
  - "'MA-27'"
  - "'MA-08'"
MID: "2"
type:
  - metric
CodeEx: true
share: true
lcstep: post
---
## QM-02 Mittlerer quadratischer Fehler

### Beschreibung

Der Root Mean Squared Error (RMSE) ist eine Metrik zur Bewertung der Genauigkeit eines Vorhersagemodells, ähnlich dem Mean Absolute Error (MAE), jedoch berücksichtigt der RMSE die quadratischen Abweichungen zwischen den tatsächlichen und den vorhergesagten Werten. 

Der RMSE ist eine nützliche Metrik, um die Genauigkeit eines Modells zu bewerten, insbesondere wenn größere Fehler stärker gewichtet werden sollen.


### Methode

- **Vorhersagen und tatsächliche Werte sammeln**:  Zuerst benötigt man eine Liste der tatsächlichen Werte (die "wahren" Ergebnisse) und eine Liste der vorhergesagten Werte, die das Modell berechnet hat. 
- **Fehler berechnen**:  Für jeden Punkt der beiden Listen berechnet man den Fehler, indem man die Differenz zwischen dem vorhergesagten Wert und dem tatsächlichen Wert ermittelt. Dies zeigt, wie stark sich die Vorhersage vom tatsächlichen Wert unterscheidet.
- **Fehler quadrieren**:  Um sicherzustellen, dass größere Fehler stärker gewichtet werden und um zu vermeiden, dass sich negative und positive Fehler gegenseitig aufheben, quadriert man jeden berechneten Fehler. 
- **Durchschnitt berechnen**:  Nachdem man die quadrierten Fehler für alle Werte in der Liste berechnet hat, bildet man den Durchschnitt dieser quadrierten Werte. Dies ergibt den mittleren quadratischen Fehler.


### Pythoncode für "RootMeanSquareError"
| RefID | Verweis                          |
| ----- | -------------------------------- |
| 2     | QM-02_RootMeanSquareError_python |



### Referenzen
| RefID | Verweis                                                              | Kurzbeschr.                                                                                                                                                                                                                                                  |
| ----- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 126   |  Statista - das Statistik-Portal: Statistiken, Marktdaten & Studien  | Statista ist eine Datenplattform, die Statistiken und Berichte aus verschiedenen Branchen und Märkten bereitstellt. Sie bietet Umfragen, Prognosen und Analysen zu Themen wie Wirtschaft, Gesellschaft und Technologie für Unternehmen, Forscher und Medien. |



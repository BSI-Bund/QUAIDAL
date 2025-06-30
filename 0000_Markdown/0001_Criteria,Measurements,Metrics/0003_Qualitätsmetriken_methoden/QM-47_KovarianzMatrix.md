---
Name: QM-47 Kovarianz Matrix
Title: QM-47 Kovarianz Matrix
TitleGer: QM-47 Kovarianz Matrix
shortdesc: Kovarianzmatrix misst Zusammenhänge zwischen Merkmalen; Diagonalen sind Varianzen, andere Werte Kovarianzen.
tags:
  - Qualitätsmetrik
ID:
  - QM-47
ListMetricID: 
ListMeasureID:
  - "'QM-10'"
MID: "64"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-47 Kovarianz-Matrix

### Beschreibung

Eine Kovarianzmatrix ist ein mathematisches Werkzeug, das in der Statistik und im maschinellen Lernen verwendet wird, um die Kovarianz zwischen Paaren von Merkmalen in einem Datensatz zu messen. Die Elemente der Matrix zeigen, wie stark die Änderungen eines Merkmals mit den Änderungen eines anderen Merkmals zusammenhängen. Jedes Element $sigma$ der Kovarianzmatrix repräsentiert die Kovarianz zwischen dem i-ten und dem j-ten Merkmal. Die Diagonale der Kovarianzmatrix enthält die Varianzen der einzelnen Merkmale, also die Kovarianz jedes Merkmals mit sich selbst. 

Diese Matrix wird oft genutzt, um die Datenstruktur zu verstehen und ist entscheidend für viele statistische Techniken und maschinelle Lernverfahren, insbesondere solche, die mit multivariaten Daten arbeiten.


### Methode 

- **Daten sammeln**: Zuerst benötigt man einen Datensatz mit mehreren Variablen. Jede Spalte im Datensatz repräsentiert eine Variable, und jede Zeile steht für eine Beobachtung oder Messung. Ein Beispiel wären Daten über Größe, Gewicht und Alter von Personen.
- **Durchschnitt berechnen**: Für jede Variable im Datensatz berechnet man den Durchschnittswert. Dies ist der Mittelwert aller Werte in einer Spalte.
- **Abweichungen bestimmen**: Anschließend berechnet man für jede Beobachtung, wie weit sie vom Durchschnitt abweicht. Man vergleicht also die einzelnen Werte mit dem zuvor ermittelten Mittelwert.
- **Zusammenhang untersuchen**: Nun betrachtet man für jede Kombination von Variablen, ob ein Zusammenhang besteht. Man prüft zum Beispiel, ob größere Personen auch schwerer sind, indem man die Abweichungen der Größe und des Gewichts für jede Beobachtung miteinander vergleicht.
- **Matrix aufbauen**: Die Ergebnisse dieser Vergleiche zwischen den Variablen werden in einer Matrix organisiert. Jede Zeile und Spalte in der Matrix entspricht einer der Variablen. Der Eintrag in der Matrix zeigt dann, wie stark zwei Variablen miteinander in Beziehung stehen.


### Pythoncode "Kovarianz-Matrix"
| RefID | Verweis                      |
| ----- | ---------------------------- |
| 46    | QM-47_KovarianzMatrix_python |



### Referenzen
| RefID | Verweis           | Kurzbeschr.                                                                                                                                                                                                  |
| ----- | ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 255   |  Kovarianzmatrix  | Die Kovarianzmatrix ist eine quadratische Matrix, die die Varianzen und Kovarianzen eines Zufallsvektors darstellt und zentrale Informationen über Streuung und lineare Zusammenhänge der Variablen liefert. |


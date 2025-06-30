---
Name: QM-55 Bestimmtheitsmaß
Title: QM-55 Bestimmtheitsmaß
TitleGer: QM-55 Bestimmtheitsmaß
shortdesc: welcher Anteil der Varianz (also der abhängigen Variablen) durch die die unabhängige Variablen erklärt werden kann.
tags:
  - Qualitätsmetrik
ID:
  - QM-55
ListMetricID: 
ListMeasureID:
  - "'QM-10'"
  - "'QM-19'"
MID: "96"
type:
  - metrik
lcstep: post
CodeEx: true
share: true
---
## QM-55 Bestimmtheitsmaß

### Beschreibung

Der $R^2$-Wert, häufig als Bestimmtheitsmaß (Coefficient of determination) bezeichnet, wird typischerweise im Kontext von Regressionsanalysen verwendet, um den **Anteil der Varianz in der abhängigen Variablen** zu quantifizieren, **der durch die unabhängigen Variablen im Modell erklärt wird**. Wichtig ist dabei die Art der Regression (bzw. der Abhängigkeit) im Blick zu behalten. Das Bestimmtheitsmaß ist nur für eine "lineare" Regression geeignet. 

Ein Beispiel für den Einsatz des Bestimmtheitsmaß findet sich in der Hauptkomponentenanalyse.
In der Hauptkomponentenanalyse (PCA) wird der Begriff $R^2$-Wert nicht auf die gleiche Weise verwendet, aber ein äquivalentes Konzept existiert in Form des Anteils der erklärten Varianz einer Komponente an der Gesamtvarianz. In der PCA wird der Anteil der durch eine bestimmte Hauptkomponente erklärten Varianz durch den entsprechenden Eigenwert dieser Komponente im Verhältnis zur Summe aller Eigenwerte ausgedrückt. (Siehe QM-19 Erklärte Varianz) Wenn mehrere Hauptkomponenten vorkommen, kann man den kumulativen Anteil der erklärten Varianz berechnen, indem man die Eigenwerte der ersten k Komponenten summiert und durch die Gesamtsumme aller Eigenwerte teilt.

### Formel

Form 1 -  empirisches Bestimmtheitsmaß: 

![Die Formel für R^2 berechnet den Anteil der Varianz der vorhergesagten Werte im Vergleich zur Gesamtvarianz der tatsächlichen Daten.](9999_Images/Bestimmtheitsma%C3%9F2.png)


Form 2 - Spezialfall mit Fit des Achsenabschnitts: 

![Die Formel für R quadrat vergleicht die Summe der quadratischen Abweichungen der Modellvorhersagen von den tatsächlichen Werten mit der Gesamtvarianz der Daten.](9999_Images/Bestimmtheitsma%C3%9F.png)

Hierbei ist:

- $y_i$​ ist der tatsächliche Wert der abhängigen Variable für die Beobachtung i,
- $hat y_i$​​ ist der vom Modell vorhergesagte Wert für die Beobachtung i,
- $bar y_i$​ ist der Durchschnitt aller tatsächlichen Werte der abhängigen Variable, und
- n ist die Anzahl der Beobachtungen.

Der Zähler dieser Formel, ist die Summe der quadrierten Residuen und misst die nicht erklärte Streuung (die Variabilität der abhängigen Variable, die nicht durch das Modell erklärt wird). Der Nenner, ist die totale Streuung (die gesamte Variabilität der abhängigen Variable) und wird auch als totale Summe der Quadrate bezeichnet.

Ein R²-Wert von 1 bedeutet, dass das Modell die abhängige Variable perfekt vorhersagt, während ein Wert von 0 bedeutet, dass das Modell die abhängige Variable nicht besser vorhersagt als das einfache Mittel der beobachteten Werte. R² kann auch negativ sein, wenn das Modell schlechter als das einfache Mittel ist, was jedoch auf Probleme mit dem Modell hinweist.


### Pythoncode "Coefficient of determination (PCA)"
| RefID | Verweis                                         |
| ----- | ----------------------------------------------- |
| 70    | QM-55_Coefficient of determination (PCA)_python |




### Referenzen
| RefID | Verweis                                      | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                         |
| ----- | -------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 82    |  A Tutorial on Principal Component Analysis  | Dieses Papier soll dazu beitragen, die „Blackbox“ der Hauptkomponentenanalyse (PCA) verständlich zu machen, indem es von einfachen Intuitionen bis hin zu den zugrundeliegenden mathematischen Prinzipien führt. Durch die Verbindung informeller Erklärungen mit mathematischen Herleitungen erhalten Leser aller Niveaus ein besseres Verständnis dafür, wann, wie und warum PCA eingesetzt wird. |
| 125   |  Bestimmtheitsmaß                            | Das Bestimmtheitsmaß beruht auf der Quadratsummenzerlegung, bei der die totale Quadratsumme in die durch das Regressionsmodell erklärte Quadratsumme einerseits und in die Residuenquadratsumme andererseits zerlegt wird.                                                                                                                                                                          |
| 176   |  Principal component analysis                | Die Hauptkomponentenanalyse (PCA) ist eine wichtige Technik der multivariaten Datenanalyse.                                                                                                                                                                                                                                                                                                         |


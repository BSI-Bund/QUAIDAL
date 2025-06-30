---
Name: QM-19 Erklärte Varianz
Title: QM-19 Erklärte Varianz
TitleGer: QM-19 Erklärte Varianz
shortdesc: Misst Modellgenauigkeit durch Anteil erklärter Variation der abhängigen Variablen. Werte zwischen 0 und 1.
tags:
  - Qualitätsmetrik
ID:
  - QM-19
ListMetricID: 
ListMeasureID:
  - "'QM-10'"
MID: "28"
type:
  - metric
CodeEx: true
lcstep: pre
share: true
---
## QM-19 Erklärte Varianz

### Beschreibung

Der Prozentsatz der erklärten Varianz ist eine zentrale Metrik bei der Bewertung der Effektivität einer Principal Component Analysis (PCA). Diese Metrik zeigt an, wie viel der Gesamtvarianz der ursprünglichen Daten durch die ersten n Hauptkomponenten erklärt wird. Je höher der Prozentsatz der erklärten Varianz, desto effektiver ist die PCA darin, die wesentlichen Informationen der Daten in einer reduzierten Anzahl von Dimensionen zu erfassen.

Im Detail bedeutet das Folgendes:

- Erklärte Varianz pro Hauptkomponente: Jede Hauptkomponente hat eine eigene erklärte Varianz, die angibt, wie viel Varianz dieser Komponente zu den Daten beiträgt.
- Kumulative erklärte Varianz: Die kumulative Summe der erklärten Varianz bis zu einer bestimmten Hauptkomponente zeigt an, wie viel der Gesamtvarianz durch alle vorhergehenden Komponenten zusammen erklärt wird. Dies ist besonders nützlich, um zu entscheiden, wie viele Hauptkomponenten beibehalten werden sollen.
- Effektivität der PCA: Wenn zum Beispiel die ersten zwei Hauptkomponenten 90 % der Gesamtvarianz erklären, bedeutet das, dass fast alle wichtigen Informationen der Daten in diesen zwei Dimensionen enthalten sind. Das ist ein Zeichen dafür, dass die PCA sehr effektiv ist.

In der Praxis wird oft ein Scree-Plot verwendet, der die erklärten Varianzanteile der Hauptkomponenten grafisch darstellt. Dies hilft, eine Entscheidung darüber zu treffen, wie viele Hauptkomponenten verwendet werden sollen, indem man den "Knick" im Diagramm sucht, wo zusätzliche Komponenten nur noch wenig zusätzliche Varianz erklären.


### Formel

![Formel der erklärten Varianz](../../../9999_Images/Erkl%C3%A4rte_Varianz.png)

Die Formel beschreibt die **erklärte Varianz** in einer Hauptkomponentenanalyse (Principal Component Analysis, PCA). Sie zeigt, wie viel der Gesamtvarianz in den Daten durch eine einzelne Hauptkomponente erklärt wird.

- $lambda_j$ für den Eigenwert der $j$-ten Hauptkomponente.
- $sum_(i=1)^n lambda_i$ für die Summe aller Eigenwerte, also die gesamte Varianz, die durch alle Hauptkomponenten erklärt wird.

Die erklärte Varianz gibt also an, welcher Anteil der gesamten Varianz durch die (j)-te Hauptkomponente erklärt wird. Dies ist ein wichtiges Maß, um zu entscheiden, wie viele Hauptkomponenten man auswählen sollte, um die wesentliche Struktur der Daten zu erfassen.


### Pythoncode "Explained Variance"

| RefID | Verweis                         |
| ----- | ------------------------------- |
| 21    | QM-19_Explained Variance_python |





### Referenzen

| RefID | Verweis                                                   | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                         |
| ----- | --------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 61    |  Hauptkomponentenanalyse und explorative Faktorenanalyse  | Der Beitrag führt in die Grundlagen der Hauptkomponentenanalyse (PCA) und explorativen Faktorenanalyse (EFA) ein.                                                                                                                                                                                                                                                                                   |
| 82    |  A Tutorial on Principal Component Analysis               | Dieses Papier soll dazu beitragen, die „Blackbox“ der Hauptkomponentenanalyse (PCA) verständlich zu machen, indem es von einfachen Intuitionen bis hin zu den zugrundeliegenden mathematischen Prinzipien führt. Durch die Verbindung informeller Erklärungen mit mathematischen Herleitungen erhalten Leser aller Niveaus ein besseres Verständnis dafür, wann, wie und warum PCA eingesetzt wird. |
| 115   |  Hauptkomponentenanalyse                                  | Die Hauptkomponentenanalyse (HKA) ist ein Verfahren der multivariaten Statistik, das große Datensätze durch Eigenvektoren der Kovarianzmatrix vereinfacht, indem viele Variablen zu wenigen aussagekräftigen Hauptkomponenten zusammengefasst werden. Sie findet Anwendung unter anderem in der Signal- und Bildverarbeitung und ist von der Faktorenanalyse zu unterscheiden.                      |
| 176   |  Principal component analysis                             | Die Hauptkomponentenanalyse (PCA) ist eine wichtige Technik der multivariaten Datenanalyse.                                                                                                                                                                                                                                                                                                         |
| 245   |  Varianz                                                  | Die Varianz misst in der Wahrscheinlichkeitsrechnung die Streuung reeller Werte um einen Mittelwert, berechnet als mittleres Abweichungsquadrat, und dient als Grundlage für weiterführende Analysen wie die Standardabweichung oder Varianzzerlegungen.                                                                                                                                            |

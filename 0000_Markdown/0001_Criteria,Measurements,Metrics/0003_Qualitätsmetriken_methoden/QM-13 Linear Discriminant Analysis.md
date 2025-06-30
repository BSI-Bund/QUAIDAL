---
Name: QM-13 Linear Discriminant Analysis
Title: QM-13 Linear Discriminant Analysis
TitleGer: QM-13 Lineare Diskriminanzanalyse
shortdesc: Die Lineare Diskriminanzanalyse (LDA) ist ein Verfahren zur Klassifikation, das lineare Trennlinien findet, um Datenpunkte anhand ihrer Merkmale optimal in vordefinierte Klassen zu unterteilen.
tags:
  - Qualitätsmetrik
ID:
  - QM-13
ListMetricID: 
ListMeasureID:
  - "'MA-12'"
MID: 
type:
  - method
lcstep: pre
share: true
CodeEx: true
---
## QM-13 Lineare Diskriminanzanalyse

### Beschreibung

Die Lineare Diskriminanzanalyse (LDA) ist eine Methode, um Daten in verschiedene Klassen zu unterteilen. Sie sucht nach den besten Trennlinien, die die Klassen voneinander unterscheiden, indem sie den Abstand zwischen den Klassen maximiert und die Streuung innerhalb der Klassen minimiert. LDA geht davon aus, dass die Daten normalverteilt sind und die Klassen ähnliche Streuungen haben. Sie wird oft zur Klassifikation verwendet, z. B. in der Gesichtserkennung oder medizinischen Diagnosen.

Die Principal-Component-Analysis (PCA) zielt darauf ab, die Varianz innerhalb der Daten zu maximieren, während die Lineare Diskriminanzanalyse (LDA) darauf abzielt, die Trennung zwischen den Klassen zu optimieren. 

### Methode

- Berechnung der Mittelwerte: Bestimme die Mittelwerte für jede Klasse und für den gesamten Datensatz.
- Berechnung der Streumatrizen: Berechne die _within-class_ Streumatrix (Streuung innerhalb der Klassen) und die _between-class_ Streumatrix (Streuung zwischen den Klassen).
- Berechnung der Eigenvektoren und Eigenwerte: Löse das Eigenwertproblem für die Streumatrizen, um die Eigenvektoren und Eigenwerte zu berechnen.
- Wahl der Eigenvektoren: Wähle die Eigenvektoren mit den größten Eigenwerten, um die Dimensionen zu reduzieren und eine optimale Trennungsfläche zu finden.
- Transformation der Daten: Projiziere die Originaldaten auf den neuen Raum, der durch die ausgewählten Eigenvektoren definiert ist.
- Klassifikation: Weise neue Datenpunkte der Klasse zu, deren Mittelwert im projizierten Raum am nächsten liegt.


### Sourcecode "Linear Discriminant Analysis"
| RefID | Verweis                                   |
| ----- | ----------------------------------------- |
| 16    | QM-13_Linear Discriminant Analysis_python |


### Referenzen
| RefID | Verweis                                                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ----- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 118   |  Diskriminanzanalyse                                             | Die Diskriminanzanalyse ist eine statistische Methode zur Unterscheidung von Gruppen anhand mehrerer Merkmale, dient als Klassifikator oder zur Dimensionsreduktion, und berücksichtigt im Gegensatz zur Hauptkomponentenanalyse die Klassenzugehörigkeit der Daten.                                                                                                                                                                                                                                   |
| 249   |  Linear discriminant analysis                                    | Die lineare Diskriminanzanalyse (LDA) ist eine statistische Methode zum Finden linearer Kombinationen von Merkmalen zur Unterscheidung zwischen Klassen. Sie wird häufig zur Dimensionsreduzierung und Klassifizierung verwendet, wobei normalverteilte unabhängige Variablen angenommen werden und der Schwerpunkt auf der Modellierung von Unterschieden zwischen vordefinierten Gruppen liegt.                                                                                                      |
| 263   |  Transfer learning via Regularized Linear Discriminant Analysis  | Die lineare Diskriminanzanalyse stößt bei hochdimensionalen Daten und kleinen Stichprobengrößen auf Probleme, die zu hohen Klassifikationsfehlern führen. Um dem entgegenzuwirken, wird ein neuartiger Transfer-Learning-Ansatz mit regularisierter Random-Effects-Diskriminanzanalyse vorgeschlagen, der Daten aus Ziel- und Quellmodellen kombiniert und durch optimierte Gewichtungsstrategien die Klassifikationsgenauigkeit verbessert, was theoretisch und durch numerische Studien belegt wird. |

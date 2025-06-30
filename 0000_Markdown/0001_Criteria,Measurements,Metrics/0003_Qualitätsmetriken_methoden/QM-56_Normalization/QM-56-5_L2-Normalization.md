---
Name: QM-56-5 L2-Normalisierung
Title: QM-56-5 L2-Normalisierung
TitleGer: QM-56-5 L2-Normalisierung
shortdesc: Die L2-Normalisierung skaliert Vektoren auf eine euklidische Norm von 1 und betont größere Abweichungen stärker als die L1-Normalisierung, was sie besonders für Anwendungen geeignet macht, bei denen die geometrische Beziehung zwischen Datenpunkten wichtig ist.
tags:
  - Qualitätsmetrik
  - Normalization
ID:
  - QM-56-5
ListMetricID: 
ListMeasureID:
  - "'MA-23'"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-56-5 L2-Normalisierung

### Beschreibung

Datenquellen liefern Merkmale in völlig unterschiedlichen Werte­bereichen (Pixel­intensität 0-255, Wortfrequenz-Counts....). L2-Normalisierung skaliert jeden Beobachtungs­vektor so, dass seine euklidische Länge **eins** ist; nur seine Richtung bleibt erhalten. Dadurch wird verhindert, dass große Betrags­werte allein wegen ihrer Skala die Distanz- oder Ähnlichkeits­messung dominieren.

Im Vergleich zur L1-Normalisierung, die jeden Vektor durch die Summe seiner Beträge skaliert, teilt die **L2-Normalisierung** durch die Quadratwurzel der Summe der quadrierten Werte. Beide Verfahren ändern lediglich die _Länge_, nicht aber die Richtung des Vektors. 

### Formel

Mathematisch betrachtet wird die L2-Norm eines Vektors $x=(x_1,x_2,…,x_n)$  berechnet, indem die Quadratwurzel der Summe der quadrierten Komponenten gezogen wird. Durch die Anwendung der L2-Normalisierung wird die Richtung des Vektors beibehalten, während seine Länge auf 1 reduziert wird. Dies ist besonders nützlich, wenn man mit Daten arbeitet, die auf unterschiedlichen Skalen liegen, da die Normalisierung sicherstellt, dass kein einzelner Wert die Analyse dominiert. In maschinellen Lernalgorithmen, wie zum Beispiel neuronalen Netzen oder k-Nearest-Neighbor, kann die L2-Normalisierung die Trainingszeit verkürzen und die Stabilität des Modells verbessern. Sie hilft auch dabei, Überanpassungen zu reduzieren, indem sie die Auswirkungen von Ausreißern minimiert, da größere Werte durch die Quadrierung in der Norm stärker gewichtet werden.

### Sourcecode "L2-Normalisierung"

| RefID | Verweis                         | Inhalt                      |
| ----- | ------------------------------- | --------------------------- |
| 76    | QM-56-5 L2-Normalization_python | L2 Normalisierung in Python |


### Referenzen

| RefID | Verweis                                                                        | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 180   |  The elements of statistical learning: data mining, inference, and prediction  | Dieses Buch bietet einen umfassenden Überblick über Schlüsselkonzepte des Data Mining in Bereichen wie Medizin und Finanzen und konzentriert sich dabei auf überwachtes und unüberwachtes Lernen. Es behandelt Themen wie neuronale Netze, Boosting und fügt neue Inhalte zu Random Forests, Ensemble-Methoden und dem Umgang mit „großen“ Daten hinzu. Es ist nützlich für Statistiker und diejenigen, die in der Wissenschaft oder Industrie tätig sind. |


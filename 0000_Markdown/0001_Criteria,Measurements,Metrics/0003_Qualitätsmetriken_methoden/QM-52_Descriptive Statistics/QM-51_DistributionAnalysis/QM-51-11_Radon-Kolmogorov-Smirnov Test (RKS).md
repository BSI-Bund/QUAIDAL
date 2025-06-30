---
Name: QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS)
Title: QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS)
TitleGer: QM-51-11 Radon-Kolmogorov-Smirnov Test (RKS)
shortdesc: Ausprägung des klassischen Kolmogorov Smirnow Tests auf höherdimensionalen Datensätzen.
tags:
  - Qualitätsmetrik
  - "#DA-Type"
  - DA-Type
ID:
  - QM-51-11
ListMetricID: 
ListMeasureID:
  - "'MA-9'"
  - "'MA-8'"
  - "'MA-08'"
  - "'MA-09'"
MID: 
type:
  - metrik
  - method
CodeEx: true
share: true
lcstep: pre
---
## QM-51-11 Radon-Kolmogorov-Smirnov-Test (RKS)

### Beschreibung

Der Radon-Kolmogorov-Smirnov-Test (RKS-Test) ist eine Erweiterung des klassischen Kolmogorov-Smirnov-Tests (KS-Test) auf höherdimensionale Daten, was ihn besonders nützlich für Anwendungen im maschinellen Lernen macht. 

Während der klassische KS-Test zwei eindimensionale Verteilungen vergleicht, zielt der RKS-Test darauf ab, Unterschiede zwischen Verteilungen in höheren Dimensionen zu identifizieren.

- **Höherdimensionale Daten**: Der klassische KS-Test vergleicht die maximale Differenz zwischen zwei kumulativen Verteilungsfunktionen. Der RKS-Test verallgemeinert diesen Ansatz, indem er die Differenzen entlang verschiedener Projektionen im mehrdimensionalen Raum berechnet. Dadurch eignet er sich besonders gut für maschinelle Lernmodelle, die in hochdimensionalen Daten arbeiten​

- **Verbindung zu neuronalen Netzen**: Der RKS-Test kann als Optimierungsproblem interpretiert werden, bei dem versucht wird, die maximale Diskrepanz zwischen den Mittelwerten der Projektionen zweier Verteilungen zu finden. Diese Art der Optimierung ähnelt der in neuronalen Netzen und erlaubt es, vorhandene Werkzeuge aus dem Bereich des Deep Learning zur Berechnung des RKS-Abstands zu nutzen​
    
- **Permutationstests zur Kalibrierung**: Um Fehler des ersten Typs (fälschlicherweise eine wahre Nullhypothese ablehnen) zu kontrollieren, verwendet der RKS-Test Permutationstests, um die Teststatistik zu kalibrieren, ähnlich wie bei anderen Tests für zwei Stichproben​
    
- **Glattheitsbeschränkungen**: Der RKS-Abstand wird in Bezug auf Funktionen mit Radon-beschränkter Variation definiert. Dies bedeutet, dass er eine gewisse Glattheit der Projektionen der Verteilung berücksichtigt, was für den Vergleich hochdimensionaler Daten entscheidend ist​

### Beispiele 

#### Beispiel 1 

Ein Unternehmen analysiert Kundenverhalten anhand von zwei Merkmalen: **Bestellwert (in Euro)** und **Zeit bis zur nächsten Bestellung (in Tagen)**. Es möchte prüfen, ob das aktuelle Kundenverhalten (basierend auf Stichprobendaten) noch mit der historischen Verteilung übereinstimmt.

- **Historische Daten**: Multivariate Normalverteilung mit bekannten Parametern.
- **Aktuelle Daten**: Stichprobe aus dem letzten Monat.

### Sourcecode "Radon-Kolmogorov-Smirnov Test (RKS)"

| RefID | Verweis                                |
| ----- | -------------------------------------- |
| 85    | QM-51-11_Radon Kolmogorov Smirnov Test |



### Referenzen

| RefID | Verweis                                                                             | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 107   |  Maximum Mean Discrepancy Meets Neural Networks: The Radon-Kolmogorov-Smirnov Test  | Maximum Mean Discrepancy (MMD) ist ein nichtparametrischer Zwei-Stichproben-Test, der den Mittelwertunterschied zwischen Proben aus zwei Verteilungen maximiert, wobei alle Transformationen in einem Funktionsraum berücksichtigt werden, und wird durch den Radon-Kolmogorow-Smirnow (RKS)-Test generalisiert, der in mehreren Dimensionen und höheren Glattheitsgraden arbeitet und mit neuronalen Netzwerken verbunden ist, wobei die Funktion, die den maximalen Unterschied erzielt, immer ein Ridge-Spline ist, der als einzelnes Neuron in einem Netzwerk dargestellt werden kann. |

---
Name: QM-61-1 Marginal Contribution Approach
Title: QM-61-1 Marginal Contribution Approach
TitleGer: QM-61-1 Marginal Contribution Approach
shortdesc: Bewertung des Datenbeitrags in Modellen.
tags:
  - Qualitätsmetrik
  - "#ML-Data-Valuation"
  - ML-Data-Valuation
ID:
  - QM-61-1
ListMetricID: 
ListMeasureID:
  - "'QM-61'"
  - "'MA-14'"
  - "'MA-15'"
MID: 
type:
  - method
lcstep: post
CodeEx: true
share: true
---
## QM-61-1 Marginal Contribution Importance

### Beschreibung

Der Marginal Contribution Importance (MCI) ist ein Ansatz zur Bewertung des Beitrags einzelner Datenpunkte oder Datensätze zur Gesamtleistung eines Modells oder einer Anwendung. Dieser Ansatz ist besonders nützlich im Kontext von Machine Learning und Datenanalyse, wo die Bewertung der Bedeutung von Daten für das Modelltraining oder die Anwendungsleistung entscheidend ist.

Im MCI wird der Beitrag eines Datenpunktes durch das Hinzufügen oder Entfernen aus einem Modell oder einem System gemessen. Dieser Beitrag wird als marginale Verbesserung oder Verschlechterung der Leistung des Modells oder der Anwendung bewertet.


### Methode

Der Prozess zur Bestimmung des marginalen Beitrags eines Datenpunktes kann je nach Anwendung und Modell variieren. Im Allgemeinen umfasst es jedoch die folgenden Schritte:

- Trainingsphase: Das Modell wird unter Verwendung eines Datensatzes trainiert, der alle verfügbaren Datenpunkte enthält.
- Evaluation der Leistung: Die Leistung des Modells wird anhand eines bestimmten Leistungsmaßes bewertet, z. B. Genauigkeit, Fehler oder eine andere Metrik, die für die spezifische Anwendung relevant ist.
- Hinzufügen oder Entfernen von Daten: Ein einzelner Datenpunkt wird dem Trainingsdatensatz hinzugefügt oder daraus entfernt, und das Modell wird erneut trainiert.
- Vergleich der Leistung: Die Leistung des Modells nach Hinzufügen oder Entfernen des Datenpunktes wird mit der Leistung des ursprünglichen Modells verglichen. Die Differenz in der Leistung wird als marginaler Beitrag des Datenpunktes betrachtet.

Der MCI kann iterativ angewendet werden, um die marginalen Beiträge aller Datenpunkte im Datensatz zu bewerten. Auf diese Weise können Datenpunkte identifiziert werden, die einen signifikanten Einfluss auf die Modellleistung haben und daher für das Training oder die Anwendung von größerer Bedeutung sind.

Dieser Ansatz ermöglicht eine feinere Bewertung der Daten und kann verwendet werden, um Datenpunkte mit hoher oder niedriger Bedeutung zu identifizieren, was für verschiedene Anwendungen wie Feature Selection, Data Cleansing oder Modellinterpretation von Nutzen sein kann.

### Sourcecode "Marginal Contribution Importance"
| RefID | Verweis                                         | Inhalt                                              |
| ----- | ----------------------------------------------- | --------------------------------------------------- |
| 82    | QM-61-1_Marginal Contribution Importance_python | Beispiel - MCI auf dem California Housing Datensatz |




### Referenzen
| RefID | Verweis                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                |
| ----- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 291   |  Interpretable Machine Learning  | Das Buch Interpretable Machine Learning – A Guide for Making Black Box Models Explainable von Christoph Molnar bietet einen umfassenden Überblick über theoretische und praxisnahe Methoden zur Erklärung und Interpretation von Black-Box-Modellen im Machine Learning, um deren Verhalten transparenter und nachvollziehbarer zu machen. |


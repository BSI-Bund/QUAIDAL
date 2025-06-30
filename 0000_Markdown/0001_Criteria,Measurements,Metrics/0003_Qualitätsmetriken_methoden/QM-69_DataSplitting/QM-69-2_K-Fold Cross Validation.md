---
Name: QM-69-2 K-Fold Cross Validation
Title: QM-69-2 K-Fold Cross Validation
TitleGer: QM-69-2 K-Fold Cross Validation
shortdesc: Der Datensatz wird in K Folds aufgeteilt, sodass in K Durchgängen jeweils ein Fold testet und die restlichen trainieren.
tags:
  - Qualitätsmetrik
ID:
  - QM-69-2
ListMetricID: 
ListMeasureID:
  - "'MA-29'"
MID: 
type:
  - method
CodeEx: false
share: true
lcstep: pre
---
## QM-69-2 K-Fold-Cross Validation

### Beschreibung

K-Fold Cross Validation ist ein weit verbreitetes Verfahren zur Bewertung und Validierung von Machine-Learning-Modellen. Es dient dazu, die Leistungsfähigkeit eines Modells zuverlässig zu schätzen, indem der Datensatz in mehrere Teilmengen (Folds) aufgeteilt und in iterativen Trainings- und Testphasen verwendet wird.

### Methode

- **Datensatzaufteilung:**  
    Der gesamte Datensatz wird zufällig in k gleich große oder nahezu gleich große Teile (Folds) unterteilt.
- **Iterativer Trainings- und Testprozess:**
    - In jedem der k Durchläufe wird ein einzelner Fold als Testdatensatz gewählt.
    - Die verbleibenden k−1 Folds dienen als Trainingsdatensatz, auf dem das Modell trainiert wird.
    - Dieser Vorgang wird so oft wiederholt, bis jeder Fold einmal als Testdatensatz verwendet wurde.
- **Leistungsmessung:**  
    In jeder Iteration wird ein Leistungsmaß (z. B. Genauigkeit, F1-Score, Mean Squared Error etc.) berechnet. Somit erhält man k Leistungswerte, die die Modellgüte in unterschiedlichen Aufteilungen widerspiegeln.
- **Aggregation der Ergebnisse:**  
    Die einzelnen Metriken aus den k Durchläufen werden gemittelt, um eine stabile und verlässliche Schätzung der Generalisierungsfähigkeit des Modells zu erhalten.

### Sourcecode "K-Fold Cross Validation"
| RefID | Verweis                                |
| ----- | -------------------------------------- |
| 93    | QM-69-2_K-Fold Cross Validation_python |



### Referenzen
| RefID | Verweis                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                           |
| ----- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 304   |  Training, validation, and test data sets  | Beim maschinellen Lernen wird ein Modell typischerweise anhand eines Trainingsdatensatzes gelernt, mit einem Validierungsdatensatz zur Feinabstimmung der Hyperparameter optimiert und schließlich mit einem unabhängigen Testdatensatz (oft als Holdout bezeichnet) objektiv bewertet, wobei die genaue Aufteilung stark vom Anwendungsfall abhängt. |
| 286   |  KFold — scikit-learn 1.6.1 documentation  | K-Fold Cross Validation ist ein weit verbreitetes Verfahren zur Bewertung und Validierung von Machine-Learning-Modellen                                                                                                                                                                                                                               |


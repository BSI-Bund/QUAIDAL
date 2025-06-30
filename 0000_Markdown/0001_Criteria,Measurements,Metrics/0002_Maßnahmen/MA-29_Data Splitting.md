---
Name: MA-29_Data Splitting
Title: MA-29 Data Splitting
TitleGer: MA-29 Data-Splitting
shortdesc: Data-Splitting beschreibt die Strategien zur Aufteilung von Trainingsdatensätzen.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-29
ListMetricID: 
ListMeasureID:
  - "'QB-13'"
MID: 
share: true
---
## MA-29 Data Splitting

### Beschreibung

Data Splitting beschreibt verschiedene Methoden zur Aufteilung und Validierung von Datensätzen. Beim klassischen Hold-out-Verfahren wird der Gesamt-Datensatz typischerweise in 
- ein Trainingsset (70–80%), 
- ein Validierungsset (10–15%) und 
- ein Testset (10–15%) 

unterteilt, sodass das Modell zunächst auf dem Trainingsset lernt, dann anhand des Validierungssets Hyperparameter optimiert werden und abschließend das Testset für eine unverfälschte Leistungsbewertung dient. Zudem gibt es moderne Ansätze wie die K-Fold-Cross-Validation, bei der der Datensatz in k gleich große Teile geteilt wird und in k Wiederholungen jeweils ein anderer Teil als Testset verwendet wird, um robustere und stabilere Schätzungen der Modellgüte zu erzielen.



### Beispiele 

#### Beispiel 1 – Klassisches Hold-out-Verfahren:  

Gegeben sei einen Datensatz mit 10000 Bildern für ein Bildklassifikationsproblem. Dieser wird in drei Teile aufgeteilt:

- **Training (70%):** 7000 Bilder werden genutzt, um ein Convolutional Neural Network (CNN) zu trainieren.
    
- **Validierung (15%):** 1500 Bilder dienen dazu, während des Trainings die Hyperparameter (wie Lernrate oder Anzahl der Schichten) abzustimmen und Überanpassung zu vermeiden.
    
- **Test (15%):** 1500 Bilder, die das Modell während des Trainings und der Validierung nie gesehen hat, werden verwendet, um die finale Leistungsfähigkeit zu evaluieren.
    

#### Beispiel 2 – K-Fold-Cross-Validation:

Ein Unternehmen arbeitet an einem Spam-Erkennungsmodell und haben einen Datensatz mit 20000 E-Mails. Es wird das (K=5) "5"-Fold-Cross-Validation Verfahren angewendet, bei der der Datensatz wie folgt aufgeteilt wird:

- Der Datensatz wird in 5 gleich große Teile (Folds) zu je 4000 E-Mails unterteilt.
    
- In jeder der 5 Iterationen wird ein Fold als Testset genutzt, während die verbleibenden 4 Folds (insgesamt 16000 E-Mails) zum Trainieren und Validieren des Modells verwendet werden.
    
- Am Ende werden die Ergebnisse der 5 Testläufe gemittelt, um eine robuste Schätzung der Modellgüte zu erhalten.


### Metriken & Methoden

| ID                              | Kurzbeschr.                                                                                                                                                                                                 |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-69-1_Hold Out                | Beim Hold-out-Verfahren wird der Datensatz einmalig in Trainings-, Test- und optional Validierungsanteile aufgeteilt, um Modellbildung, Hyperparameteroptimierung und objektive Evaluation klar zu trennen. |
| QM-69-2 K-Fold Cross Validation | Der Datensatz wird in K Folds aufgeteilt, sodass in K Durchgängen jeweils ein Fold testet und die restlichen trainieren.                                                                                    |



### Referenzen

| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                             |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 100   |  An Introduction to Statistical Learning: with Applications in Python  | Präsentiert im wesentlichen ein statistisches Lernwerkzeug für Praktiker in Wissenschaft, Industrie und anderen Bereichen. Demonstriert die Anwendung der statistischen Lernmethoden in Python. Behandelt Regression, Klassifizierung, Baummethoden, SVM, Clustering, Überlebensanalyse, Deep Learning. |

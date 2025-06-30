---
Name: QM-25-1_Variance-Treshold
Title: QM-25-1 Variance-Treshold
TitleGer: QM-25-1 Variance-Treshold
shortdesc: Merkmale mit einer Varianz unter einem bestimmten Schwellenwert (Threshold) werden aus dem Datensatz entfernt.
tags:
  - Qualitätsmetrik
  - ML-FeatureImpScore
ID:
  - QM-25-1
ListMetricID: 
ListMeasureID:
  - "'MA-24'"
MID: 
type:
  - metrik
  - method
share: true
CodeEx: true
lcstep: pre
---
## QM-25-1 Variance-Treshold

### Beschreibung

Beim Variance Threshold-Verfahren wird für jedes Merkmal die Varianz berechnet, und Merkmale mit einer Varianz unter einem bestimmten Schwellenwert (Threshold) werden aus dem Datensatz entfernt. Der Gedanke dahinter ist, dass Merkmale, die wenig variieren, wenig zur Unterscheidung der Zielvariable beitragen, da sie für nahezu alle Datenpunkte denselben Wert annehmen. In Extremfällen sind diese Merkmale konstant, und somit für die Modellierung irrelevant, da sie keine Variabilität in den Daten darstellen.

### Beispiel 

Ursprünglicher Datensatz: Enthält vier Merkmale.
- Feature_1: Hat eine konstante Varianz (kein Unterschied in den Werten).
- Feature_2: Hat eine geringe Varianz.
- Feature_3: Hat eine hohe Varianz.
- Feature_4: Hat eine moderate Varianz.
    
- Nach Anwendung des Schwellenwerts (Treshold = 1.0):
    - Nur Feature_3 wurde beibehalten, da es die einzige Spalte ist, deren Varianz über dem Schwellenwert von 1.0 liegt.

Dieses Beispiel zeigt, wie Merkmale mit geringer Varianz aus einem Datensatz entfernt werden können, um irrelevante oder redundante Informationen zu reduzieren. Dies hilft, das Modell effizienter zu machen und sich auf aussagekräftigere Merkmale zu konzentrieren.


### Referenzen

| RefID | Verweis                                  | Kurzbeschr.                                                                                                                                                                                                   |
| ----- | ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 262   |  Feature Selection - Variance Threshold  | Das Variance Threshold-Verfahren filtert Merkmale mit geringer Varianz aus einem Datensatz, da sie wenig zur Unterscheidung der Zielvariable beitragen und somit für die Modellierung irrelevant sein können. |

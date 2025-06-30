---
Name: QM-06 Recall
Title: QM-06 Recall
TitleGer: QM-06 Recall
shortdesc: Anteil wahrer Positiver an allen tatsächlichen Positiven.
tags:
  - Qualitätsmetrik
ID:
  - QM-06
ListMetricID: 
ListMeasureID:
  - "'MA-27'"
MID: "6"
type:
  - metric
CodeEx: true
share: true
lcstep: post
---
## QM-06_Recall

### Beschreibung

Recall ist eine Metrik, die im maschinellen Lernen verwendet wird, um zu messen, wie gut ein Modell alle tatsächlich positiven Fälle aus den Daten erkennt. Sie wird definiert als der Anteil der korrekt identifizierten positiven Fälle (True Positives) an der Gesamtzahl der tatsächlichen positiven Fälle (True Positives plus False Negatives). Recall ist besonders wichtig in Situationen, in denen das Übersehen von positiven Fällen hohe Kosten oder Risiken verursacht, wie beispielsweise bei der Krankheitsdiagnose. Mitunter wird Recall auch als Sensitivität, Treffergenauigkeit oder Empfindlichkeit bezeichnet.


### Formel

- Alle echten positiven Fälle werden betrachtet. Das sind alle Fälle, die tatsächlich „positiv“ sind (zum Beispiel kranke Personen).
- Es wird ermittelt, welche dieser echten positiven Fälle vom Modell ebenfalls als positiv erkannt wurden. Dies sind die Fälle, bei denen das Modell korrekt lag und angab: „Ja, diese Person ist krank.“
- Der Recall ist das Verhältnis zwischen den positiv identifizierten Fällen und allen tatsächlich vorhandenen positiven Fällen. Er gibt an, wie viele der relevanten Fälle das Modell korrekt gefunden hat.


### Python Code für "Recall"
| RefID | Verweis             |
| ----- | ------------------- |
| 6     | QM-06_Recall_python |



### Referenzen
| RefID | Verweis                                                                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                  |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 121   |  Precision and recall                                                                                                                 | Präzision und Recall sind Leistungskennzahlen in der Mustererkennung und Klassifikation, wobei Präzision den Anteil relevanter Instanzen unter den abgerufenen misst und Recall den Anteil relevanter Instanzen, die korrekt identifiziert wurden, wobei der F1-Score als ausgewogenes Maß beide kombiniert. |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance  | Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                                                                                                                                                                 |

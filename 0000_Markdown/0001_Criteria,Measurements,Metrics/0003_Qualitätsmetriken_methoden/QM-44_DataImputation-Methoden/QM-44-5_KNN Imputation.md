---
Name: QM-44-5 KNN Imputation
Title: QM-44-5 KNN Imputation
TitleGer: QM-44-5 KNN Imputation
shortdesc: K-Nearest Neighbors ersetzt fehlende Daten mit Werten nächster Nachbarn.
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-5
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "58"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-5 K-NN-Imputation

### Beschreibung

K-NN (K-Nearest Neighbors) ersetzt fehlende Werte, indem es die ähnlichsten Beobachtungen (d. h. die nächsten Nachbarn) findet und deren Werte verwendet, um eine Vervollständigung durchzuführen.

Es eignet sich besonders gut für Datensätze, bei denen es klare Ähnlichkeiten zwischen den Datenpunkten gibt und bei welchen einfachen Methoden wie Mittelwert- oder Median-Imputation zu ungenauen Ergebnissen führen würden.


### Methode

- **Identifizieren der fehlenden Werte**: Zuerst wird festgestellt, welche Einträge im Datensatz fehlen (z. B. fehlende numerische oder kategoriale Werte in bestimmten Spalten).
    
- **Berechnung der Distanzen**: Für jede Instanz mit fehlenden Werten wird der K-NN-Algorithmus verwendet, um die **Distanzen zwischen dieser Instanz und allen anderen Instanzen** mit vollständigen Werten zu berechnen. Die Distanz kann beispielsweise mit der **euklidischen Distanz** für numerische Daten oder anderen Metriken für kategoriale Daten berechnet werden.
    
- **Auswahl der K nächsten Nachbarn**: Es werden die **K nächstgelegenen Datenpunkte** (basierend auf der Distanzmetrik) ausgewählt, die vollständige Werte haben.
    
- **Imputation der fehlenden Werte**:
    
    - **Für numerische Werte**: Der fehlende Wert wird durch den **Durchschnitt der K nächsten Nachbarn** ersetzt.
    - **Für kategoriale Werte**: Der fehlende Wert wird durch die **am häufigsten vorkommende Kategorie** unter den K nächsten Nachbarn ersetzt (Mode).
- **Wiederholung**: Dieser Prozess wird für jede Instanz mit fehlenden Werten wiederholt.

### Sourcecode "KNN Imputation"
| RefID | Verweis                       |
| ----- | ----------------------------- |
| 40    | QM-44-5_KNN Imputation_python |


### Referenzen
| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                               |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können. |

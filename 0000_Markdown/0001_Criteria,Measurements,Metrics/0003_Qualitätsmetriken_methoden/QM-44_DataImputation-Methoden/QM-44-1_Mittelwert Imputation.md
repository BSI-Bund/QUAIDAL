---
Name: QM-44-1 Mittelwert Imputation
Title: QM-44-1 Mittelwert Imputation
TitleGer: QM-44-1 Mittelwert Imputation
shortdesc: Ersetzung fehlender Werte durch den Mittelwert der beobachteten Werte der entsprechenden Variablen.
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-1
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "54"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-1 Mittelwert-Imputation

### Beschreibung

Mittelwert-Imputation ersetzt fehlender Werte durch den Mittelwert der beobachteten Werte der entsprechenden Variablen. Aufgrund der Berechnungsvorschrift des Mittelwertes können jedoch mitunter größere Fehler erzeugt werden, da der "wahre" Wert der entsprechenden Variable stark vom imputierten Wert abweichen kann. Die Nachteile dieser Methode sind die fehlende Betrachtung der Varianz. 


### Sourcecode "Mittelwert Imputation"

| RefID | Verweis                              |
| ----- | ------------------------------------ |
| 36    | QM-44-1_Mittelwert Imputation_python |


### Referenzen

| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                               |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 84    |  Statistical Approaches for Epidemiology: From Concept to Application  | Dieses Lehrbuch vermittelt die grundlegenden Konzepte der Epidemiologie und bereitet den Leser gleichzeitig auf die Fähigkeiten vor, statistische Instrumente in realen Situationen anzuwenden.                           |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können. |

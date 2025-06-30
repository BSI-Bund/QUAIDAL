---
Name: QM-44-2 Median Imputation
Title: QM-44-2 Median Imputation
TitleGer: QM-44-2 Median Imputation
shortdesc: Ersetzen fehlender Werte durch den Median der beobachteten Werte.
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-2
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "55"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-2 Median-Imputation

### Beschreibung

Die Median-Imputation ersetzt fehlende Werte durch den Median der beobachteten Werte. Im Gegensatz zur Mittelwert-Imputation ist der Median robuster gegen Ausreißer, was eine stabilere Wertegenerierung erlaubt. Auch hier wird der Einfluss der Varianz auf die imputierten Werte vernachlässigt und kann zu entsprechenden Fehlern bei den erzeugten Werten führen. Für kategoriale Werte ist diese Art der Imputation nicht durchführbar. 

### Sourcecode "Median Imputation"
| RefID | Verweis                          |
| ----- | -------------------------------- |
| 37    | QM-44-2_Median Imputation_python |



### Referenzen
| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                               |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 84    |  Statistical Approaches for Epidemiology: From Concept to Application  | Dieses Lehrbuch vermittelt die grundlegenden Konzepte der Epidemiologie und bereitet den Leser gleichzeitig auf die Fähigkeiten vor, statistische Instrumente in realen Situationen anzuwenden.                           |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können. |



---
Name: QM-44-8 Regression Imputation
Title: QM-44-8 Regression Imputation
TitleGer: QM-44-8 Regression Imputation
shortdesc: Regressionsmodelle sagen fehlende Werte durch Variablenbeziehungen vorher.
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-8
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "60"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-8 Regression-Imputation

### Beschreibung

Regression Imputation ist eine Methode zur Schätzung fehlender Werte in einem Datensatz. Indem eine Regressionsanalyse verwendet wird, werden die fehlenden Werte basierend auf den verfügbaren Daten prognostiziert. Dabei werden die vorhandenen Variablen als Prädiktoren verwendet, um den Wert der fehlenden Variable zu schätzen. Diese Methode kann sowohl einfache lineare Regression als auch fortgeschrittenere Techniken wie multiple lineare Regression oder logistische Regression umfassen.

### Methode

- **Identifikation der fehlenden Werte**: Zunächst werden die fehlenden Werte im Datensatz identifiziert. Die fehlenden Werte können in numerischen oder kategorialen Variablen vorkommen.
- **Auswahl der erklärenden Variablen**: Um die fehlenden Werte zu schätzen, werden Variablen aus dem Datensatz ausgewählt, die stark mit der Variable, in der Werte fehlen, korreliert sind. Diese Variablen fungieren als Prädiktoren (erklärende Variablen).
- **Erstellung eines Regressionsmodells**: Basierend auf den beobachteten Werten der Zielvariable (die Variable, in der Werte fehlen) und den Prädiktorvariablen wird ein Regressionsmodell erstellt. Dies kann ein lineares Modell sein (bei numerischen Variablen) oder ein logistisches Modell (bei kategorialen Variablen).
- **Vorhersage der fehlenden Werte**: Das erstellte Regressionsmodell wird verwendet, um die fehlenden Werte zu schätzen. Die geschätzten Werte basieren auf den Beziehungen zwischen den Prädiktorvariablen und der Zielvariablen.
- **Einfügen der geschätzten Werte**: Die fehlenden Werte im Datensatz werden durch die geschätzten Werte ersetzt.
- **Verifizierung und Anpassung**: Nach der Imputation wird überprüft, ob die geschätzten Werte sinnvoll erscheinen und ob die Verteilung der Daten konsistent bleibt. In manchen Fällen wird ein zusätzliches Verfahren, wie die multiple Imputation, verwendet, um Unsicherheiten in den Schätzungen besser zu berücksichtigen.

### Sourcecode "Regression Imputation"
| RefID | Verweis                              |
| ----- | ------------------------------------ |
| 44    | QM-44-8_Regression Imputation_python |


### Referenzen
| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                               |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können. |

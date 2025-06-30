---
Name: QM-54-3_SHAP-Force-Plot
Title: QM-54-3 SHAP-Force-Plot
TitleGer: QM-54-3 SHAP-Force-Plot
shortdesc: Visualisiert Auswirkungen von Merkmalen auf das Modell
tags:
  - Qualitätsmetrik
  - ChartTypes
ID:
  - QM-54-3
ListMetricID: 
ListMeasureID:
  - "'MA-14'"
MID: "94"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-54-3 SHAP-Force-Plot

### Beschreibung
  
Der SHAP(SHapley Additive exPlanations)-Force-Plot ist ein Visualisierungswerkzeug, das innerhalb des SHAP-Frameworks verwendet wird, um die Auswirkungen einzelner Merkmale auf die Vorhersage eines maschinellen Lernmodells zu erklären. Es hilft zu verstehen, wie die Werte jedes Features zur Gesamtvorhersage beitragen, basierend auf den Konzepten aus der kooperativen Spieltheorie, insbesondere den Shapley-Werten. Die unterschiedlichen Abschnitte des Plots geben jeweils den Anteil an der Entscheidungsfindung wieder. 

![Beispiel für einen SHAP-Force-Plot auf dem Titanic Datensatz](../../../../../9999_Images/SHAPFPl-Classi-Titanic.png)

### Sourcecode "SHAP-Force-Plot"

| RefID | Verweis                          | Inhalt                                                  |
| ----- | -------------------------------- | ------------------------------------------------------- |
| 69    | QM-54-3_SHAP-Force-Plot_python   | Klassifikationsbeispiel - Titanic Datensatz             |
| 68    | QM-54-3_SHAP-Force-Plot_2_python | Regressionsbeispiel - "Kaggle Housing Prices" Datensatz |


### Referenzen

| RefID | Verweis                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                |
| ----- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 291   |  Interpretable Machine Learning  | Das Buch Interpretable Machine Learning – A Guide for Making Black Box Models Explainable von Christoph Molnar bietet einen umfassenden Überblick über theoretische und praxisnahe Methoden zur Erklärung und Interpretation von Black-Box-Modellen im Machine Learning, um deren Verhalten transparenter und nachvollziehbarer zu machen. |


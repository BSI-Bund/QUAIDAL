---
Name: QM-27 Permutation Feature Importance
Title: QM-27 Permutation Feature Importance
TitleGer: QM-27 Permutation Feature Importance
shortdesc: Methode zur Bestimmung der Bedeutung von Merkmalen
tags:
  - Qualitätsmetrik
  - ML-FeatureImpScore
ID:
  - QM-27
ListMetricID: 
ListMeasureID:
  - "'MA-12'"
  - "'MA-14'"
  - "'QM-10'"
MID: "36"
lcstep: post
CodeEx: true
share: true
type:
  - metrik
---
## QM-27 Permutation Feature Importance

### Beschreibung

Permutation Feature Importance ist eine Modellinspektions-Technik, die den Beitrag jedes Merkmals zur statistischen Leistung eines angepassten Modells auf einem gegebenen tabellarischen Datensatz misst.

### Methode

- Trainiere das Modell: Trainiere ein Modell mit den Trainingsdaten und den Merkmalen, um die Hauspreise vorherzusagen.
- Grundlage Vorhersagefehler berechnen: Berechne den Vorhersagefehler (z. B. mittlere quadratische Abweichung, Mean Squared Error, MSE) auf einem separaten Testdatensatz mit den echten Merkmalswerten.
- Permutation eines Merkmals: Wähle ein Merkmal, z. B. die "Wohnfläche", und permutiere (durchmische) die Werte dieses Merkmals im Testdatensatz. Dies zerstört den Zusammenhang zwischen der "Wohnfläche" und dem Zielwert (Hauspreis).
- Berechne den permutierten Vorhersagefehler: Verwende das trainierte Modell, um Vorhersagen mit dem permutierten Testdatensatz zu machen, und berechne erneut den Vorhersagefehler.
- Bedeutung des Merkmals bestimmen: Die Differenz zwischen dem ursprünglichen Vorhersagefehler und dem permutierten Vorhersagefehler zeigt die Bedeutung des Merkmals "Wohnfläche". Je größer die Differenz, desto wichtiger ist das Merkmal.
- Wiederhole dies für alle Merkmale: Wiederhole die Schritte 3 bis 5 für jedes der anderen Merkmale ("Anzahl der Zimmer", "Alter des Hauses"), um ihre relative Bedeutung zu bestimmen.

Je größer der Unterschied, desto wichtiger ist das Feature. Manchmal wird dieser Wert normalisiert, indem er durch die Standardabweichung der Leistungsänderungen über mehrere Permutationen geteilt wird, um die Stabilität der Schätzung zu erhöhen.



### Beispiel - Hauspreisvorhersage

Gegeben sei ein lineares Regressionsmodell, das den Preis eines Hauses basierend auf folgenden Merkmalen vorhersagt:

- Wohnfläche (Größe): Quadratmeter der Wohnfläche
- Anzahl der Zimmer: Gesamtzahl der Zimmer im Haus
- Alter des Hauses: Jahre seit dem Bau des Hauses

Nachfolgende Aktionen: 
- Ein Modell hat auf dem Testdatensatz einen MSE von 2000 Euro. 
- Nach der Permutation der "Wohnfläche" ergibt sich ein MSE von 3500 Euro. Die Differenz ist 1500 Euro.
- Nach der Permutation der "Anzahl der Zimmer" ergibt sich ein MSE von 2100 Euro. Die Differenz ist 100 Euro.
- Nach der Permutation des "Alters des Hauses" ergibt sich ein MSE von 2200 Euro. Die Differenz ist 200 Euro.

#### Interpretation

- Die "Wohnfläche" hat die größte Auswirkung auf den Vorhersagefehler (Differenz = 1500 Euro), daher ist sie das wichtigste Merkmal.
- Die "Anzahl der Zimmer" und das "Alter des Hauses" haben weniger Einfluss auf den Vorhersagefehler (Differenz = 100 Euro bzw. 200 Euro), daher sind sie weniger wichtige Merkmale.


### Sourcecode "Permutation Feature Importance"

| RefID | Verweis                                     |
| ----- | ------------------------------------------- |
| 26    | QM-27_Permutation Feature Importance_python |




### Referenzen

| RefID | Verweis                                   | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 102   |  Kaggle - Feature Importance - Beispiele  | Das Kaggle-Notebook zur Feature Importance bietet einen Überblick über verschiedene Methoden zur Bewertung von Feature-Bedeutungen in Machine-Learning-Modellen, einschließlich Permutationsbedeutung, baumbasierten Modellen und SHAP-Werten, und richtet sich mit praxisnahen Beispielen und Visualisierungen an Praktiker, die das Modellverständnis verbessern möchten. |


---
Name: MA-11 Größe des Trainingsdatensatzes
Title: MA-11 Größe des Trainingsdatensatzes
TitleGer: MA-11 Stichprobengröße
shortdesc: Optimale Größe für den Trainingsdatensatz erfordert iterative Anpassung nach vorherigen Tests
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-11
ListMetricID: 
ListMeasureID:
  - "'QB-05'"
  - "'QB-06'"
share: true
---
## MA-11 Größe des Trainingsdatensatzes

### Beschreibung

Die notwendige Stichprobengröße bzw. die notwendige Menge an Trainingsdaten kann über die Fehlerschwankung und das Konfidenzniveau berechnet werden. Sie ist darüber hinaus abhängig von der Größe der Gesamtpopulation.

Es kann auch deutliche Unterschiede in den Trainingsergebnissen geben, je nachdem, ob Daten "horizontal" oder "vertikal" vergrößert werden. 

- **Horizontal**  
  Bei der horizontalen Vergrößerung wird die Anzahl der Datenpunkte (Instanzen) erhöht. Das heißt, es werden mehr Beispiele desselben Merkmalsraums gesammelt oder generiert, um die Stichprobe zu verbreitern. Typische Maßnahmen sind:
  - Aufnahme zusätzlicher Aufzeichnungen oder Messungen  
  - Datenerweiterung durch Data Augmentation (z. B. Bildrotation, Rauschen)  
  - Sammeln von Daten aus neuen Quellen

- **Vertikal**  
  Bei der vertikalen Vergrößerung werden die Merkmale (Features) eines Datensatzes erweitert. Das bedeutet, dass pro Instanz zusätzliche Variablen erhoben oder abgeleitet werden, um den Informationsgehalt zu steigern. Beispiele hierfür sind:
  - Hinzufügen neuer Sensor- oder Attributwerte  
  - Berechnung abgeleiteter Features (z. B. statistische Kennwerte, Text-Embeddings)  
  - Einbeziehung externer Datendimensionen (z. B. geografische oder zeitliche Kontextinformationen)


### Metriken & Methoden

| ID                       | Kurzbeschr.                                                                                                                                                                                      |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-08 LearningCurve      | Mittels einer "Learning Curve" kann die Abhängigkeit einer Trainings- oder Validierungsmetrik (z.B. Genauigkeit) von der Größe des Datensatzes in ausgedrückt werden (z.B. in Form eines Plots). |
| QM-09 KonfidenzNiveau    | Wahrscheinlichkeit, dass ein Konfidenzintervall den wahren Wert enthält.                                                                                                                         |
| QM-39 Power Analyse      | Poweranalyse bestimmt benötigte Stichprobengröße für statistisch signifikanten Effekt.                                                                                                           |
| QM-41 KonfidenzIntervall | Statistisches Maß für Unsicherheit um Schätzwert, mit Konfidenzniveau.                                                                                                                           |


### Referenzen

| RefID | Verweis                                          | Kurzbeschr.                                                                                                                                                                                                                                                                                 |
| ----- | ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 71    |  Statistical learning theory                     | Das Buch behandelt unter anderem die theoretischen Grundlagen für die Auswahl der Trainingsdaten.                                                                                                                                                                                           |
| 178   |  Training Compute-Optimal Large Language Models  | Die Studie belegt, dass Modelle optimal trainiert werden, wenn Parameterzahl und Tokenmenge gleich skaliert werden, und zeigt, dass Chinchilla (70 Mrd. Parameter) – dank deutlich mehr Trainingsdaten – Gopher (280 Mrd.) und GPT-3 in Effizienz und MMLU-Genauigkeit (67,5 %) übertrifft. |

---
Name: QM-10-1_PrincipalComponentAnalysis
Title: QM-10-1 Principal Component Analysis
TitleGer: QM-10-1 Principal Component Analysis
shortdesc: PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.
tags:
  - Qualitätsmetrik
  - "#metric-method"
  - "#ML-DimRed"
  - metric-method
  - ML-DimRed
ID:
  - QM-10-1
ListMetricID: 
ListMeasureID:
  - "'MA-8'"
  - "'QB-12'"
  - "'MA-12'"
  - "'MA-14'"
  - "'MA-16'"
  - "'MA-23'"
  - "'MA-08'"
  - "'MA-10'"
type:
  - method
CodeEx: true
share: true
lcstep: pre
---
## QM-10-1 Principal Component Analysis

### Beschreibung

Die Principal Component Analysis (PCA) ist eine statistische Methode, die verwendet wird, um die Struktur in den Daten zu verstehen, indem man die Dimensionalität reduziert ohne dabei zu viel Information zu verlieren. Das Ziel ist es, die ursprünglichen Merkmale in eine kleinere Anzahl von nicht-korrelierten Merkmale umzuwandeln, die als Hauptkomponenten (Principal Components - PC's) bezeichnet werden. Die Durchführung einer PCA umfasst mehrere Schritte. Die PCA ist ein mächtiges Werkzeug der explorativen Datenanalyse. Sie hilft, die Komplexität zu reduzieren und die interpretierbaren Informationen zu maximieren.

### Vorgehensweise: 

Detaillierte Beschreibungen der einzelnen Punkte sind in den entsprechenden Metriken hinterlegt. 

- **Standardisierung der Daten**: Skalierung der Daten, so dass jede Variable einen Mittelwert von 0 und eine Standardabweichung von 1 hat. 
- **Berechnung der Kovarianzmatrix**: Ermittlung der Kovarianz zwischen allen Variablen, um die Beziehungen zwischen ihnen zu verstehen.
- **Berechnung der Eigenwerte und Eigenvektoren**: Aus der Kovarianzmatrix werden Eigenwerte und Eigenvektoren berechnet, die die Richtung und Größe der Hauptkomponenten angeben.
- **Sortieren der Eigenvektoren**: Die Eigenvektoren werden nach ihren zugehörigen Eigenwerten in absteigender Reihenfolge sortiert. Die Eigenwerte geben die Varianz an, die jede Hauptkomponente einfängt.
- **Auswahl der Hauptkomponenten**: Entscheidung, wie viele Hauptkomponenten beibehalten werden sollen, basierend auf ihrem Beitrag zur Gesamtvarianz.
- **Transformation der Daten**: Die ursprünglichen Daten werden in den neuen Raum transformiert, der durch die ausgewählten Hauptkomponenten definiert wird, indem die Daten mit den Eigenvektoren multipliziert werden.
- **Interpretation der Ergebnisse**: Analyse der transformierten Daten bzw. der Hauptkomponenten, um Muster oder Strukturen zu identifizieren und zu interpretieren.

### Python Code für "PrincipalComponentAnalysis"

| RefID | Verweis                                 |
| ----- | --------------------------------------- |
| 10    | QM-10_PrincipalComponentAnalysis_python |



### Referenzen

| RefID | Verweis                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                         |
| ----- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 61    |  Hauptkomponentenanalyse und explorative Faktorenanalyse                              | Der Beitrag führt in die Grundlagen der Hauptkomponentenanalyse (PCA) und explorativen Faktorenanalyse (EFA) ein.                                                                                                                                                                                                                                                                                   |
| 82    |  A Tutorial on Principal Component Analysis                                           | Dieses Papier soll dazu beitragen, die „Blackbox“ der Hauptkomponentenanalyse (PCA) verständlich zu machen, indem es von einfachen Intuitionen bis hin zu den zugrundeliegenden mathematischen Prinzipien führt. Durch die Verbindung informeller Erklärungen mit mathematischen Herleitungen erhalten Leser aller Niveaus ein besseres Verständnis dafür, wann, wie und warum PCA eingesetzt wird. |
| 115   |  Hauptkomponentenanalyse                                                              | Die Hauptkomponentenanalyse (HKA) ist ein Verfahren der multivariaten Statistik, das große Datensätze durch Eigenvektoren der Kovarianzmatrix vereinfacht, indem viele Variablen zu wenigen aussagekräftigen Hauptkomponenten zusammengefasst werden. Sie findet Anwendung unter anderem in der Signal- und Bildverarbeitung und ist von der Faktorenanalyse zu unterscheiden.                      |
| 176   |  Principal component analysis                                                         | Die Hauptkomponentenanalyse (PCA) ist eine wichtige Technik der multivariaten Datenanalyse.                                                                                                                                                                                                                                                                                                         |
| 224   |  ClusterGraph: a new tool for visualization and compression of multidimensional data  | Herkömmliche Methoden zur Analyse hochdimensionaler Daten wie Dimensionsreduktion und Clustering bewahren zwar lokale Strukturen, erfassen jedoch oft nicht die globale Datenorganisation. Das Paper stellt den ClusterGraph vor, eine datenstrukturierte Ergänzung, die die globale Anordnung von Clustern bewahrt und eine qualitativ hochwertige Visualisierung und Analyse ermöglicht.          |

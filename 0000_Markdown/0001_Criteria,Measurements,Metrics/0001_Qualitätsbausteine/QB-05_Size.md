---
Name: QB-05_Size
Title: QB-05 Size
TitleGer: QB-05 Umfang
shortdesc: Größere Datensätze verbessern Modellgenauigkeit, Robustheit und reduzieren Overfitting.
tags:
  - Qualitätsbaustein
ID:
  - QB-05
ListCritID:
  - "'QKB-01'"
  - "'QKB-08'"
  - "'QKB-07'"
share: true
---
## QB-05 Umfang

### Beschreibung 

Der Qualitätsbaustein "Umfang" beschreibt den messbaren Umfang eines Trainingsdatensatzes, indem er vor allem die Anzahl der enthaltenen Datenpunkte in den Blick nimmt. Eine große Datenmenge ermöglicht es, statistische Zusammenhänge genauer zu identifizieren, seltene Muster abzubilden und die Stabilität des Modells zu erhöhen, indem Zufallseffekte reduziert werden. Der reine quantitative Aspekt sorgt dafür, dass genügend Beispiele vorhanden sind, um eine fundierte und belastbare Analyse der zugrundeliegenden Datenverteilungen zu ermöglichen. Durch große Datensätze sind auch die Trainingsläufe weniger anfällig für Overfitting. Größere Datensätze können auch die Generalisierung und die Robustheit von Trainingsverfahren verbessern. 

Im Gegensatz dazu konzentrieren sich ähnliche Kriterien wie **Datenvielfalt**, **Repräsentativität** oder Datenintegrität auf die qualitativen Dimensionen der Daten. Während beispielsweise die Datenvielfalt die Bandbreite und Heterogenität der Merkmale erfasst und Repräsentativität überprüft, inwieweit die Daten die gesamte Problemwelt abbilden, fokussiert sich die Größe ausschließlich auf den numerischen Umfang. Somit bildet sie eine grundlegende Basis, die jedoch ergänzend zu den qualitativen Aspekten betrachtet werden muss, um ein vollständiges Bild der Datenqualität zu erhalten.
### Beispiele

#### Bilderkennung

##### MNIST-Datensatz

- Größe: 70.000 Bilder (60.000 Trainingsbilder, 10.000 Testbilder)
- Beschreibung: Enthält handgeschriebene Ziffern von 0 bis 9, die in 28x28 Pixelbildern dargestellt sind.

##### ImageNet-Datensatz

- Größe:  > 14 Millionen Bilder
- Beschreibung: Enthält Bilder aus 1000 Klassen, die für die Objekterkennung und Bildklassifizierung verwendet werden.


#### Textklassifikation

##### IMDB-Datensatz

- Größe: 50.000 Filmrezensionen (25.000 für Training, 25.000 für Testen)
- Beschreibung: Wird für die Sentiment-Analyse (positive oder negative Bewertung) verwendet.

##### 20 Newsgroups-Datensatz

- Größe: Rund 20.000 Dokumente, verteilt auf 20 verschiedene Newsgroups
- Beschreibung: Wird für die Textklassifikation und Themenmodellierung verwendet.




### Maßnahmen

| Maßnahme                             | Kurzbeschr.                                                                                   |
| ------------------------------------ | --------------------------------------------------------------------------------------------- |
| MA-11 Größe des Trainingsdatensatzes | Optimale Größe für den Trainingsdatensatz erfordert iterative Anpassung nach vorherigen Tests |
| MA-12 Abdeckung relevanter Merkmale  | Abdeckung aller wichtigen Merkmale im Datensatz zur Modellierung.                             |
| MA-15 Empirische Evidenz             | Vergleich ähnlicher Fälle ermöglicht Rückschlüsse auf Maßnahmeneffektivität.                  |
| MA-27 StatisticalBasics              | Sammelobjekt für statistische Grundlagen                                                      |


### Referenzen

| RefID | Verweis                                                                                                                                                              | Kurzbeschr.                                                                                                                                                                                                                                                                                                                            |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 18    |  ISO/IEC 5259-2 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 2: Data quality measures                                     | Dieser Standard spezifiziert Maßnahmen zur Bewertung und Sicherstellung der Datenqualität, einschließlich der Ausgewogenheit der Daten.                                                                                                                                                                                                |
| 19    |  ISO/IEC 5259-3:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 3: Data quality management requirements and guidelines  | Dieses Dokument definiert allgemeine Anforderungen und Leitlinien für die Verbesserung, Implementierung und Aufrechterhaltung der Datenqualität in Analytik und maschinellem Lernen, anwendbar auf alle Organisationen unabhängig von Art, Größe oder Beschaffenheit, ohne detaillierte Prozesse, Methoden oder Metriken vorzugeben.   |
| 25    |  ISO/IEC 20546:2019 - Information technology — Big data — Overview and vocabulary                                                                                    | Information technology — Big data — Overview and vocabulary bietet eine umfassende Übersicht über Big Data, einschließlich der Terminologie, Konzepte und allgemeinen Prinzipien, die mit Big Data-Technologien und -Anwendungen verbunden sind. Es dient als Grundlage für das Verständnis und die Kommunikation im Bereich Big Data. |
| 28    |  ISO/IEC 22989:2022 - Information technology — Artificial intelligence — Artificial intelligence concepts and terminology                                            | Dieser Standard definiert die grundlegenden Konzepte und die Terminologie im Bereich der künstlichen Intelligenz, einschließlich der Aspekte der Datenqualität und Ausgewogenheit von Trainingsdaten.                                                                                                                                  |
| 40    |  ISO/IEC TR 24027:2021 - Information technology — Artificial intelligence (AI) — Bias in AI systems and AI aided decision making                                     | Der Bericht untersucht Bias in KI-Systemen und betont, dass hochwertige Trainingsdaten essenziell sind, um Verzerrungen zu reduzieren und faire, gerechte Entscheidungen zu ermöglichen.                                                                                                                                               |
| 163   |  Towards better generalization: Weight Decay induces low-rank bias for neural networks                                                                               | Das Paper zeigt, dass Weight Decay in neuronalen Netzen eine Low-Rank-Voreingenommenheit in den Gewichtsmatrizen induziert, was die Generalisierung verbessert, indem es die Generalisierungsfehler verringert.                                                                                                                        |
| 178   |  Training Compute-Optimal Large Language Models                                                                                                                      | Die Studie belegt, dass Modelle optimal trainiert werden, wenn Parameterzahl und Tokenmenge gleich skaliert werden, und zeigt, dass Chinchilla (70 Mrd. Parameter) – dank deutlich mehr Trainingsdaten – Gopher (280 Mrd.) und GPT-3 in Effizienz und MMLU-Genauigkeit (67,5 %) übertrifft.                                            |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                                                        | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.                                                    |
| 190   |  Kriterienkatalog C5                                                                                                                                                 | Der C5 (Cloud Computing Compliance Criteria Catalogue) des Bundesamts für Sicherheit in der Informationstechnik (BSI) stellt einen detaillierten Kriterienkatalog dar, der grundlegende Anforderungen an die Informationssicherheit von Cloud-Diensten festlegt.                                                                       |
| 206   |  Open Data Act                                                                                                                                                       | RICHTLINIE  (EU)  2019/  1024  DES  EUROPÄISCHEN  PARLAMENTS  UND  DES  RATES  -  vom  20. Juni  2019  -  über  offene  Daten  und  die  Weiterverwendung  von  Informationen  des  öffentlichen  Sektors                                                                                                                              |



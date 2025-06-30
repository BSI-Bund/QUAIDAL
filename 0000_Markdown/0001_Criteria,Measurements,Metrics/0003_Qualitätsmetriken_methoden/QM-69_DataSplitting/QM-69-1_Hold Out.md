---
Name: QM-69-1_Hold Out
Title: QM-69-1 Hold Out
TitleGer: QM-69-1 Hold Out
shortdesc: Beim Hold-out-Verfahren wird der Datensatz einmalig in Trainings-, Test- und optional Validierungsanteile aufgeteilt, um Modellbildung, Hyperparameteroptimierung und objektive Evaluation klar zu trennen.
tags:
  - Qualitätsmetrik
ID:
  - QM-69-1
ListMetricID: 
ListMeasureID:
  - "'MA-29'"
MID: 
type:
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-69-1 Hold-Out Verfahren

### Beschreibung

Das Hold-out-Verfahren teilt einen vorhandenen Datensatz einmalig in unabhängige Teilmengen auf, um ein Modell zu trainieren und anschließend dessen Leistung objektiv zu bewerten. Konkret wird der Datensatz häufig in einen Trainingssatz (z. B. 70–80%), der zur Modellbildung dient, und einen Testsatz (z. B. 10–15%) aufgeteilt, der ausschließlich zur abschließenden Evaluation verwendet wird; manchmal wird zusätzlich ein Validierungssatz (ebenfalls ca. 10–15%) eingeführt, um während der Trainingsphase Hyperparameter zu optimieren, ohne die finale Testbewertung zu beeinflussen.

### Formel

| Teilmenge   | Typische Verteilungsgewichte |
| ----------- | ---------------------------- |
| Training    | 60% – 80%                    |
| Validierung | 10% – 20%                    |
| Test        | 10% – 30%                    |

### Beispiele 

#### Beispiel 1 – Bildklassifikation:  
Auf Basis eines Datensatzes mit 10.000 Bildern soll ein Convolutional Neural Network (CNN) trainiert werden.

- **Aufteilung:**
    - **Training (70%):** 7000 Bilder
    - **Validierung (15%):** 1500 Bilder
    - **Test (15%):** 1500 Bilder
        
- **Begründung:**  
    Mit 70% der Daten im Trainingsset wird sichergestellt, dass genügend Beispiele vorliegen, um die Vielfalt der Bildmotive zu erlernen, während 15% jeweils im Validierungs- und Testset eine verlässliche Optimierung der Hyperparameter sowie eine objektive Endbewertung ohne Datenleck ermöglichen.

#### Beispiel 2 – Textklassifikation:  
Ein Datensatz mit 6.000 Textdokumenten soll zur Klassifikation von Nachrichtenartikeln genutzt werden.

- **Aufteilung:**
    - **Training (80%):** 4800 Texte
    - **Validierung (10%):** 600 Texte
    - **Test (10%):** 600 Texte
        
- **Begründung:**  
    Durch einen größeren Anteil (80%) im Trainingsset wird sichergestellt, dass das Modell ausreichend Beispiele zur Erfassung sprachlicher Nuancen erhält. Die geringeren Anteile im Validierungs- und Testset (je 10%) erlauben eine effiziente Hyperparameterabstimmung und zuverlässige Leistungsüberprüfung, ohne dass zu viele Daten aus dem Trainingsprozess entnommen werden.

### Sourcecode "Hold Out"
| RefID | Verweis                 |
| ----- | ----------------------- |
| 92    | QM-69-1_Hold Out_python |



### Referenzen
| RefID | Verweis                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                           |
| ----- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 304   |  Training, validation, and test data sets  | Beim maschinellen Lernen wird ein Modell typischerweise anhand eines Trainingsdatensatzes gelernt, mit einem Validierungsdatensatz zur Feinabstimmung der Hyperparameter optimiert und schließlich mit einem unabhängigen Testdatensatz (oft als Holdout bezeichnet) objektiv bewertet, wobei die genaue Aufteilung stark vom Anwendungsfall abhängt. |

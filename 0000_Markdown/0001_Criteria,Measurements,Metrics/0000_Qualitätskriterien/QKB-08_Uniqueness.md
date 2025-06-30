---
Name: QKB-08 Eindeutigkeit
Title: QKB-08 Eindeutigkeit
TitleGer: QKB-08 Eindeutigkeit
shortdesc: Jeder Datensatz muss eindeutig interpretierbar sein. Das Vorhandensein von Duplikaten kann zu Verwirrung und Fehlern in Analysen und Berichten führen.
tags:
  - Qualitätskriterien
ID:
  - QKB-08
ListMeasureID: 
ListCritID: 
share: true
---
## QKB-08 Eindeutigkeit

### Beschreibung 

Jeder Datensatz muss eindeutig interpretierbar, klar und unmissverständlich sein. Das Vorhandensein von Duplikaten kann zu Verwirrung und Fehlern in Analysen und Berichten führen oder im Training von Modellen zu Overfitting führen.

In Abgrenzung zur Eindeutigkeit bezieht sich Einheitlichkeit auf die Standardisierung von Datenformaten und -werten über verschiedene Datensätze hinweg, wie zum Beispiel die einheitliche Verwendung von Datumsformaten oder Maßeinheiten. Eindeutigkeit hingegen stellt sicher, dass jede Dateneinheit nur einmal existiert und eindeutig identifizierbar ist, um Duplikate zu vermeiden. Einheitlichkeit bezieht beispielsweise darauf, dass alle Daten in einem Datensatz im selben Format vorliegen (z.B.: dd-MM-yyyy). Konsistenz dagegen stellt sicher, dass die Daten frei von Widersprüchen und logisch zusammenhängend sind. 

### Beispiele

#### Kategorisierung von Tieren 

In einem einen Datensatz werden Tiere klassifiziert. Die Kategorien sind „Hund“, „Katze“ und „Vogel“. Eine eindeutige Kategorisierung würde sicherstellen, dass es keine Überlappungen gibt, wie z. B. die Kategorie „Hund/Katze“. Jedes Tier wird eindeutig einer Kategorie zugeordnet, ohne Mehrdeutigkeiten. Zum Beispiel:

- Ein Labrador wird eindeutig als „Hund“ kategorisiert.
- Eine Siamkatze wird eindeutig als „Katze“ kategorisiert.

Diese klare Trennung verhindert Missverständnisse und stellt sicher, dass das Modell genau lernen kann, was unter „Hund“ oder „Katze“ zu verstehen ist.

#### Eindeutige Bestellnummern

Jede Bestellung in einem Online-Shop erhält eine eindeutige Bestellnummer, um Verwechslungen und doppelte Einträge zu vermeiden.


### Bausteine

| Baustein              | Kurzbeschr.                                                                                                                                                                                                               |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QB-05_Size            | Größere Datensätze verbessern Modellgenauigkeit, Robustheit und reduzieren Overfitting.                                                                                                                                   |
| QB-10_DataChecks      | Überprüfung von Trainingsdaten sichert Qualität vor dem Modelltraining.                                                                                                                                                   |
| QB-13_DataPreparation | Die Datenvorbereitung bezieht sich auf alle Datentransformationsschritte, die erforderlich sind, um Rohdaten in eine initial nutzbare Form zu bringen, die für das Training eines Machine-Learning-Modells geeignet sind. |



### Referenzen

| RefID | Verweis                                                                                                                          | Kurzbeschr.                                                                                                      |
| ----- | -------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model  | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell |

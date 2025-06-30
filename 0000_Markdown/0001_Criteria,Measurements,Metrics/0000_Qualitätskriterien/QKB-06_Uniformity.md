---
Name: QKB-06 Einheitlichkeit
Title: QKB-06 Einheitlichkeit
TitleGer: QKB-06 Einheitlichkeit
shortdesc: Definieren von Form, Inhalt und Einheitlichkeit eines Datensatzes.
tags:
  - Qualitätskriterien
ID:
  - QKB-06
ListMeasureID: 
ListCritID: 
share: true
---

## QKB-06 Einheitlichkeit

### Beschreibung 

Einheitlichkeit bezeichnet die konsequente Anwendung von festgelegten Formaten, Strukturen und Darstellungsregeln bei der Datenerfassung und -verarbeitung. Dabei wird sichergestellt, dass alle Datenfelder gemäß vorab definierten Standards angelegt und dargestellt werden – beispielsweise durch ein einheitliches Datumsformat, standardisierte Maßeinheiten oder konsistente Kodierungen von Kategorien. Das Kriterium "Einheitlichkeit" bezieht sich ausschließlich auf diese formalen Aspekte der Daten und garantiert, dass alle Einträge optisch und strukturell identisch formatiert vorliegen, unabhängig von deren inhaltlicher Richtigkeit oder logischer Verbindung.

Einheitlichkeit fokussiert sich rein auf die Standardisierung und das Format der Daten und überschneidet sich nicht mit inhaltlichen Aspekten. Konsistenz stellt sicher, dass die inhaltlichen Angaben in verschiedenen Datensätzen logisch zusammenpassen, während Korrektheit die Fehlerfreiheit der Daten in Hinblick auf reale Werte sicherstellt. Genauigkeit bezieht sich dagegen auf die quantitative Nähe von Messwerten zum Ideal- oder Referenzwert.

### Beispiele

#### Formatierung von Datumsangaben

Einheitlich: Alle Datumsangaben in einem Datensatz verwenden das Format "YYYY-MM-DD". Nicht einheitlich: Einige Datumsangaben sind im Format "DD/MM/YYYY" und andere im Format "MM-DD-YYYY".

#### Verwendung von Maßeinheiten

Einheitlich: Alle Längenangaben werden in Zentimetern angegeben. Nicht einheitlich: Einige Längenangaben sind in Zentimetern, andere in Metern und wieder andere in Zoll.


### Bausteine

| Baustein                  | Kurzbeschr.                                                                                                                                                                                                                               |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QB-02_Semantic Accuracy   | Genauigkeit bzgl. Bedeutung und Kontext in Daten                                                                                                                                                                                          |
| QB-08 Konsistenzsicherung | Einheitliche, widerspruchsfreie Datenformate und -werte gewährleisten.                                                                                                                                                                    |
| QB-10_DataChecks          | Überprüfung von Trainingsdaten sichert Qualität vor dem Modelltraining.                                                                                                                                                                   |
| QB-12_FeatureEngineering  | Feature Engineering wandelt Rohdaten um, verbessert ML-Modelle durch relevante, generalisierbare, skalierbare Features.                                                                                                                   |
| QB-14_Expertanalysis      | Die Expertenanalyse ist ein Allzweckwerkzeug um die Qualität eines Trainingsdatensatzes hinsichtlich bestimmter Kriterien zu prüfen. Idealerweise werden dafür mehrere Expert\*innen unabhängig voneinander um eine Einschätzung gebeten. |



### Referenzen

| RefID | Verweis                                                                                                                          | Kurzbeschr.                                                                                                      |
| ----- | -------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model  | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell |


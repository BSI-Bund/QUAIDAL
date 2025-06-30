---
Name: QM-59-3_Metadaten-Vollständigkeit
Title: QM-59-3_Metadaten-Vollständigkeit
TitleGer: QM-59-3_Metadaten-Vollständigkeit
shortdesc: Anteil der Datensätze mit vollständigen Herkunfts-Metadaten
tags:
  - Qualitätsmetrik
  - Methods-Meta
ID:
  - QM-59-3
ListMetricID: 
ListMeasureID:
  - "'MA-17'"
MID: 
type:
  - metrik
  - method
share: true
lcstep: pre
CodeEx: true
---
## QM-59-3 Metadaten-Vollständigkeit

### Beschreibung

Die Metrik "Metadaten-Vollständigkeit“ misst, wie viele Datensätze in einem System über lückenlos dokumentierte Informationen zur Datenherkunft verfügen – etwa Quelle, Erhebungszeitpunkt und verantwortliche Akteure. Sie ermöglicht eine quantitative Bewertung der Transparenz und Rückverfolgbarkeit innerhalb eines Datenbestands und dient als Indikator für die Umsetzung eines etablierten Provenienz-Metadatenschemas.

### Beispiele 

#### Beispiel 1 - Verkehrsdaten einer Smart City:  

Ein städtisches Verkehrsmanagementsystem sammelt Bewegungsdaten von Sensoren an 100 Kreuzungen. Die Stadtverwaltung definiert ein Provenienz-Schema, das für jeden Datensatz folgende Angaben verlangt: Sensor-ID, Standort, Zeitpunkt der Messung, eingesetzter Sensortyp und verantwortliche Wartungsfirma. Bei einer Stichprobe zeigt sich, dass 87 von 100 Datensätzen alle fünf Felder korrekt enthalten – die Metrik ergibt somit: 87 % vollständig dokumentierte Datensätze.

#### Beispiel 2 – Gesundheitsdaten in einer KI-Studie:  

Ein Forschungsteam verwendet Patientendaten zur Entwicklung eines KI-Modells zur Diagnostik. Das Provenienz-Schema fordert Angaben zu Erhebungsort (Klinik), Erhebungszeitraum, Zustimmung der Patienten, eingesetzte Diagnosetechnologie und den Namen des durchführenden Arztes. Bei der Evaluierung sind nur 62 % der Datensätze vollständig mit diesen Metadaten versehen – entsprechend beträgt die Metrik hier: 62 % vollständig dokumentierte Datensätze, was auf eine Verbesserung der Dokumentationsprozesse hinweist.

### Sourcecode "Metadaten-Vollständigkeit"
| RefID | Verweis                                  | Inhalt                                                                                                       |
| ----- | ---------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 94    | QM-59-3_Metadaten-Vollständigkeit_python | Erstellt ein Datenfeld mit abstrakten Informationen und berechnet die Vollständigkeitsmetrik ihrer Metadaten |


### Referenzen
| RefID | Verweis                                                       | Kurzbeschr.                                                                                                                                                                                                                                                                                                     |
| ----- | ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 96    |  Statistical analysis with missing data                       | Die erste Auflage von Statistical Analysis with Missing Data wird für ihren wichtigen Beitrag zur angewandten Statistik, ihre zugängliche Darstellung von aktuellen und früheren Arbeiten sowie interessante Beispiele und Übungen gelobt und sollte auf jedem Statistikregal stehen.                           |
| 191   |  The Effects of Data Quality on Machine Learning Performance  | Moderne KI-Anwendungen erfordern große Mengen hochwertiger Daten. Unvollständige oder fehlerhafte Daten führen zu unzuverlässigen Modellen und schlechten Entscheidungen. Eine vertrauenswürdige KI ist auf genaue, vollständige und konsistente Daten angewiesen.                                              |
| 288   |  DOI Foundation                                               | Ein DOI (Digital Object Identifier) ist ein standardisierter, persistenter Identifikator, der digitale Objekte wie wissenschaftliche Artikel eindeutig kennzeichnet, indem er aus einem Präfix und einem individuellen Suffix besteht, und so auch bei Änderungen des Speicherorts dauerhaft zugänglich bleibt. |
| 289   |  DataCite Schema                                              | Das DataCite Metadata Schema Kernel 4.6 legt einheitliche, erweiterte Kern-Metadatenfelder (z. B. Identifier, Creator, Title, ResourceTypeGeneral, RelatedIdentifierType, ContributorType, DateType) zur konsistenten Beschreibung und Zitierung von Forschungsdaten fest .                                     |



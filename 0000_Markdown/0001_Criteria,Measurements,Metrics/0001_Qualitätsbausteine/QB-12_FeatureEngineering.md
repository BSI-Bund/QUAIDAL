---
Name: QB-12_FeatureEngineering
Title: QB-12 FeatureEngineering
TitleGer: QB-12 Merkmalsentwicklung
shortdesc: Feature Engineering wandelt Rohdaten um, verbessert ML-Modelle durch relevante, generalisierbare, skalierbare Features.
tags:
  - Qualitätsbaustein
ID:
  - QB-12
ListCritID:
  - "'QKB-05'"
  - "'QKB-04'"
  - "'QKB-06'"
share: true
---
## QB-12 Feature Engineering

### Beschreibung

Feature Engineering ist ein wichtiger Schritt im maschinellen Lernen und in der Datenvorverarbeitung. Es bezieht sich auf den Prozess, aus den Rohdaten relevante Merkmale (Features) zu erstellen/auszuwählen oder bestehende Merkmale so zu transformieren, dass sie für das Modell besser nutzbar werden. Die Merkmale sollten folgende Aspekte umfassen: 

#### Relevanz 
Features sollten relevant für die Aufgabe sein. Sie müssen eine signifikante Beziehung zur Zielvariable haben, damit das Modell gültige Vorhersagen oder Klassifikationen vornehmen kann.
    
#### Verständlichkeit
Die transformierten Features sollten möglichst klar und verständlich sein. Sowohl für diejenigen, die die Modelle entwickeln, als auch für diejenigen, die die Ergebnisse interpretieren, ist es wichtig, die Features zu verstehen.
    
#### Informationsgewinn
Ein gutes Feature bringt neue Informationen oder Erkenntnisse, die nicht bereits in anderen Features vorhanden sind. Dies kann die Vorhersagekraft des Modells erhöhen.
    
#### Redundanzvermeidung
Features sollten nicht redundant sein, d.h., sie sollten keine Kopien oder nahezu identische Versionen anderer Features im Datensatz sein. Redundante Features können zu unnötiger Komplexität und zu Überanpassung (Overfitting) führen.
    
#### Generalisierbarkeit
Die erstellten Features sollten gut generalisieren und auch auf neue, unbekannte Daten anwendbar sein, um das Modell robust gegenüber Datenveränderungen zu machen.
    

#### Skalierbarkeit

Feature Engineering sollte effizient und skalierbar sein. Die Erstellung und Verarbeitung von Features sollten nicht zu rechenintensiv sein insbesondere, wenn große Datensätze vorliegen.


### Maßnahmen

| Maßnahme                            | Kurzbeschr.                                                                                                                                                                                                                                                   |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MA-01 Datentyp Validierung          | Eine sorgfältige Validierung der Datentypen stellt sicher, dass Trainings- und Eingabedaten den erwarteten Typen des Modells entsprechen, wodurch fehlerhafte Datenpunkte erkannt und gegebenenfalls korrigiert oder entfernt werden können.                  |
| MA-02 Format Prüfung                | Inhalte mittels Formatierungsprüfung auf Korrektheit prüfen                                                                                                                                                                                                   |
| MA-03_Range Check                   | Bereichsprüfung erkennt Ausreißer und falsche Daten in Merkmalen                                                                                                                                                                                              |
| MA-06_Expert Evaluation             | Ein Experte prüft die Daten manuell.                                                                                                                                                                                                                          |
| MA-12 Abdeckung relevanter Merkmale | Abdeckung aller wichtigen Merkmale im Datensatz zur Modellierung.                                                                                                                                                                                             |
| MA-14 EDA-Explorative Daten Analyse | Die Explorative Datenanalyse (EDA) dient dazu, Hauptmerkmale, Muster und Anomalien in Datensätzen zu entdecken, um ein tiefes Verständnis der Daten für fundierte weitere Analyseschritte zu entwickeln.                                                      |
| MA-17_MetadataManagement            | Metadaten sind beschreibende Daten über andere Daten, die deren Verwaltung, Analyse und Nutzung erleichtern und im Trainingsprozess zur Verbesserung von Trainingsdatensätzen eingesetzt werden können.                                                       |
| MA-23 Merkmalsskalierung            | Feature Scaling passt die Merkmale eines Datensatzes an einen einheitlichen Bereich an, um Unterschiede in den Skalierungen zu reduzieren und sicherzustellen, dass maschinelle Lernalgorithmen effizienter arbeiten und genauere Vorhersagen liefern können. |
| MA-24 Merkmalserstellung            | Methoden zur Generierung neuer Merkmale aus Rohdaten, um die Leistung von maschinellen Lernmodellen zu verbessern.                                                                                                                                            |
| MA-27 StatisticalBasics             | Sammelobjekt für statistische Grundlagen                                                                                                                                                                                                                      |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                  | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 4     |  ISO 8000-61:2016 - Data quality — Part 61: Data quality management: Process reference model                                                                                                                                                                             | Das Dokument beschreibt den Datenqualitätsmanagementprozess als steuerbaren, wiederholbaren und verbesserbaren Ablauf (PDCA), betont die kontinuierliche Verbesserung der Daten bei Fehlern und die Einbeziehung verschiedener Stakeholder wie Nutzer, Management und Datenmanager.                                                                                                                              |
| 10    |  ISO/TS 8000-81:2021 - Data quality — Part 81: Data quality assessment: Profiling                                                                                                                                                                                        | Die ISO/TS 8000-81:2021 legt ein Verfahren für Datenprofiling zur Bewertung der Datenqualität fest, das sich auf Strukturanalyse, Spaltenanalyse und Beziehungsanalyse konzentriert. Sie ist auf tabellarische Daten anwendbar, behandelt jedoch keine Methoden zur Datenextraktion oder Regelableitung und kann sowohl eigenständig als auch zusammen mit Qualitätsmanagementsystem-Standards verwendet werden. |
| 11    |  ISO/TS 8000-82:2022 - Data quality — Part 82: Data quality assessment: Creating data rules                                                                                                                                                                              | Die ISO/TS 8000-82:2022 behandelt die Datenqualitätsbewertung durch Anwendung von Datenregeln auf verschiedene Datentypen, einschließlich Identifikatoren, Währungen und Datums-/Zeitangaben. Sie betont die Bedeutung von Datenprofiling bei der Formulierung effektiver Datenregeln, um die Integrität und Zuverlässigkeit von Daten in Informationssystemen sicherzustellen.                                  |
| 19    |  ISO/IEC 5259-3:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 3: Data quality management requirements and guidelines                                                                                                      | Dieses Dokument definiert allgemeine Anforderungen und Leitlinien für die Verbesserung, Implementierung und Aufrechterhaltung der Datenqualität in Analytik und maschinellem Lernen, anwendbar auf alle Organisationen unabhängig von Art, Größe oder Beschaffenheit, ohne detaillierte Prozesse, Methoden oder Metriken vorzugeben.                                                                             |
| 24    |  ISO/IEC 8183:2023 - Information technology — Artificial intelligence — Data life cycle framework                                                                                                                                                                        | Das Dokument definiert die Phasen und Maßnahmen der Datenverarbeitung im Lebenszyklus von KI-Systemen und ist für alle Organisationen unabhängig von deren Art, Größe oder Natur anwendbar.                                                                                                                                                                                                                      |
| 29    |  ISO/IEC 23053:2022 - Framework for AI systems using machine learning                                                                                                                                                                                                    | Das Dokument legt ein Rahmenwerk für KI- und ML-Systeme fest, das die Systemkomponenten und Funktionen im KI-Ökosystem beschreibt und für alle Organisationstypen und -größen anwendbar ist.                                                                                                                                                                                                                     |
| 143   |  ISO/IEC 27701:2019 - Extension to ISO/IEC 27001 and ISO/IEC 27002 for privacy information management                                                                                                                                                                    | Sicherheitstechniken – Erweiterung auf ISO/IEC 27001 und ISO/IEC 27002 für das Datenschutzinformationsmanagement – ​​Anforderungen und Richtlinien                                                                                                                                                                                                                                                               |
| 237   |  Digital Services Act - Verordnung (EU) 2022/2065 des Europäischen Parlaments und des Rates vom 19. Oktober 2022 über einen Binnenmarkt für digitale Dienste und zur Änderung der Richtlinie 2000/31/EG (Gesetz über digitale Dienste) (Text von Bedeutung für den EWR)  | Die Verordnung (EU) 2022/2065 über digitale Dienste harmonisiert Vorschriften für Vermittlungsdienste in der EU, stärkt den Schutz von Grundrechten, bekämpft rechtswidrige Inhalte und schafft ein sicheres, transparentes Online-Umfeld.                                                                                                                                                                       |



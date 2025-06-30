---
Name: MA-01 Datentyp Validierung
Title: MA-01 Datentyp Validierung
TitleGer: MA-01 Datentyp Validierung
shortdesc: Eine sorgfältige Validierung der Datentypen stellt sicher, dass Trainings- und Eingabedaten den erwarteten Typen des Modells entsprechen, wodurch fehlerhafte Datenpunkte erkannt und gegebenenfalls korrigiert oder entfernt werden können.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-01
ListMetricID: 
ListMeasureID:
  - "'QB-1'"
  - "'QB-8'"
  - "'QB-12'"
  - "'QB-01'"
  - "'QB-08'"
  - "'QB-06'"
share: true
---
## MA-01 Datentyp Validierung

### Beschreibung

Durch eine sorgfältige Validierung der Datentypen kann sichergestellt werden, dass sowohl Trainings- als auch Eingabedaten den konzeptionierten Typen (z.B. Integer, String, Date) des Modells entsprechen. Dies kann bspw. automatisiert durch Skripte erfolgen oder durch Datenbankmanagementsysteme. Datenpunkte, die nicht den Vorgaben entsprechen und zur Trainings- oder Inferenzzeit zu Problemen führen könnten, können somit detektiert und nötigenfalls bearbeitet oder entfernt werden.

### Beispiele 

* Prüfen, ob der Wert des Attributs "Alter" einem Integer (Ganzzahl) entspricht
* Prüfen, ob der Wert des Attributs "Name" nicht die Länge des Datentyps (z.B. CHAR) überschreitet 

### Metriken & Methoden

| ID                              | Kurzbeschr.                                                                               |
| ------------------------------- | ----------------------------------------------------------------------------------------- |
| QM-32 Reguläre Ausdrücke        |  Technik zur Mustererkennung und Textmanipulation                                         |
| QM-34 Validierung der Feldgröße | Textfelder und Variablen auf erwartete Länge überprüfen. Automatisiert/expertengesteuert. |



### Referenzen

| RefID | Verweis                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                   |
| ----- | ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods  | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                                                                                           |
| 173   |  OWASP - Development-time threats – AI Exchange                                                            | Die OWASP-Seite beschreibt Risiken während der Entwicklung von KI-Systemen, wie Datenvergiftung, geistigen Diebstahl und Supply-Chain-Angriffe. Sie empfiehlt Schutzmaßnahmen wie Verschlüsselung, Datenisolation und Integritätsprüfungen, um Modelle und Daten zu sichern.                                                                  |
| 219   |  Google - Data Validation for Machine Learning                                                             | Die Google-Forschungsseite beschreibt ein Datenvalidierungssystem für maschinelles Lernen, das Anomalien in Eingabedaten erkennt und so die Datenqualität für das Modelltraining sicherstellt. Es verbessert die Fehlererkennung und Effizienz, indem es große Produktionsdaten überwacht und in die TFX-Plattform von Google integriert ist. |

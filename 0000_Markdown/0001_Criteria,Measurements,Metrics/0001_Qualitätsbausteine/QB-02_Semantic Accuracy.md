---
Name: QB-02_Semantic Accuracy
Title: QB-02 Semantische Genauigkeit
TitleGer: QB-02 Semantische Genauigkeit
shortdesc: Genauigkeit bzgl. Bedeutung und Kontext in Daten
tags:
  - Qualitätsbaustein
ID:
  - QB-02
ListCritID:
  - "'QKB-03'"
  - "'QKB-06'"
  - "'QKB-04'"
  - "'QKB-07'"
share: true
---
## QB-02 Semantische Genauigkeit

### Beschreibung 

Semantische Genauigkeit bestimmt sich über die inhaltliche Korrektheit der Daten. Werden Katzen beispielsweise als Fahrzeuge klassifiziert, kann hier trotz allem eine syntaktische Korrektheit über das Format der Daten vorherrschen, allerdings sind die Inhalte inkorrekt. 

Während syntaktische Genauigkeit sicherstellt, dass ein Datenwert formal korrekt aufgebaut ist (z.B. korrektes Datumsformat „2025-04-11“), geht es bei semantischer Genauigkeit darum, dass der Inhalt des Werts bedeutungsmäßig richtig interpretiert werden kann.

Semantische Genauigkeit bezeichnet die Übereinstimmung von Daten mit ihrer beabsichtigten Bedeutung im jeweiligen Anwendungskontext. Im Gegensatz zu syntaktischer Genauigkeit lässt sich semantische Genauigkeit wesentlich schwieriger bewerten, da u.a. Domänenwissen dafür notwendig ist.
### Beispiele

- **Datenfeld:** `{"Geburtsdatum": "1990-01-01"}
    - Syntaktisch genau: Ja – korrektes Datumsformat nach ISO 8601
    - Semantisch genau: Nur, wenn dieses Datum tatsächlich das echte Geburtsdatum der Person ist.
        
- **Datenfeld:** `{"Alter": "25"}` (für eine Person, die 1990 geboren wurde und die Daten wurden 2025 erhoben)
    - Syntaktisch genau: Ja – eine ganze Zahl.
    - Semantisch ungenau: Ja – das Alter ist inhaltlich nicht plausibel, da die Person 35 Jahre (Geburtsdatum: 1990-01-01) alt sein müsste.

### Maßnahmen

| Maßnahme                      | Kurzbeschr.                                                  |
| ----------------------------- | ------------------------------------------------------------ |
| MA-05 Automatisierte Aufgaben | Skripte können wiederkehrende Aufgaben automatisieren        |
| MA-06_Expert Evaluation       | Ein Experte prüft die Daten manuell.                         |
| MA-07 Crowdsourcing           | Einbeziehung größerer Menschengruppen zur Prüfung der Daten. |
| MA-27 StatisticalBasics       | Sammelobjekt für statistische Grundlagen                     |




### Referenzen

| RefID | Verweis                                                                                                                                                       | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2     |  ISO 8000-8:2015 - Data quality — Part 8: Information and data quality: Concepts and measuring                                                                | Diese Norm bietet eine Übersicht über die Konzepte und Messmethoden für Datenqualität. Sie umfasst Genauigkeit als eines der wesentlichen Merkmale zur Bewertung der Datenqualität.                                                                                                                                                                                                                                                                                                                         |
| 10    |  ISO/TS 8000-81:2021 - Data quality — Part 81: Data quality assessment: Profiling                                                                             | Die ISO/TS 8000-81:2021 legt ein Verfahren für Datenprofiling zur Bewertung der Datenqualität fest, das sich auf Strukturanalyse, Spaltenanalyse und Beziehungsanalyse konzentriert. Sie ist auf tabellarische Daten anwendbar, behandelt jedoch keine Methoden zur Datenextraktion oder Regelableitung und kann sowohl eigenständig als auch zusammen mit Qualitätsmanagementsystem-Standards verwendet werden.                                                                                            |
| 11    |  ISO/TS 8000-82:2022 - Data quality — Part 82: Data quality assessment: Creating data rules                                                                   | Die ISO/TS 8000-82:2022 behandelt die Datenqualitätsbewertung durch Anwendung von Datenregeln auf verschiedene Datentypen, einschließlich Identifikatoren, Währungen und Datums-/Zeitangaben. Sie betont die Bedeutung von Datenprofiling bei der Formulierung effektiver Datenregeln, um die Integrität und Zuverlässigkeit von Daten in Informationssystemen sicherzustellen.                                                                                                                             |
| 16    |  ISO 19157-1:2023 - Geographic information — Data quality — Part 1: General requirements                                                                      | Dieses Dokument legt die Prinzipien zur Beschreibung der Qualität geografischer Daten fest, definiert ein System und Prozesse zur Beschreibung der Datenqualität, spezifiziert Qualitätsmesskomponenten, beschreibt Verfahren zur Qualitätsbewertung und Prinzipien zur Berichterstattung, ohne Mindestqualitätsniveaus festzulegen.                                                                                                                                                                        |
| 24    |  ISO/IEC 8183:2023 - Information technology — Artificial intelligence — Data life cycle framework                                                             | Das Dokument definiert die Phasen und Maßnahmen der Datenverarbeitung im Lebenszyklus von KI-Systemen und ist für alle Organisationen unabhängig von deren Art, Größe oder Natur anwendbar.                                                                                                                                                                                                                                                                                                                 |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods                                                     | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                                                                                                                                                                                                                                                         |
| 155   |  ISO 8000-110:2021 - Data quality — Part 110: Master data: Exchange of characteristic data: Syntax, semantic encoding, and conformance to data specification  | Das Dokument legt Anforderungen für den Austausch von Stammdatenmeldungen mit Fokus auf Syntax, semantische Kodierung und Datenspezifikationen fest und betont, dass diese allein nicht ausreichen, um die vollständige Datenqualität zu gewährleisten, da auch Aspekte wie Genauigkeit und Herkunft berücksichtigt werden müssen.                                                                                                                                                                          |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                                                 | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.                                                                                                                                                                                                                         |
| 190   |  Kriterienkatalog C5                                                                                                                                          | Der C5 (Cloud Computing Compliance Criteria Catalogue) des Bundesamts für Sicherheit in der Informationstechnik (BSI) stellt einen detaillierten Kriterienkatalog dar, der grundlegende Anforderungen an die Informationssicherheit von Cloud-Diensten festlegt.                                                                                                                                                                                                                                            |
| 192   |  Scaling Laws for Data Poisoning in LLMs                                                                                                                      | Aktuelle Untersuchungen zeigen, dass LLMs anfällig für Datenvergiftung sind, bei der maliziöse oder fehlerhafte Daten zu schädlichem Verhalten führen. Die Studie untersucht drei Bedrohungsmodelle: böswillige Feinabstimmung, schlechte Datenverwaltung und absichtliche Kontamination. Experimente an 23 LLMs zeigen, dass größere Modelle anfälliger sind und schädliches Verhalten schneller erlernen. Dies unterstreicht die Notwendigkeit stärkerer Schutzmaßnahmen im Zuge der Skalierung von LLMs. |




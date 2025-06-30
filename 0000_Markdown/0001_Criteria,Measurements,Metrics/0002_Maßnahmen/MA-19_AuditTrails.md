---
Name: MA-19_AuditTrails
Title: MA-19 AuditTrails
TitleGer: MA-19 Audit Trails
shortdesc: Audit Trails sind detaillierte, zeitlich geordnete Aufzeichnungen von Aktivitäten in einem System, die dazu dienen, Änderungen und Zugriffe nachvollziehbar zu dokumentieren. Sie sind entscheidend für die Sicherstellung von Transparenz, Sicherheit und Compliance in verschiedenen Bereichen, wie IT-Sicherheit und Qualitätsmanagement.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-19
ListMetricID: 
ListMeasureID:
  - "'QB-09'"
share: true
---
## MA-19 Audit-Trail

### Beschreibung

In einem Audit-Trail wird typischerweise festgehalten, wer eine konkrete Aktion durchgeführt hat, was genau gemacht wurde, wann es passiert ist und wo, sowie welche spezifischen Objekte betroffen waren. Dies kann die Identifikation von Benutzern umfassen, die sich an einem System angemeldet haben, Änderungen an Daten oder Konfigurationen, Dateizugriffe und andere kritische Aktionen.

Im Sinne der Nachverfolgbarkeit von Änderungen an Daten oder Modellen ist ein beständiges Mitschneiden (Logging) von Aktionen unumgänglich. Darüber hinaus erleichtert dies das Zurücksetzen auf einen älteren (funktionierenden) Stand (z.B. mittels Source-Code-Verwaltungstools).

Es muss eine Abgrenzung zu MA-22 Prozessdokumentation gemacht werden. Diese Maßnahme beschreibt, wie Prozesse für das bessere Verständnis dokumentiert werden, während hier die konkrete Aufzeichnung einer Handlung dokumentiert wird. 
### Beispiele 

#### Aktionen:

- Aktion 1: Datenerfassung
- Aktion 2: Datenbereinigung und -vorverarbeitung
- Aktion 3: Datenanreicherung
- Aktion 4: Änderungen und Aktualisierungen des Datensatzes

#### Audit-Trail-Einträge

- Datenerfassung
    - Zeitstempel: 2024-08-01 08:00:00
    - Benutzer: Dr. Eva Müller (Mitarbeiter-ID: 112233)
    - Aktion: Datenerfassung
    - Details: Erfassung von Patientendaten aus Krankenhaus A, 5000 Datensätze aufgenommen.

- Datenbereinigung
    - Zeitstempel: 2024-08-02 09:15:30
    - Benutzer: Datenanalyst Max Weber (Mitarbeiter-ID: 334455)
    - Aktion: Datenbereinigung
    - Details: Entfernen von unvollständigen Datensätzen und Korrektur von Dateninkonsistenzen, 200 Datensätze entfernt.

- Datenanreicherung
    - Zeitstempel: 2024-08-03 10:45:00
    - Benutzer: Data Scientist Laura Schmidt (Mitarbeiter-ID: 556677)
    - Aktion: Datenanreicherung
    - Details: Anreicherung des Datensatzes mit externen Wetterdaten, 5000 Datensätze aktualisiert.

- Datenaktualisierung
    - Zeitstempel: 2024-08-05 11:30:45
    - Benutzer: Dr. Eva Müller (Mitarbeiter-ID: 112233)
    - Aktion: Datenaktualisierung
    - Details: Aktualisierung von 300 Datensätzen aufgrund neuer Labortestergebnisse.



### Referenzen

| RefID | Verweis                                                                                                                                            | Kurzbeschr.                                                                                                                                                                                                                                                                                         |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7     |  ISO 8000-63:2019 - Data quality — Part 63: Data quality management: Process measurement                                                           | Die ISO 8000-63 ist eine 2019 veröffentlichte Norm, die Richtlinien zur Messung und Verbesserung von Datenqualitätsmanagementprozessen bietet, einschließlich Reifegradmodellen und Inspektionsplänen, um Unternehmen bei der effektiven Steuerung ihrer Datenqualitätsinitiativen zu unterstützen. |
| 14    |  ISO 8000-150:2022 - Data quality — Part 150: Data quality management: Roles and responsibilities                                                  | Dieses Dokument legt die wichtigsten Überlegungen für die Festlegung von Rollen und Verantwortlichkeiten im Datenqualitätsmanagement fest und bietet ein Rahmenwerk sowie Beispiel-Szenarien zur Implementierung.                                                                                   |
| 15    |  ISO 9001:2015 - Quality management systems                                                                                                        | ISO 9001 ist eine weltweit anerkannte Norm für Qualitätsmanagement, die Organisationen dabei unterstützt, ihre Leistung zu verbessern, Kundenerwartungen zu erfüllen, Prozesse zu optimieren und durch regelmäßige Audits langfristigen Erfolg zu sichern.                                          |
| 21    |  ISO/IEC 5338:2023 - Information technology — Artificial intelligence — AI system life cycle processes                                             | Standardisiertes Verfahren und Rahmenwerk zur Sicherstellung der Datenqualität für Analytik und maschinelles Lernen einschließlich spezifischer Prozesse und Leitlinien gemäß den ISO/IEC 5259-Standards.                                                                                           |
| 36    |  ISO/IEC 27001:2022 - Information security management systems                                                                                      | Während dieser Standard primär auf Informationssicherheitsmanagement abzielt, enthält er auch Bestimmungen zur Sicherstellung der Integrität und Vertraulichkeit von Daten, die für Trainingsdaten von Bedeutung sind.                                                                              |
| 143   |  ISO/IEC 27701:2019 - Extension to ISO/IEC 27001 and ISO/IEC 27002 for privacy information management                                              | Sicherheitstechniken – Erweiterung auf ISO/IEC 27001 und ISO/IEC 27002 für das Datenschutzinformationsmanagement – ​​Anforderungen und Richtlinien                                                                                                                                                  |
| 151   |  ISO/IEC FDIS 5259-5 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 5: Data quality governance framework  | Ein Framework zur Implementierung und Überwachung von Datenqualitätsmaßnahmen im gesamten Lebenszyklus von Analyse- und ML-Projekten, ohne dabei Management- oder Prozessvorgaben aus ISO 5259-3/4 zu wiederholen.                                                                                  |
| 173   |  OWASP - Development-time threats – AI Exchange                                                                                                    | Die OWASP-Seite beschreibt Risiken während der Entwicklung von KI-Systemen, wie Datenvergiftung, geistigen Diebstahl und Supply-Chain-Angriffe. Sie empfiehlt Schutzmaßnahmen wie Verschlüsselung, Datenisolation und Integritätsprüfungen, um Modelle und Daten zu sichern.                        |
| 179   |  DAMA-DMBOK: data management body of knowledge                                                                                                     | Der DAMA-DMBOK2-Leitfaden bietet Fach- und Führungskräften einen umfassenden Rahmen für alle Bereiche des Datenmanagements – von Governance über Architektur, Entwicklung, Betrieb, Sicherheit und Qualität bis hin zu Business Intelligence, Metadaten und beruflicher Weiterbildung.              |
| 181   |  Data Quality Toolkit: Automatic assessment of data quality and remediation for machine learning datasets                                          | Das Data Quality Toolkit hilft dabei, Probleme mit Daten für maschinelles Lernen zu erkennen und zu beheben, indem es Bewertungen automatisiert und die Datenvorbereitung beschleunigt. Es ist über den IBM API Hub verfügbar, mit Tutorials auf dem IBM Learning Path.                             |
| 247   |  Data version control                                                                                                                              | Die Datenversionskontrolle ist ein System zum Verwalten und Nachverfolgen von Änderungen an Datensätzen, das für Datenanalyse und Forschung optimiert ist. Es bietet Funktionen, die speziell für die Handhabung großer Datensätze konzipiert sind und die Zusammenarbeit erleichtern.              |

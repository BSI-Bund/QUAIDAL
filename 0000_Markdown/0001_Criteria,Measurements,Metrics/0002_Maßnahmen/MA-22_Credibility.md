---
Name: MA-22 Vertrauenswürdigkeit
Title: MA-22 Vertrauenswürdigkeit
TitleGer: MA-22 Vertrauenswürdigkeit
shortdesc: Glaubwürdigkeit, Vertrauenswürdigkeit der Datenquelle muss bestätigt werden
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-22
ListMetricID: 
ListMeasureID:
  - "'QB-14'"
  - "'QB-09'"
share: true
---
## MA-22 Vertrauenswürdigkeit

### Beschreibung

Die Beurteilung der Glaubwürdigkeit von Trainingsdaten muss im spezifischen Nutzungskontext durchgeführt werden. Der Kontext kann hier jeweils auf das einzelne Datenobjekt, verwandte Datenobjekte oder den gesamten Datensatz gelegt werden. Im Fokus muss auch auf die potenzielle Störung des Verarbeitungsablaufs durch versehentliche oder böswillige Veränderung stehen. Wenn im Verarbeitungsprozess Datenveränderungen durchgeführt werden, um Fehler zu korrigieren oder Lücken zu füllen, dürfen diese keinen Einfluss auf die Glaubwürdigkeit der Daten haben. Es ist wichtig, dass auch durch andere Maßnahmen (bspw. Data-Imputation) die Glaubwürdigkeit erhalten bleibt. 


### Beispiele 

#### Beispiel 1 - Datenquellenprüfung

Sicherstellen, dass die Daten aus vertrauenswürdigen und anerkannten Quellen stammen. Zum Beispiel, wenn man medizinische Daten verwendet, sollten diese von zertifizierten Gesundheitsorganisationen stammen.

#### Beispiel 2 - Datenintegritätsprüfung

Überprüfung der Datenintegrität, indem man sicherstellt, dass die Daten nicht manipuliert oder unvollständig sind. Bei Finanzdaten könnte dies bedeuten, dass Transaktionsdaten auf Vollständigkeit und Konsistenz geprüft werden.

#### Beispiel 3 - Kreuzvalidierung mit anderen Datensätzen

Vergleichen des Trainingsdatensatzes mit anderen ähnlichen Datensätzen, um dessen Konsistenz und Zuverlässigkeit zu bestätigen. In der Praxis könnte dies bedeuten, dass ein medizinischer Datensatz mit anderen Studien oder Datensätzen verglichen wird, um Konsistenz zu gewährleisten.


### Metriken & Methoden

| ID                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-15 SixSigmaProcess | Werkzeuge zur Prozessverbesserung und Qualitätskontrolle.                                                                                                                                                                                                                                                                                                                                     |
| QM-43 Kreuzabgleich   | Ergebnisprüfung durch Kreuzabgleich verschiedener Quellen.                                                                                                                                                                                                                                                                                                                                    |
| QM-65_AI_or_S_Bom     | Eine SBOM (Software Bill of Materials) und ihr KI-Pendant, der AIBOM, bieten eine umfassende und transparente Dokumentation aller Komponenten, Abhängigkeiten und Prozessinformationen – inklusive Sicherheitslücken, Versions- und Lizenzdetails sowie ethischer und Compliance-Aspekte – um potenzielle Risiken in der Software- bzw. KI-Lieferkette frühzeitig zu erkennen und zu mindern. |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                  | Kurzbeschr.                                                                                                                                                                                                                                                                                         |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 4     |  ISO 8000-61:2016 - Data quality — Part 61: Data quality management: Process reference model                                                                                                                                                                             | Das Dokument beschreibt den Datenqualitätsmanagementprozess als steuerbaren, wiederholbaren und verbesserbaren Ablauf (PDCA), betont die kontinuierliche Verbesserung der Daten bei Fehlern und die Einbeziehung verschiedener Stakeholder wie Nutzer, Management und Datenmanager.                 |
| 7     |  ISO 8000-63:2019 - Data quality — Part 63: Data quality management: Process measurement                                                                                                                                                                                 | Die ISO 8000-63 ist eine 2019 veröffentlichte Norm, die Richtlinien zur Messung und Verbesserung von Datenqualitätsmanagementprozessen bietet, einschließlich Reifegradmodellen und Inspektionsplänen, um Unternehmen bei der effektiven Steuerung ihrer Datenqualitätsinitiativen zu unterstützen. |
| 14    |  ISO 8000-150:2022 - Data quality — Part 150: Data quality management: Roles and responsibilities                                                                                                                                                                        | Dieses Dokument legt die wichtigsten Überlegungen für die Festlegung von Rollen und Verantwortlichkeiten im Datenqualitätsmanagement fest und bietet ein Rahmenwerk sowie Beispiel-Szenarien zur Implementierung.                                                                                   |
| 21    |  ISO/IEC 5338:2023 - Information technology — Artificial intelligence — AI system life cycle processes                                                                                                                                                                   | Standardisiertes Verfahren und Rahmenwerk zur Sicherstellung der Datenqualität für Analytik und maschinelles Lernen einschließlich spezifischer Prozesse und Leitlinien gemäß den ISO/IEC 5259-Standards.                                                                                           |
| 28    |  ISO/IEC 22989:2022 - Information technology — Artificial intelligence — Artificial intelligence concepts and terminology                                                                                                                                                | Dieser Standard definiert die grundlegenden Konzepte und die Terminologie im Bereich der künstlichen Intelligenz, einschließlich der Aspekte der Datenqualität und Ausgewogenheit von Trainingsdaten.                                                                                               |
| 36    |  ISO/IEC 27001:2022 - Information security management systems                                                                                                                                                                                                            | Während dieser Standard primär auf Informationssicherheitsmanagement abzielt, enthält er auch Bestimmungen zur Sicherstellung der Integrität und Vertraulichkeit von Daten, die für Trainingsdaten von Bedeutung sind.                                                                              |
| 40    |  ISO/IEC TR 24027:2021 - Information technology — Artificial intelligence (AI) — Bias in AI systems and AI aided decision making                                                                                                                                         | Der Bericht untersucht Bias in KI-Systemen und betont, dass hochwertige Trainingsdaten essenziell sind, um Verzerrungen zu reduzieren und faire, gerechte Entscheidungen zu ermöglichen.                                                                                                            |
| 86    |  KI-Prüfkatalog: Leitfaden zur Gestaltung vertrauenswürdiger Künstlicher Intelligenz                                                                                                                                                                                     | Der Fraunhofer KI-Prüfkatalog ist ein kostenfreier Leitfaden zur Gestaltung vertrauenswürdiger Künstlicher Intelligenz. Er unterstützt Entwickler*innen bei der Gestaltung und KI-Prüfer*innen bei der Evaluation und Qualitätssicherung neuer und bestehender KI-Anwendungen.                      |
| 151   |  ISO/IEC FDIS 5259-5 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 5: Data quality governance framework                                                                                                                        | Ein Framework zur Implementierung und Überwachung von Datenqualitätsmaßnahmen im gesamten Lebenszyklus von Analyse- und ML-Projekten, ohne dabei Management- oder Prozessvorgaben aus ISO 5259-3/4 zu wiederholen.                                                                                  |
| 227   |  Operations Bill of Materials (OBOM)                                                                                                                                                                                                                                     | Die Operations Bill of Materials (OBOM) von CycloneDX ermöglicht eine umfassende Dokumentation und dynamische Aktualisierung von Laufzeitumgebungen, einschließlich Hardware, Firmware und Anwendungen, unabhängig von der Software-BOM (SBOM).                                                     |
| 237   |  Digital Services Act - Verordnung (EU) 2022/2065 des Europäischen Parlaments und des Rates vom 19. Oktober 2022 über einen Binnenmarkt für digitale Dienste und zur Änderung der Richtlinie 2000/31/EG (Gesetz über digitale Dienste) (Text von Bedeutung für den EWR)  | Die Verordnung (EU) 2022/2065 über digitale Dienste harmonisiert Vorschriften für Vermittlungsdienste in der EU, stärkt den Schutz von Grundrechten, bekämpft rechtswidrige Inhalte und schafft ein sicheres, transparentes Online-Umfeld.                                                          |
| 247   |  Data version control                                                                                                                                                                                                                                                    | Die Datenversionskontrolle ist ein System zum Verwalten und Nachverfolgen von Änderungen an Datensätzen, das für Datenanalyse und Forschung optimiert ist. Es bietet Funktionen, die speziell für die Handhabung großer Datensätze konzipiert sind und die Zusammenarbeit erleichtern.              |

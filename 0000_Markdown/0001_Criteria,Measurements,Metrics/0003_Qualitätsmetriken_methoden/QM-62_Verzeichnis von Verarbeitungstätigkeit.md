---
Name: QM-62_Verzeichnis von Verarbeitungstätigkeit
Title: QM-62 Verzeichnis von Verarbeitungstätigkeit
TitleGer: QM-62 Verzeichnis von Verarbeitungstätigkeit
shortdesc: Erfassung und regelmäßige Aktualisierung von Verarbeitungstätigkeiten, Zwecken, betroffenen Personengruppen, Empfängern, Löschfristen, Sicherheitsmaßnahmen und Rechtsgrundlagen, einschließlich der Implementierung eines Datenschutz-Managementsystems und Schulungen für Mitarbeiter.
tags:
  - Qualitätsmetrik
ID:
  - QM-62
ListMetricID: 
ListMeasureID:
  - "'MA-20'"
MID: 
type:
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-62 Verzeichnis von Verarbeitungstätigkeit

### Beschreibung

Verantwortliche und gegebenenfalls Auftragsverarbeiter müssen ein Verzeichnis aller Verarbeitungstätigkeiten führen, die ihrer Zuständigkeit unterliegen. Dieses Verzeichnis dient der Dokumentation und muss verschiedene Informationen enthalten, wie:

- Name und Kontaktdaten des Verantwortlichen, Auftragsverarbeiters und eines etwaigen Datenschutzbeauftragten.
- Zweck der Datenverarbeitung.
- Kategorien betroffener Personen und der verarbeiteten personenbezogenen Daten.
- Empfänger der Daten, einschließlich Übermittlungen an Drittländer oder internationale Organisationen.
- Gegebenenfalls vorgesehene Löschfristen der Daten.
- Technische und organisatorische Maßnahmen zum Schutz der Daten (gemäß Artikel 32 DSGVO).

#### Relevanz für Trainingsdaten:

Für die Haltung und Verwaltung von Trainingsdaten bedeutet dies, dass Unternehmen, die personenbezogene Daten für KI-Modelle verwenden, ein detailliertes Verzeichnis aller Verarbeitungsschritte führen müssen. Es ist entscheidend, dass alle relevanten Informationen zur Herkunft, Empfängern und Schutzmaßnahmen der Trainingsdaten dokumentiert sind, um die Transparenz und Rechenschaftspflicht gemäß der DSGVO sicherzustellen. Auch die Löschfristen und Datenschutzmaßnahmen sollten berücksichtigt werden, um den gesetzlichen Anforderungen zu genügen.

### Beispiele 

#### Beispiel 1 - Verzeichnis für ein Unternehmen, das Kundendaten für ein Empfehlungs-KI-Modell verarbeitet

##### Verantwortlicher:  
Name: XYZ AI Solutions GmbH  
Kontaktdaten: info@xyzai.de  
Datenschutzbeauftragter: datenschutz@xyzai.de

##### Zweck der Verarbeitung:  
Entwicklung eines KI-Modells zur Personalisierung von Produktempfehlungen auf Grundlage von Kundendaten.

##### Kategorien betroffener Personen:  
Kunden der XYZ AI Solutions GmbH (Personen, die die E-Commerce-Plattform nutzen).

##### Kategorien personenbezogener Daten:

- Name, E-Mail-Adresse, Kundennummer
- Kaufhistorie (Produktkategorien, Kaufdaten, Warenkorb)
- Website-Interaktionen (Klicks, besuchte Seiten, Produktansichten)

##### Kategorien von Empfängern:

- Marketingabteilung (zur Erstellung von personalisierten Angeboten)
- Technischer Dienstleister für KI-Modelltraining (Drittland, USA) – Datenübermittlung gemäß Standardvertragsklauseln.

##### Übermittlung an Drittländer oder internationale Organisationen:  
Datenübermittlung an den technischen Dienstleister in den USA unter Verwendung von Standardvertragsklauseln (gemäß Art. 49 DSGVO).

##### Vorgesehene Löschfristen:

- Kundendaten werden 3 Jahre nach dem letzten Kauf gelöscht.
- Nicht abgeschlossene Warenkörbe werden nach 30 Tagen anonymisiert.

##### Technische und organisatorische Maßnahmen:

- Datenverschlüsselung bei der Übertragung und Speicherung.
- Pseudonymisierung der Kundendaten für das Modelltraining.
- Zugriffsbeschränkungen auf die Daten nur für berechtigte Mitarbeiter.

#### Beispiel 2 - Verzeichnis für ein Forschungsprojekt zur Gesichtserkennung in der Gesundheitsversorgung

##### Verantwortlicher:  
Name: Medical AI Research Institute  
Kontaktdaten: research@medicalai.org  
Datenschutzbeauftragter: dpo@medicalai.org

##### Zweck der Verarbeitung:  
Trainieren eines KI-Modells zur Erkennung von Krankheitsmerkmalen in Gesichtern zur Diagnoseunterstützung.

##### Kategorien betroffener Personen:  
Patienten, die an der klinischen Studie teilnehmen.

##### Kategorien personenbezogener Daten:
- Gesichtsbilder
- Gesundheitsdaten (Diagnosen, Symptome)
- Geschlecht, Alter

##### Kategorien von Empfängern:

- Forschungsteams innerhalb des Medical AI Research Institute.
- Partnerkrankenhäuser im EU-Raum für diagnostische Tests.

##### Übermittlung an Drittländer oder internationale Organisationen:  
Keine Übermittlungen an Drittländer.

##### Vorgesehene Löschfristen:

- Gesichtsbilder und Gesundheitsdaten werden 10 Jahre nach Abschluss der Studie gelöscht.
- Anonymisierte Daten bleiben für wissenschaftliche Analysen unbegrenzt erhalten.

##### Technische und organisatorische Maßnahmen:

- Speicherung der Daten in einer gesicherten Cloud mit Zugangsbeschränkungen.
- Gesichtsbilder werden nach dem Modelltraining pseudonymisiert.
- Regelmäßige Sicherheitsprüfungen und Audits zum Schutz der Datenintegrität.


### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 36    |  ISO/IEC 27001:2022 - Information security management systems                                                                                                                                                                                                                                                                                                                                                                                                   | Während dieser Standard primär auf Informationssicherheitsmanagement abzielt, enthält er auch Bestimmungen zur Sicherstellung der Integrität und Vertraulichkeit von Daten, die für Trainingsdaten von Bedeutung sind.                                                                                                                                                                                                                                               |
| 128   |  DSGVO - Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (Datenschutz-Grundverordnung) (Text von Bedeutung für den EWR)                                                                                                                                                   | Die DSGVO (Datenschutz-Grundverordnung) ist eine EU-Verordnung, die den Schutz personenbezogener Daten regelt. Sie stärkt die Rechte von Einzelpersonen und legt strenge Anforderungen an Unternehmen und Organisationen zur Verarbeitung und Sicherheit von Daten fest. Sie gilt seit Mai 2018 in allen EU-Staaten.                                                                                                                                                 |
| 143   |  ISO/IEC 27701:2019 - Extension to ISO/IEC 27001 and ISO/IEC 27002 for privacy information management                                                                                                                                                                                                                                                                                                                                                           | Sicherheitstechniken – Erweiterung auf ISO/IEC 27001 und ISO/IEC 27002 für das Datenschutzinformationsmanagement – ​​Anforderungen und Richtlinien                                                                                                                                                                                                                                                                                                                   |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                                                                                                                                                                                                                                                                                                                                                   | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.                                                                                                                                                                                  |
| 235   |  Data Governance Act - Regulation (EU) 2022/868 of the European Parliament and of the Council of 30 May 2022 on European data governance and amending Regulation (EU) 2018/1724 (Data Governance Act) (Text with EEA relevance)                                                                                                                                                                                                                                 | Die Verordnung (EU) 2022/868 über europäische Daten-Governance schafft einen harmonisierten Rahmen für die Nutzung und Weiterverwendung von Daten in der EU, um Innovation und einen digitalen Binnenmarkt zu fördern. Sie regelt gemeinsame Datenräume, sichere Datenweiterverwendung, freiwilligen Datenaltruismus und neutrale Datenvermittlungsdienste, wobei Datenschutz und Grundrechte gewährleistet bleiben.                                                 |
| 260   |  AI-Act - Verordnung (EU) 2024/1689 des Europäischen Parlaments und des Rates vom 13. Juni 2024 zur Festlegung harmonisierter Vorschriften für künstliche Intelligenz und zur Änderung der Verordnungen (EG) Nr. 300/2008, (EU) Nr. 167/2013, (EU) Nr. 168/2013, (EU) 2018/858, (EU) 2018/1139 und (EU) 2019/2144 sowie der Richtlinien 2014/90/EU, (EU) 2016/797 und (EU) 2020/1828 (Verordnung über künstliche Intelligenz) (Text von Bedeutung für den EWR)  | Der AI Act reguliert KI-Systeme nach Risikostufen, fordert für hochriskante Anwendungen strenge Vorgaben und setzt auf Transparenz und Menschenrechtsschutz. Artikel 10 verlangt qualitativ hochwertige, dokumentierte Datensätze, um faire und vertrauenswürdige KI zu gewährleisten.                                                                                                                                                                               |
| 284   |  BSI - IT-Grundschutz-Kompendium                                                                                                                                                                                                                                                                                                                                                                                                                                | Der BSI IT-Grundschutz ist ein standardisiertes Konzept des BSI, das Organisationen durch modulare Bausteine und standardisierte Maßnahmen einen effizienten Aufbau und Nachweis eines Informationssicherheitsmanagementsystems ermöglicht, um IT-Systeme kostengünstig und praxisnah vor Bedrohungen zu schützen.                                                                                                                                                   |
| 301   |  GDPR and Large Language Models: Technical and Legal Obstacles                                                                                                                                                                                                                                                                                                                                                                                                  | Große Sprachmodelle (LLMs) stehen im Spannungsfeld zur DSGVO, da ihre undurchsichtige Struktur zentrale Rechte wie Auskunft oder Löschung erschwert. Das Papier untersucht technische Lösungen wie Machine Unlearning, erklärbare KI und differenzielle Privatsphäre sowie ein vierstufiges Governance-Modell für Datenschutz und Compliance. Ziel ist es, eine praxisnahe Verbindung zwischen moderner KI-Technologie und den Anforderungen der DSGVO herzustellen. |


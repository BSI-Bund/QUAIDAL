---
Name: QKB-10 Daten mit Personenbezug
Title: QKB-10 Daten mit Personenbezug
TitleGer: QKB-10 Daten mit Personenbezug
shortdesc: Prüfung ob Trainingsdaten personenbezogene Daten enthalten
tags:
  - Qualitätskriterien
ID:
  - QKB-10
ListMeasureID: 
ListCritID: 
share: true
---
## QKB-10 Daten mit Personenbezug

### Beschreibung 

Aus Sicht diverser grundlegender gesetzlicher Regelungen müssen Datensätze auf den Gehalt von personenbezogenen Informationen geprüft werden. Eine umfassende Überprüfung der Datensätze nach personenbezogenen Datensätzen ist hierfür ebenso wichtig wie die kontrollierte und nachweisbare Entfernung der Datensätze, die in den Datensätzen vorhanden sind.


### Beispiele

#### Beispiel 1: Datenschutz
Personenbezogene Daten unterliegen Datenschutzgesetzen wie der DSGVO in der Europäischen Union. Die Verarbeitung erfordert diverse Maßnahmen um die grundlegenden Anforderungen dieser Richtlinie umzusetzen. 



### Bausteine

| Baustein                | Kurzbeschr.                                                                                                                                                                                                                               |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QB-09 Quellenmanagement | Organisation und Überwachung der Datenherkunft für Qualität und Integrität.                                                                                                                                                               |
| QB-10_DataChecks        | Überprüfung von Trainingsdaten sichert Qualität vor dem Modelltraining.                                                                                                                                                                   |
| QB-11 Prozesse          | Dokumentation sichert Abläufe und Prozesse in IT-Infrastruktur und Softwareentwicklung.                                                                                                                                                   |
| QB-14_Expertanalysis    | Die Expertenanalyse ist ein Allzweckwerkzeug um die Qualität eines Trainingsdatensatzes hinsichtlich bestimmter Kriterien zu prüfen. Idealerweise werden dafür mehrere Expert\*innen unabhängig voneinander um eine Einschätzung gebeten. |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                                                        | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                        |
| ----- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 296   |  Bias in der künstlichen Intelligenz                                                                                                                                                                                                                                                                           | Das Dokument Bias in der künstlichen Intelligenz befasst sich mit den Grundlagen und zeigt Detektion und Mitigationsmechanismen auf um Bias in den eigenen Datensätzen auf die Spur zu kommen.                                                                                                                                                                                                                     |
| 223   |  The Assessment List for Trustworthy Artificial Intelligence (ALTAI) for self assessment                                                                                                                                                                                                                       | Im Jahr 2019 veröffentlichte die hochrangige KI-Expertengruppe der Europäischen Kommission *Ethikrichtlinien für vertrauenswürdige KI*, einschließlich einer Bewertungsliste zur Bewertung von KI-Systemen auf der Grundlage von sieben Schlüsselanforderungen: menschliche Handlungsfähigkeit, technische Robustheit, Datenschutz, Transparenz, Fairness, gesellschaftliches Wohlergehen. Sein und Verantwortung. |
| 206   |  Open Data Act                                                                                                                                                                                                                                                                                                 | RICHTLINIE  (EU)  2019/  1024  DES  EUROPÄISCHEN  PARLAMENTS  UND  DES  RATES  -  vom  20. Juni  2019  -  über  offene  Daten  und  die  Weiterverwendung  von  Informationen  des  öffentlichen  Sektors                                                                                                                                                                                                          |
| 187   |  Extracting Training Data from Large Language Models                                                                                                                                                                                                                                                           | Das Papier zeigt, dass große Sprachmodelle wie GPT-2 anfällig für Datenextraktionsangriffe sind, bei denen sensible Informationen aus den Trainingsdaten wiederhergestellt werden können. Größere Modelle sind dabei besonders gefährdet. Die Autoren schlagen Schutzmaßnahmen vor, um dieses Risiko zu verringern.                                                                                                |
| 128   |  DSGVO - Verordnung (EU) 2016/679 des Europäischen Parlaments und des Rates vom 27. April 2016 zum Schutz natürlicher Personen bei der Verarbeitung personenbezogener Daten, zum freien Datenverkehr und zur Aufhebung der Richtlinie 95/46/EG (Datenschutz-Grundverordnung) (Text von Bedeutung für den EWR)  | Die DSGVO (Datenschutz-Grundverordnung) ist eine EU-Verordnung, die den Schutz personenbezogener Daten regelt. Sie stärkt die Rechte von Einzelpersonen und legt strenge Anforderungen an Unternehmen und Organisationen zur Verarbeitung und Sicherheit von Daten fest. Sie gilt seit Mai 2018 in allen EU-Staaten.                                                                                               |
| 127   |  BDSG                                                                                                                                                                                                                                                                                                          | Das Bundesdatenschutzgesetz (BDSG) schützt personenbezogene Daten in Deutschland und ergänzt die EU-Datenschutz-Grundverordnung (DSGVO). Es regelt, wie Daten von öffentlichen und privaten Stellen verarbeitet werden dürfen, definiert Rechte der Betroffenen wie Auskunft und Löschung und legt Pflichten für Datenverantwortliche fest, z. B. zur Datensicherheit.                                             |
| 36    |  ISO/IEC 27001:2022 - Information security management systems                                                                                                                                                                                                                                                  | Während dieser Standard primär auf Informationssicherheitsmanagement abzielt, enthält er auch Bestimmungen zur Sicherstellung der Integrität und Vertraulichkeit von Daten, die für Trainingsdaten von Bedeutung sind.                                                                                                                                                                                             |

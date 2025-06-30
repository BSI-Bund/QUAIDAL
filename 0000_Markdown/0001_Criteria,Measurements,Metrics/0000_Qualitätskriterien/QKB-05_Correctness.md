---
Name: QKB-05 Korrektheit
Title: QKB-05 Korrektheit
TitleGer: QKB-05 Korrektheit
shortdesc: Korrektheit in Bezug auf Trainingsdaten bedeutet, dass die Daten reelle, der Wirklichkeit entsprechende (oder die Wirklichkeit simulierende) Werte oder im Rahmen des Einsatzzwecks als Wahr gelabelte Werte enthalten müssen.
tags:
  - Qualitätskriterien
ID:
  - QKB-05
ListMeasureID: 
ListCritID: 
share: true
---

## QKB-05 Korrektheit

### Beschreibung 

KI-Modelle sammeln im Lernprozess Korrelationen auf den Daten. Falsche Daten können die Leistung eines KI-Modells oder Machine-Learning-Algorithmus erheblich beeinflussen. Korrektheit beschreibt, inwieweit Daten inhaltlich richtig sind – das heißt, ob sie die Realität oder einen als gültig anerkannten Zustand fehlerfrei widerspiegeln. Korrekte Daten entsprechen entweder tatsächlich gemessenen Werten, externen Referenzquellen oder als „wahr“ gekennzeichneten Informationen im Anwendungskontext (z.B. Labels in Trainingsdaten).

Korrektheit erfordert die Abwesenheit von inhaltlichen Fehlern, unabhängig davon, wie präzise oder vollständig die Daten sind.

Häufig genutzte Synonyme für "Korrektheit" sind Konsistenz (siehe Abgrenzung zu Konsistenz), Konformität und Uniformität.

Das Kriterium "Korrektheit" muss gegen "Genauigkeit" abgrenzt werden. Genauigkeit bezieht sich auf das Maß oder die Vorhersage in dem eine Messung den tatsächlichen Wert widerspiegelt. Es handelt sich also um die Nähe der berechneten Werte zu den tatsächlichen (wahren) Werten. 
"Korrektheit" hingegen bezieht sich auf die Abwesenheit von Fehlern in einem bestimmten Kontext. Sie konzentriert sich darauf, ob die Daten einem Satz vordefinierter Regeln oder Erwartungen ohne Fehler entsprechen. 

### Beispiele

#### Beispiel 1: Korrektheit von Kundendaten

In einem CRM-System (Customer Relationship Management) ist Korrektheit entscheidend, um sicherzustellen, dass die Kundeninformationen exakt und aktuell sind. Wenn ein Kunde beispielsweise seine Adresse ändert, muss diese Änderung korrekt und zeitnah im System eingetragen werden, um sicherzustellen, dass alle nachfolgenden Kommunikation und Lieferungen an die richtige Adresse erfolgen. Fehlerhafte Adressdaten könnten dazu führen, dass wichtige Dokumente oder Produkte an die falsche Adresse gesendet werden, was Kundenunzufriedenheit und zusätzliche Kosten zur Folge haben könnte

#### Beispiel 2: Korrektheit in medizinischen Daten

In einem Krankenhausinformationssystem müssen die Patientendaten absolut korrekt sein, um eine ordnungsgemäße medizinische Versorgung zu gewährleisten. Zum Beispiel müssen die Angaben zu Allergien, Medikation und Krankengeschichte eines Patienten korrekt und vollständig in den Akten verzeichnet sein. Ein Fehler, wie die falsche Angabe einer Allergie, könnte zu schwerwiegenden gesundheitlichen Folgen führen, wenn dem Patienten ein Medikament verabreicht wird, auf das er allergisch reagiert.



### Bausteine

| Baustein                 | Kurzbeschr.                                                                                                                                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QB-09 Quellenmanagement  | Organisation und Überwachung der Datenherkunft für Qualität und Integrität.                                                                                                                                                               |
| QB-10_DataChecks         | Überprüfung von Trainingsdaten sichert Qualität vor dem Modelltraining.                                                                                                                                                                   |
| QB-12_FeatureEngineering | Feature Engineering wandelt Rohdaten um, verbessert ML-Modelle durch relevante, generalisierbare, skalierbare Features.                                                                                                                   |
| QB-14_Expertanalysis     | Die Expertenanalyse ist ein Allzweckwerkzeug um die Qualität eines Trainingsdatensatzes hinsichtlich bestimmter Kriterien zu prüfen. Idealerweise werden dafür mehrere Expert\*innen unabhängig voneinander um eine Einschätzung gebeten. |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Kurzbeschr.                                                                                                                                                                                                                                                                            |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2     |  ISO 8000-8:2015 - Data quality — Part 8: Information and data quality: Concepts and measuring                                                                                                                                                                                                                                                                                                                                                                  | Diese Norm bietet eine Übersicht über die Konzepte und Messmethoden für Datenqualität. Sie umfasst Genauigkeit als eines der wesentlichen Merkmale zur Bewertung der Datenqualität.                                                                                                    |
| 17    |  ISO/IEC 5259-1:2024 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 1: Overview, terminology, and examples                                                                                                                                                                                                                                                                                                             | Dieser Standard bietet eine Übersicht und definiert die Terminologie sowie Beispiele zur Datenqualität im Kontext von Analytik und maschinellem Lernen. Er adressiert die Bedeutung der Ausgewogenheit von Trainingsdaten als Teil der Datenqualitätsanforderungen.                    |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model                                                                                                                                                                                                                                                                                                                                 | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                       |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                                                                                                                                                                                                                                                                                                                                                   | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.    |
| 206   |  Open Data Act                                                                                                                                                                                                                                                                                                                                                                                                                                                  | RICHTLINIE  (EU)  2019/  1024  DES  EUROPÄISCHEN  PARLAMENTS  UND  DES  RATES  -  vom  20. Juni  2019  -  über  offene  Daten  und  die  Weiterverwendung  von  Informationen  des  öffentlichen  Sektors                                                                              |
| 260   |  AI-Act - Verordnung (EU) 2024/1689 des Europäischen Parlaments und des Rates vom 13. Juni 2024 zur Festlegung harmonisierter Vorschriften für künstliche Intelligenz und zur Änderung der Verordnungen (EG) Nr. 300/2008, (EU) Nr. 167/2013, (EU) Nr. 168/2013, (EU) 2018/858, (EU) 2018/1139 und (EU) 2019/2144 sowie der Richtlinien 2014/90/EU, (EU) 2016/797 und (EU) 2020/1828 (Verordnung über künstliche Intelligenz) (Text von Bedeutung für den EWR)  | Der AI Act reguliert KI-Systeme nach Risikostufen, fordert für hochriskante Anwendungen strenge Vorgaben und setzt auf Transparenz und Menschenrechtsschutz. Artikel 10 verlangt qualitativ hochwertige, dokumentierte Datensätze, um faire und vertrauenswürdige KI zu gewährleisten. |

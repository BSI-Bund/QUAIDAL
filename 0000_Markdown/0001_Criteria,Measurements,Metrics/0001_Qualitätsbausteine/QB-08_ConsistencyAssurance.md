---
Name: QB-08 Konsistenzsicherung
Title: QB-08 Konsistenzsicherung
TitleGer: QB-08 Konsistenzsicherung
shortdesc: Einheitliche, widerspruchsfreie Datenformate und -werte gewährleisten.
tags:
  - Qualitätsbaustein
ID:
  - QB-08
ListCritID:
  - "'QKB-06'"
  - "'QKB-04'"
share: true
---
## QB-08 Konsistenzsicherung

### Beschreibung

Die Sicherstellung der Konsistenz der Daten (z.B. auf Basis von Attributen, Anzahl an Datenpunkten, im zeitlichen Verlauf, ...) kann durch viele Maßnahmen erfolgen. Einheitliche oder vordefinierte Formate und Typen sind diesem Umstand dienlich. Standardisierte Formate und automatisierte Prüfmechanismen erkennen frühzeitig Abweichungen, sodass Änderungen wie Imputation und Transformation nachvollziehbar durchgeführt werden können. Dadurch bleibt die Datenintegrität erhalten und bildet eine zuverlässige Basis für fundierte Analysen und Entscheidungen. Die Konsistenzsicherung gewährleistet, dass Daten während ihres gesamten Lebenszyklus einheitlich und korrekt bleiben. 

Synonyme zur Konsistenzsicherung sind bspw. Kohärenzsicherung, Stimmigkeitsprüfung. 

### Maßnahmen

| Maßnahme                   | Kurzbeschr.                                                                                                                                                                                                                                  |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MA-01 Datentyp Validierung | Eine sorgfältige Validierung der Datentypen stellt sicher, dass Trainings- und Eingabedaten den erwarteten Typen des Modells entsprechen, wodurch fehlerhafte Datenpunkte erkannt und gegebenenfalls korrigiert oder entfernt werden können. |
| MA-02 Format Prüfung       | Inhalte mittels Formatierungsprüfung auf Korrektheit prüfen                                                                                                                                                                                  |
| MA-03_Range Check          | Bereichsprüfung erkennt Ausreißer und falsche Daten in Merkmalen                                                                                                                                                                             |



### Referenzen

| RefID | Verweis                                                                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 15    |  ISO 9001:2015 - Quality management systems                                                                                                                | ISO 9001 ist eine weltweit anerkannte Norm für Qualitätsmanagement, die Organisationen dabei unterstützt, ihre Leistung zu verbessern, Kundenerwartungen zu erfüllen, Prozesse zu optimieren und durch regelmäßige Audits langfristigen Erfolg zu sichern.                                                                                                                                                                                                                                                  |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model                            | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                                                                                                                                                                                                                                            |
| 175   |  Rethinking Backdoor Attacks                                                                                                                               | Bei einem Backdoor-Angriff fügt ein Angreifer böswillig konstruierte Backdoor-Beispiele in einen Trainingssatz ein, um das resultierende Modell anfällig für Manipulationen zu machen. Bei der Abwehr solcher Angriffe geht es in der Regel darum, diese eingefügten Beispiele als Ausreißer im Trainingssatz zu betrachten und Techniken aus robusten Statistiken zu verwenden, um sie zu erkennen und zu entfernen.                                                                                       |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                                              | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.                                                                                                                                                                                                                         |
| 190   |  Kriterienkatalog C5                                                                                                                                       | Der C5 (Cloud Computing Compliance Criteria Catalogue) des Bundesamts für Sicherheit in der Informationstechnik (BSI) stellt einen detaillierten Kriterienkatalog dar, der grundlegende Anforderungen an die Informationssicherheit von Cloud-Diensten festlegt.                                                                                                                                                                                                                                            |
| 192   |  Scaling Laws for Data Poisoning in LLMs                                                                                                                   | Aktuelle Untersuchungen zeigen, dass LLMs anfällig für Datenvergiftung sind, bei der maliziöse oder fehlerhafte Daten zu schädlichem Verhalten führen. Die Studie untersucht drei Bedrohungsmodelle: böswillige Feinabstimmung, schlechte Datenverwaltung und absichtliche Kontamination. Experimente an 23 LLMs zeigen, dass größere Modelle anfälliger sind und schädliches Verhalten schneller erlernen. Dies unterstreicht die Notwendigkeit stärkerer Schutzmaßnahmen im Zuge der Skalierung von LLMs. |
| 230   |  ISO/IEC TS 12791 - Information technology — Artificial intelligence — Treatment of unwanted bias in classification and regression machine learning tasks  | Information Technology – Artificial Intelligence – Behandlung unerwünschter Verzerrungen bei Klassifizierungs- und Regressionsaufgaben des maschinellen Lernens                                                                                                                                                                                                                                                                                                                                             |



---
Name: QKB-04 Konsistenz
Title: QKB-04 Konsistenz
TitleGer: QKB-04 Konsistenz
shortdesc: Konsistenz soll sicherstellen, das Trainingsdaten einheitlich, fehlerfrei und ohne Widersprüche sind.
tags:
  - Qualitätskriterien
ID:
  - QKB-04
ListMeasureID: 
ListCritID: 
share: true
---

## QKB-04 Konsistenz

### Beschreibung 
Konsistenz soll sicherstellen, dass Trainingsdaten einheitlich, fehlerfrei und ohne Widersprüche sind. Nur durch wiederkehrende, nicht widersprüchliche Muster können Modelle die Inhalte aus den Daten generalisieren. Einheitliche Formatierungen können zur Konsistenz der Daten beitragen. Gleiche Kategorien oder Klassifikationen müssen einheitlich kodiert werden. 

Als Synonyme für 'Konsistenz' kommen Begriffe wie Übereinstimmung, Kohärenz und Einhaltung in Betracht. Diese Synonyme betonen die Konformität der Daten mit vordefinierten Standards, ihren logischen Zusammenhang sowie die strikte Befolgung von Regeln bei der Datenerfassung und -verarbeitung. 

Im Rahmen der Datenqualität unterscheidet man zwei wichtige, jedoch voneinander unabhängige Dimensionen:

- **Einheitlichkeit** stellt sicher, dass alle Dateneinträge denselben Formatierungsstandards entsprechen. Zum Beispiel müssen alle Datumswerte in einem vordefinierten Format (z.B. dd-MM-yyyy) vorliegen.
    
- **Konsistenz** geht darüber hinaus und prüft, ob die Daten inhaltlich stimmig und frei von Widersprüchen sind. Sie betrachtet die Beziehung zwischen den Daten, also ob Einträge miteinander in Einklang stehen, selbst wenn sie formal korrekt sein mögen. Dies bedeutet, dass zusammenhängende Daten – etwa Kundendaten, die in verschiedenen Tabellen geführt werden – übereinstimmen. Ein Datensatz kann also einheitlich formatiert sein und dennoch inkonsistente (widersprüchliche) Informationen enthalten, wenn z.B. Adressangaben nicht synchron aktualisiert werden.  

Zur Veranschaulichung: Während Einheitlichkeit vor allem die optische und strukturtechnische Übereinstimmung der Daten sicherstellt, bewertet Konsistenz, ob die hinterlegten Informationen logisch und inhaltlich korrekt zueinander passen. 

### Beispiele

#### Beispiel 1: Datenbankmanagement

In einem Kundendatenbanksystem müssen alle Datensätze, die sich auf denselben Kunden beziehen, konsistent sein. Wenn ein Kunde beispielsweise in verschiedenen Tabellen der Datenbank aufgeführt ist, müssen die Informationen über diesen Kunden in allen Tabellen übereinstimmen.

**Situation:**

- Tabelle "Kunden": Ein Eintrag für John Doe mit der Kundennummer 12345 und der Adresse "Musterstraße 1".
- Tabelle "Bestellungen": Einträge für Bestellungen von John Doe mit der Kundennummer 12345.

**Konsistenzproblem:** Wenn die Adresse von John Doe in der Tabelle "Kunden" auf "Beispielstraße 2" geändert wird, aber in der Tabelle "Bestellungen" immer noch "Musterstraße 1" steht, gibt es ein Konsistenzproblem.

**Lösung:** Es muss ein Mechanismus implementiert werden, der sicherstellt, dass alle Tabellen, die Informationen über John Doe enthalten, nach einer Adressänderung aktualisiert werden, sodass die Adresse überall gleich ist.


#### Beispiel 2: Finanzberichterstattung

In einem Unternehmen ist es entscheidend, dass die Finanzdaten konsistent über verschiedene Abteilungen hinweg geführt werden, um genaue und zuverlässige Berichte zu erstellen.

**Situation:**

- Abteilung "Vertrieb": Berichtet monatlich über Einnahmen aus Produktverkäufen.
- Abteilung "Buchhaltung": Berichtet ebenfalls monatlich über Einnahmen und Ausgaben.

**Konsistenzproblem:** Wenn die Abteilung "Vertrieb" für Januar 2024 Einnahmen von 100.000 EUR meldet, die Abteilung "Buchhaltung" jedoch nur Einnahmen von 95.000 EUR verzeichnet, besteht ein Konsistenzproblem, das auf falsche oder unvollständige Daten in einer der Abteilungen hinweisen könnte.

**Lösung:** Es muss eine regelmäßige Abstimmung und Überprüfung der Daten zwischen den Abteilungen erfolgen, um sicherzustellen, dass die Einnahmen korrekt und übereinstimmend berichtet werden. Dies könnte durch monatliche Meetings und die Einführung eines zentralen, gemeinsam genutzten Finanzsystems erfolgen, das die Daten automatisch abgleicht.

Diese Beispiele zeigen, wie wichtig Konsistenz für die Integrität und Zuverlässigkeit von Daten in verschiedenen Kontexten ist.


### Bausteine

| Baustein                  | Kurzbeschr.                                                                                                             |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| QB-02_Semantic Accuracy   | Genauigkeit bzgl. Bedeutung und Kontext in Daten                                                                        |
| QB-07 Gesamtheit          | Gesamtheit besteht, wenn alle erwarteten Werte vorhanden sind                                                           |
| QB-08 Konsistenzsicherung | Einheitliche, widerspruchsfreie Datenformate und -werte gewährleisten.                                                  |
| QB-10_DataChecks          | Überprüfung von Trainingsdaten sichert Qualität vor dem Modelltraining.                                                 |
| QB-11 Prozesse            | Dokumentation sichert Abläufe und Prozesse in IT-Infrastruktur und Softwareentwicklung.                                 |
| QB-12_FeatureEngineering  | Feature Engineering wandelt Rohdaten um, verbessert ML-Modelle durch relevante, generalisierbare, skalierbare Features. |



### Referenzen

| RefID | Verweis                                                                                                                           | Kurzbeschr.                                                                                                                                                                                                                                                                                                                          |
| ----- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 2     |  ISO 8000-8:2015 - Data quality — Part 8: Information and data quality: Concepts and measuring                                    | Diese Norm bietet eine Übersicht über die Konzepte und Messmethoden für Datenqualität. Sie umfasst Genauigkeit als eines der wesentlichen Merkmale zur Bewertung der Datenqualität.                                                                                                                                                  |
| 16    |  ISO 19157-1:2023 - Geographic information — Data quality — Part 1: General requirements                                          | Dieses Dokument legt die Prinzipien zur Beschreibung der Qualität geografischer Daten fest, definiert ein System und Prozesse zur Beschreibung der Datenqualität, spezifiziert Qualitätsmesskomponenten, beschreibt Verfahren zur Qualitätsbewertung und Prinzipien zur Berichterstattung, ohne Mindestqualitätsniveaus festzulegen. |
| 18    |  ISO/IEC 5259-2 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 2: Data quality measures  | Dieser Standard spezifiziert Maßnahmen zur Bewertung und Sicherstellung der Datenqualität, einschließlich der Ausgewogenheit der Daten.                                                                                                                                                                                              |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model   | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                                                                     |

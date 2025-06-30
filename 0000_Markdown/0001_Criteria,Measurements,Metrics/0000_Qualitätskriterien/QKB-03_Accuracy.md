---
Name: QKB-03 Genauigkeit
Title: QKB-03 Genauigkeit
TitleGer: QKB-03 Genauigkeit
shortdesc: Konkret muss jeder Datenpunkt zu einem gewissen Grad den korrekten Wert des Datums enthalten.
tags:
  - Qualitätskriterien
ID:
  - QKB-03
ListMeasureID: 
ListCritID: 
share: true
---

## QKB-03 Genauigkeit

### Beschreibung 

Genauigkeit beschreibt den Grad, in dem ein Datenwert in seiner numerischen oder symbolischen Darstellung einem festgelegten Referenzstandard entspricht – beispielsweise hinsichtlich zulässiger Rundungsgrade, Formatvorgaben oder Messauflösungen. Sie gibt an, wie präzise Daten im Verhältnis zu einem sogenannten _wahren_ oder _idealen_ Wert erfasst sind.

In diesem Kontext bezieht sich Genauigkeit nicht auf die Leistung eines KI-Modells, sondern auf die Qualität einzelner Datenpunkte hinsichtlich ihrer feingranularen Übereinstimmung mit technisch oder fachlich definierten Zielwerten.

"Genauigkeit" muss gegen "Korrektheit" abgrenzt werden. Semantisch unterscheiden sich die beiden Definitionen klar in ihrem Schwerpunkt: _Genauigkeit_ bezieht sich auf den **Grad der Detailtreue** (Wie genau wird ein Wert erfasst?), während _Korrektheit_ die **Richtigkeit an sich** meint (Stimmt der Wert überhaupt?). Damit sind die **Grundkonzepte** verschieden – Präzision vs. inhaltliche Wahrheit. 


### Beispiele

- Medizin: Ein Bluttest zur Bestimmung des Glukosespiegels muss genaue Werte liefern, um die richtige Diagnose und Behandlung von Diabetes zu ermöglichen. Ungenaue Testergebnisse könnten zu falschen Diagnosen und gefährlichen Behandlungsfehlern führen.
- Im Lagerverwaltungssystem eines Logistikunternehmens müssen die Bestände präzise nachverfolgt werden, um sicherzustellen, dass Produkte verfügbar sind und rechtzeitig geliefert werden können.


### Bausteine

| Baustein                       | Kurzbeschr.                                                             |
| ------------------------------ | ----------------------------------------------------------------------- |
| QB-01 Syntaktische Genauigkeit | Genauigkeit der Datenstruktur gemäß grammatikalischen Regeln und Syntax |
| QB-02_Semantic Accuracy        | Genauigkeit bzgl. Bedeutung und Kontext in Daten                        |



### Referenzen

| RefID | Verweis                                                                                                                           | Kurzbeschr.                                                                                                                                                                                                                                                                                                                          |
| ----- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 2     |  ISO 8000-8:2015 - Data quality — Part 8: Information and data quality: Concepts and measuring                                    | Diese Norm bietet eine Übersicht über die Konzepte und Messmethoden für Datenqualität. Sie umfasst Genauigkeit als eines der wesentlichen Merkmale zur Bewertung der Datenqualität.                                                                                                                                                  |
| 16    |  ISO 19157-1:2023 - Geographic information — Data quality — Part 1: General requirements                                          | Dieses Dokument legt die Prinzipien zur Beschreibung der Qualität geografischer Daten fest, definiert ein System und Prozesse zur Beschreibung der Datenqualität, spezifiziert Qualitätsmesskomponenten, beschreibt Verfahren zur Qualitätsbewertung und Prinzipien zur Berichterstattung, ohne Mindestqualitätsniveaus festzulegen. |
| 18    |  ISO/IEC 5259-2 - Artificial intelligence — Data quality for analytics and machine learning (ML) — Part 2: Data quality measures  | Dieser Standard spezifiziert Maßnahmen zur Bewertung und Sicherstellung der Datenqualität, einschließlich der Ausgewogenheit der Daten.                                                                                                                                                                                              |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model   | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                                                                     |

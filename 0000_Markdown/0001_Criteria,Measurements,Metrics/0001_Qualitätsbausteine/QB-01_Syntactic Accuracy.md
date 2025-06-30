---
Name: QB-01 Syntaktische Genauigkeit
Title: QB-01 Syntaktische Genauigkeit
TitleGer: QB-01 Syntaktische Genauigkeit
shortdesc: Genauigkeit der Datenstruktur gemäß grammatikalischen Regeln und Syntax
tags:
  - Qualitätsbaustein
ID:
  - QB-01
ListCritID:
  - "'QKB-03'"
share: true
---
## QB-01 Syntaktische Genauigkeit

### Beschreibung 

Ein Ausdruck ist syntaktisch genau, wenn alle festgelegten Formregeln exakt eingehalten werden – unabhängig davon, ob es sich um natürliche Sprache, Programmiersprachen oder andere Datentypen handelt. 

Diese korrekte Anordnung und Verbindung der Elemente führt dazu, dass der Datensatz in seiner formalen Struktur fehlerfrei ist und problemlos von Parsern oder Sprachmodellen verarbeitet werden kann, was vor allem in der Informatik und in der formalen Sprachtheorie von großer Bedeutung ist. 

Dabei bezieht sich syntaktische Genauigkeit ausschließlich auf die Einhaltung der strukturellen Regeln und nicht auf den Inhalt. Ein Ausdruck kann also formal korrekt sein, auch wenn seine inhaltliche Aussage unklar oder widersinnig erscheint. Diese Unterscheidung zwischen rein formaler und semantischer Genauigkeit ist grundlegend für das Verständnis und die Analyse von Daten in verschiedenen Kontexten.

### Beispiele

#### Grammatiken (NLP, Code)

Im Rahmen der maschinellen Übersetzung ist es entscheidend, syntaktisch korrekte Daten zu verwenden. Die Strukturen der Eingangs- und Zielsprache sind zu erfassen und reproduzieren. 

#### Rechtschreibprüfung

Bei der Rechtschreibprüfung werden Trainingsdaten verwendet, die Sätze und Texte mit korrekt angewendeter Grammatik und Syntax enthalten, sowie markierte Fehler und deren Korrekturen. Diese Daten helfen dabei, ein Modell zu trainieren, das in der Lage ist, typische Rechtschreib- und Grammatikfehler zu erkennen und Vorschläge zur Korrektur zu machen. Ein Beispiel wäre der Satz "He go to the store," der vom Modell als falsch erkannt und zu "He goes to the store" korrigiert wird.




### Maßnahmen

| Maßnahme                      | Kurzbeschr.                                                                                                                                                                                                                                  |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MA-01 Datentyp Validierung    | Eine sorgfältige Validierung der Datentypen stellt sicher, dass Trainings- und Eingabedaten den erwarteten Typen des Modells entsprechen, wodurch fehlerhafte Datenpunkte erkannt und gegebenenfalls korrigiert oder entfernt werden können. |
| MA-02 Format Prüfung          | Inhalte mittels Formatierungsprüfung auf Korrektheit prüfen                                                                                                                                                                                  |
| MA-03_Range Check             | Bereichsprüfung erkennt Ausreißer und falsche Daten in Merkmalen                                                                                                                                                                             |
| MA-04_Over-Undersampling      | Oversampling erhöht die Anzahl der Minderheitenklasse durch kopierte oder synthetische Beispiele, oft mit SMOTE, während beim Undersampling Datenpunkte der Majoritätsklasse entfernt werden, um ein Klassen-Gleichgewicht zu erreichen.     |
| MA-05 Automatisierte Aufgaben | Skripte können wiederkehrende Aufgaben automatisieren                                                                                                                                                                                        |
| MA-27 StatisticalBasics       | Sammelobjekt für statistische Grundlagen                                                                                                                                                                                                     |


### Referenzen

| RefID | Verweis                                                                                                                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | -------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 192   |  Scaling Laws for Data Poisoning in LLMs                                                                                         | Aktuelle Untersuchungen zeigen, dass LLMs anfällig für Datenvergiftung sind, bei der maliziöse oder fehlerhafte Daten zu schädlichem Verhalten führen. Die Studie untersucht drei Bedrohungsmodelle: böswillige Feinabstimmung, schlechte Datenverwaltung und absichtliche Kontamination. Experimente an 23 LLMs zeigen, dass größere Modelle anfälliger sind und schädliches Verhalten schneller erlernen. Dies unterstreicht die Notwendigkeit stärkerer Schutzmaßnahmen im Zuge der Skalierung von LLMs. |
| 190   |  Kriterienkatalog C5                                                                                                             | Der C5 (Cloud Computing Compliance Criteria Catalogue) des Bundesamts für Sicherheit in der Informationstechnik (BSI) stellt einen detaillierten Kriterienkatalog dar, der grundlegende Anforderungen an die Informationssicherheit von Cloud-Diensten festlegt.                                                                                                                                                                                                                                            |
| 189   |  Kriterienkatalog für KI-Cloud-Dienste – AIC4                                                                                    | Der AIC4 (Artificial Intelligence Cloud Services Compliance Criteria Catalogue) ist ein Kriterienkatalog entwickelt vom Bundesamt für Sicherheit in der Informationstechnik (BSI) mit dem Ziel, die Sicherheit von KI-basierten Clouddiensten zu verbessern und zu standardisieren.                                                                                                                                                                                                                         |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model  | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                                                                                                                                                                                                                                            |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods                        | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                                                                                                                                                                                                                                                         |
| 16    |  ISO 19157-1:2023 - Geographic information — Data quality — Part 1: General requirements                                         | Dieses Dokument legt die Prinzipien zur Beschreibung der Qualität geografischer Daten fest, definiert ein System und Prozesse zur Beschreibung der Datenqualität, spezifiziert Qualitätsmesskomponenten, beschreibt Verfahren zur Qualitätsbewertung und Prinzipien zur Berichterstattung, ohne Mindestqualitätsniveaus festzulegen.                                                                                                                                                                        |
| 11    |  ISO/TS 8000-82:2022 - Data quality — Part 82: Data quality assessment: Creating data rules                                      | Die ISO/TS 8000-82:2022 behandelt die Datenqualitätsbewertung durch Anwendung von Datenregeln auf verschiedene Datentypen, einschließlich Identifikatoren, Währungen und Datums-/Zeitangaben. Sie betont die Bedeutung von Datenprofiling bei der Formulierung effektiver Datenregeln, um die Integrität und Zuverlässigkeit von Daten in Informationssystemen sicherzustellen.                                                                                                                             |
| 10    |  ISO/TS 8000-81:2021 - Data quality — Part 81: Data quality assessment: Profiling                                                | Die ISO/TS 8000-81:2021 legt ein Verfahren für Datenprofiling zur Bewertung der Datenqualität fest, das sich auf Strukturanalyse, Spaltenanalyse und Beziehungsanalyse konzentriert. Sie ist auf tabellarische Daten anwendbar, behandelt jedoch keine Methoden zur Datenextraktion oder Regelableitung und kann sowohl eigenständig als auch zusammen mit Qualitätsmanagementsystem-Standards verwendet werden.                                                                                            |
| 2     |  ISO 8000-8:2015 - Data quality — Part 8: Information and data quality: Concepts and measuring                                   | Diese Norm bietet eine Übersicht über die Konzepte und Messmethoden für Datenqualität. Sie umfasst Genauigkeit als eines der wesentlichen Merkmale zur Bewertung der Datenqualität.                                                                                                                                                                                                                                                                                                                         |



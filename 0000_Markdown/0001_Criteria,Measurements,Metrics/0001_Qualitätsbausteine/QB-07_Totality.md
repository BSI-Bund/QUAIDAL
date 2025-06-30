---
Name: QB-07 Gesamtheit
Title: QB-07 Gesamtheit
TitleGer: QB-07 Gesamtheit
shortdesc: Gesamtheit besteht, wenn alle erwarteten Werte vorhanden sind
tags:
  - Qualitätsbaustein
ID:
  - QB-07
ListCritID:
  - "'QKB-02'"
  - "'QKB-04'"
share: true
---
## QB-07 Gesamtheit
### Beschreibung

Gesamtheit als Qualitätsbaustein stellt die Eigenschaft von Daten dar, Werte für alle erwarteten Attribute und Entitätsinstanzen aufzuweisen. 

Die Gesamtheit ist eine relative Eigenschaft, deren Bedeutung natürlich auch nach Anwendungsszenario variiert und immer im Kontext der spezifischen Nutzung betrachtet werden muss. Ebenso kann sie auf Datensatz-, Spalten- oder Datenpunktebene gemessen/betrachtet werden.  

Faktoren zur Messung der Gesamtheit könnten etwa 
- die Überprüfung unbeschrifteter Samples bei der bildbasierten Klassifikation oder 
- die Gesamtheit von beschrifteten Begrenzungsrahmen bei der Objekterkennung sein.
- Bei der Bilderkennung müssen besonders die Existenz von Zielobjekten in den Samples, die korrekte Kategorisierung aller Zielobjekte und die adäquate Beschriftung aller erkannten Zielobjekte mit Begrenzungsrahmen oder anderen Methoden beachtet werden. Diese Aspekte sind essentiell, um die Effizienz und Zuverlässigkeit von ML-Modellen zu gewährleisten.
- Auch die Gesamtheit aller Merkmale zur Beschreibung des Problems muss hierbei betrachtet werden. 

### Beispiele
#### Beispiel 1: Bilderkennung von Katzen und Hunden

**Anwendungsszenario:**
Ein ML-Modell soll Katzen und Hunde auf Bildern erkennen und kategorisieren.

**Gesamtheit:**
- **Datensatzebene:** Der Datensatz enthält Bilder von Katzen und Hunden.
- **Spaltenebene:** Jedes Bild ist mit einem Label (Katze oder Hund) versehen.
- **Datenpunktebene:** Jedes Bild, das eine Katze oder einen Hund enthält, hat einen korrekten Begrenzungsrahmen und ist korrekt kategorisiert.

**Messung der Gesamtheit:**
- Überprüfung, ob alle Bilder im Datensatz entweder eine Katze oder einen Hund zeigen.
- Sicherstellen, dass alle Katzen- und Hundebilder korrekt beschriftet sind.
- Prüfen, dass alle erkannten Katzen und Hunde mit einem Begrenzungsrahmen versehen sind.


#### Beispiel 2: Qualitätskontrolle in der Fertigung

**Anwendungsszenario:**
Ein System soll fehlerhafte Produkte auf einem Förderband erkennen.

**Gesamtheit:**
- **Datensatzebene:** Der Datensatz enthält Bilder von Produkten auf dem Förderband.
- **Spaltenebene:** Jedes Bild ist mit einem Label versehen, ob das Produkt fehlerhaft ist oder nicht.
- **Datenpunktebene:** Alle fehlerhaften Produkte sind korrekt identifiziert und beschriftet.

**Messung der Gesamtheit:**
- Sicherstellen, dass der Datensatz alle möglichen Zustände (fehlerhaft und nicht fehlerhaft) der Produkte abdeckt.
- Überprüfung, ob alle fehlerhaften Produkte im Datensatz korrekt beschriftet sind.
- Prüfen, dass jedes erkannte fehlerhafte Produkt mit einem Begrenzungsrahmen versehen ist.


#### Beispiel 3: Sentiment-Analyse von Kundenbewertungen

**Anwendungsszenario:**
Ein Modell soll die Stimmung (positiv, neutral, negativ) in Kundenbewertungen erkennen.

**Gesamtheit:**
- **Datensatzebene:** Der Datensatz enthält eine Vielzahl von Kundenbewertungen.
- **Spaltenebene:** Jede Bewertung ist mit einem Sentiment-Label (positiv, neutral, negativ) versehen.
- **Datenpunktebene:** Alle Kundenbewertungen sind korrekt kategorisiert.

**Messung der Gesamtheit:**
- Sicherstellen, dass der Datensatz eine breite und repräsentative Auswahl an Kundenbewertungen umfasst.
- Überprüfung, ob alle Bewertungen im Datensatz korrekt mit dem entsprechenden Sentiment-Label versehen sind.
- Prüfen, dass jede Bewertung vollständig erfasst und keine Daten fehlen.



### Maßnahmen
| Maßnahme                                      | Kurzbeschr.                                                                           |
| --------------------------------------------- | ------------------------------------------------------------------------------------- |
| MA-12 Abdeckung relevanter Merkmale           | Abdeckung aller wichtigen Merkmale im Datensatz zur Modellierung.                     |
| MA-13 Vollständige Information in Datensätzen | Prüfung ob Informationen nach einem bestimmtem Verlustschema fehlen (MCAR, MAR, MNAR) |
| MA-27 StatisticalBasics                       | Sammelobjekt für statistische Grundlagen                                              |



### Referenzen

| RefID | Verweis                                                                            | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 10    |  ISO/TS 8000-81:2021 - Data quality — Part 81: Data quality assessment: Profiling  | Die ISO/TS 8000-81:2021 legt ein Verfahren für Datenprofiling zur Bewertung der Datenqualität fest, das sich auf Strukturanalyse, Spaltenanalyse und Beziehungsanalyse konzentriert. Sie ist auf tabellarische Daten anwendbar, behandelt jedoch keine Methoden zur Datenextraktion oder Regelableitung und kann sowohl eigenständig als auch zusammen mit Qualitätsmanagementsystem-Standards verwendet werden. |
| 167   |  Beyond Accuracy: What Data Quality Means to Data Consumers                        | Die Studie entwickelt ein Rahmenwerk für Datenqualität, das die Bedürfnisse der Datenkonsumenten erfasst und zeigt, dass Datenqualität neben Genauigkeit auch Aspekte wie Kontext, Repräsentation und Zugänglichkeit umfasst, wodurch Unternehmen die Datenanforderungen besser verstehen und erfüllen können.                                                                                                   |
| 191   |  The Effects of Data Quality on Machine Learning Performance                       | Moderne KI-Anwendungen erfordern große Mengen hochwertiger Daten. Unvollständige oder fehlerhafte Daten führen zu unzuverlässigen Modellen und schlechten Entscheidungen. Eine vertrauenswürdige KI ist auf genaue, vollständige und konsistente Daten angewiesen.                                                                                                                                               |



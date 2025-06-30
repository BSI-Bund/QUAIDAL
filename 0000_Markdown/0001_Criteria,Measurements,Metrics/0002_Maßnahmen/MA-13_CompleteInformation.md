---
Name: MA-13 Vollständige Information in Datensätzen
Title: MA-13 Vollständige Information in Datensätzen
TitleGer: MA-13 Vollständige Information in Datensätzen
shortdesc: Prüfung ob Informationen nach einem bestimmtem Verlustschema fehlen (MCAR, MAR, MNAR)
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - unsicher
ID:
  - MA-13
ListMeasureID:
  - "'QB-13'"
  - "'QB-07'"
  - "'QB-06'"
ListCritID:
  - "'QKB-2'"
share: true
---
## MA-13 Vollständige Information in Datensätzen

### Beschreibung

Die Datensätze müssen vollständig sein, um das Problem konkret als Modell abbilden zu können. Liegen Lücken in den Datensätzen vor, müssen die Gründe hierfür bestimmt werden. Es dürfen keine Informationen fehlen. Alle Informationen, die für die Ermittlung von analytischen Zusammenhängen notwendig sind, müssen vorliegen. 

Eine wichtige Information ist die Antwort auf die Frage, warum die Daten fehlen, denn der Grund kann Hinweise auf das beste Imputationsverfahren zur Ergänzung der Lücken liefern. 

- Bei MCAR (Missing completely at random) fehlen die Daten zufällig ohne Bezug zu anderen Datenwerten. Beispiel: Verlust von ausgefüllten Fragebögen 
- Bei MAR (Missing at random) hängt die Wahrscheinlichkeit für das Fehlen von anderen Werten ab. Beispiel: Männer brechen Umfragen häufiger ab als Frauen und das Geschlecht ist bekannt. (Logistische Regression)
- Bei MNAR (Missing not at random) hängt das Fehlen der Daten von den fehlenden Werten selbst ab. Beispiel: Umfrageteilnehmer, die ihr hohes Einkommen nicht angeben wollten. 

Für jeden Typ von fehlenden Daten können diverse Prüfverfahren angesetzt werden. 

### Beispiele 

#### Beispiel 1 - MCAR

Ein Beispiel für MCAR (Missing Completely at Random) könnte eine Umfrage sein, bei der einige Teilnehmer zufällig die Frage nach ihrem Einkommen übersehen. Hierbei fehlt der Einkommenswert für einige Personen völlig zufällig, unabhängig von ihrem tatsächlichen Einkommen oder anderen Variablen wie Alter oder Geschlecht. Es gibt keinen systematischen Grund, warum diese Daten fehlen; sie fehlen einfach zufällig. (Prüfung mittels: Little's MCAR Test, Chi-Quadrat Test).

#### Beispiel 2 - MAR

Ein Beispiel für "Missing At Random" (MAR) wäre, wenn das Fehlen von Antworten in einer Umfrage von einer bekannten Variablen wie dem Geschlecht abhängt, aber nicht von den fehlenden Antworten selbst. Zum Beispiel könnten Männer eher dazu neigen, eine Umfrage abzubrechen als Frauen. (Prüfung mittels: Logistischer Regression).

#### Beispiel 3 - MNAR

Ein Beispiel für "Missing Not At Random" (MNAR) wäre, wenn in einer Umfrage Teilnehmer mit höherem Einkommen eher ihr Einkommen nicht angeben. Das Fehlen der Daten hängt hier direkt mit dem tatsächlichen Wert des Einkommens zusammen. Der konkrete Nachweis von MNAR ist schwierig und erfolgt oft nur indirekt. Hilfreich sind hier eine Kombination aus Domänenwissen, Sensitivitätsanalysen und deskriptiver Statistik zur Veranschaulichung des Problems. 


### Metriken & Methoden

| Metriken                       | Kurzbeschr.                                                                                                                        |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------- |
| QM-12_Prozent fehl. Variablen  | Durch die Analyse fehlender Informationen in einem Merkmal werden die entsprechenden Prozentzahlen für fehlende Element berechnet. |
| QM-40 Chi-Quadrat Test         | Chi-Quadrat-Test prüft Unabhängigkeit oder Anpassungsgüte von kategorialen Daten.                                                  |
| QM-53-1 Logistische Regression | Modelliert Wahrscheinlichkeit binärer oder mehrklassiger Ereignisse.                                                               |



### Referenzen

| RefID | Verweis                                                       | Kurzbeschr.                                                                                                                                                                                                                                                                           |
| ----- | ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 96    |  Statistical analysis with missing data                       | Die erste Auflage von Statistical Analysis with Missing Data wird für ihren wichtigen Beitrag zur angewandten Statistik, ihre zugängliche Darstellung von aktuellen und früheren Arbeiten sowie interessante Beispiele und Übungen gelobt und sollte auf jedem Statistikregal stehen. |
| 191   |  The Effects of Data Quality on Machine Learning Performance  | Moderne KI-Anwendungen erfordern große Mengen hochwertiger Daten. Unvollständige oder fehlerhafte Daten führen zu unzuverlässigen Modellen und schlechten Entscheidungen. Eine vertrauenswürdige KI ist auf genaue, vollständige und konsistente Daten angewiesen.                    |

---
Name: QM-50 Little's MCAR Test
Title: QM-50 Little's MCAR Test
TitleGer: QM-50 Little's MCAR Test
shortdesc: ist ein statistischer Test, der überprüft, ob fehlende Daten in einem Datensatz vollständig zufällig verteilt sind, ohne von den beobachteten oder fehlenden Werten beeinflusst zu werden.
tags:
  - Qualitätsmetrik
ID:
  - QM-50
ListMetricID: 
ListMeasureID:
  - "'QM-10'"
  - "'MA-08'"
MID: 
type:
  - method
CodeEx: true
share: true
lcstep: pre
---
## QM-50 Little's MCAR-Test

### Beschreibung

Dieser Test prüft die Nullhypothese, dass die Daten MCAR (Missing completely at random) fehlen. Also komplett zufällig fehlen, ohne weitere Zusammenhänge zu den restlichen Daten. 

Der Test vergleicht die Muster der fehlenden Daten über verschiedene Variablen hinweg und prüft, ob diese Muster zufällig verteilt sind. Wenn der Test Signifikanz hat, deutet dies darauf hin, dass die Daten nicht MCAR fehlen.

### Methode

- **Fehlende Daten identifizieren**: Es wird ermittelt, welche Variablenwerte im Datensatz fehlen. Dabei ist sicherzustellen, dass alle fehlenden Einträge als `NaN` (Not a Number) oder über einen anderen einheitlichen Indikator kenntlich gemacht sind.
- **Voraussetzungen prüfen**: Für den Little-MCAR-Test müssen die betrachteten Variablen mindestens auf Intervallskalenniveau vorliegen, und es müssen fehlende Werte im Datensatz vorhanden sein.
- **Durchführung des Little-MCAR-Tests**: Die Teststatistik sowie der zugehörige p-Wert werden berechnet, beispielsweise mithilfe spezialisierter Statistiksoftware oder entsprechender Pakete in Programmiersprachen wie Python.
    - $H_0$: Die fehlenden Daten sind MCAR (Missing Completely at Random).
    - $H_1$​: Die fehlenden Daten sind nicht MCAR.
- **Ergebnisinterpretation**:
    - **p-Wert**: Ein p-Wert größer als 0,05 zeigt an, dass die Nullhypothese nicht verworfen wird. Das spricht dafür, dass die fehlenden Daten als zufällig verteilt (MCAR) angesehen werden können.
    - **Teststatistik**: Wird der p-Wert nahe der Signifikanzgrenze beobachtet, kann die Teststatistik zusätzliche Hinweise liefern, um mögliche Abweichungen von der MCAR-Annahme zu erkennen.
- **Dokumentation und Schlussfolgerungen**: Die Resultate des Little-MCAR-Tests werden protokolliert, und auf dieser Basis erfolgt eine Bewertung der Verteilung der fehlenden Daten. Die gewonnenen Erkenntnisse dienen dazu, die geeignetste Vorgehensweise beim weiteren Umgang mit den fehlenden Werten auszuwählen (z. B. Listenweise Löschung, Imputation, Modellierung der fehlenden Daten).


### Pythoncode "Little's MCAR Test"

| RefID | Verweis                         |
| ----- | ------------------------------- |
| 49    | QM-50_Little's MCAR Test_python |



### Referenzen

| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                           |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 84    |  Statistical Approaches for Epidemiology: From Concept to Application  | Dieses Lehrbuch vermittelt die grundlegenden Konzepte der Epidemiologie und bereitet den Leser gleichzeitig auf die Fähigkeiten vor, statistische Instrumente in realen Situationen anzuwenden.                                                                                       |
| 96    |  Statistical analysis with missing data                                | Die erste Auflage von Statistical Analysis with Missing Data wird für ihren wichtigen Beitrag zur angewandten Statistik, ihre zugängliche Darstellung von aktuellen und früheren Arbeiten sowie interessante Beispiele und Übungen gelobt und sollte auf jedem Statistikregal stehen. |
| 248   |  Multiple Imputation: A Review of Practical and Theoretical Findings   | Der Artikel gibt einen Überblick über Multiple Imputation zur Behandlung fehlender Daten, diskutiert theoretische Ergebnisse, verschiedene Strategien zur Generierung von Imputationen und vergleicht unterschiedliche Methoden, bevor es zukünftige Forschungsperspektiven aufzeigt. |


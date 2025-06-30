---
Name: QM-11 Korrelationskoeffizient(diverse)
Title: QM-11 Korrelationskoeffizient(diverse)
TitleGer: QM-11 Korrelationskoeffizient(diverse)
shortdesc: Maß für lineare Beziehung zwischen Variablen.
tags:
  - Qualitätsmetrik
ID:
  - QM-11
ListMetricID: 
ListMeasureID:
  - "'MA-8'"
  - "'MA-12'"
  - "'MA-08'"
  - "'MA-24'"
MID: "11"
CodeEx: true
share: true
lcstep: pre
type:
  - method
---
## QM-11 Korrelationskoeffizient (diverse)

### Beschreibung

Korrelationskoeffizienten sind statistische Maße, die verwendet werden, um die Stärke und Richtung der Beziehung zwischen zwei Variablen zu bestimmen. Sie quantifizieren, in welchem Ausmaß Veränderungen in einer Variablen mit Veränderungen in einer anderen Variablen zusammenhängen. Korrelationskoeffizienten können Werte zwischen -1 und 1 annehmen, wobei:

- Ein Wert nahe +1 eine starke positive Korrelation anzeigt, was bedeutet, dass wenn eine Variable zunimmt, die andere ebenfalls tendenziell zunimmt.
- Ein Wert nahe -1 eine starke negative Korrelation anzeigt, was bedeutet, dass wenn eine Variable zunimmt, die andere tendenziell abnimmt.
- Ein Wert nahe 0 bedeutet, dass zwischen den Variablen keine oder eine sehr schwache Korrelation besteht.

Je nach Datentyp müssen andere Arten von Korrelationskoeffizienten gewählt werden. 

### Metrikformel/Methoden

| Tool                                                | Kurzbeschr.                                                                                                                                                                                                                                                                          |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-11-1_Pearson-Korrelationskoeffizient             | Der Pearson-Korrelationskoeffizient ist ideal für kontinuierliche Daten auf einer Intervall- oder Verhältnisskala, um die Stärke und Richtung eines linearen Zusammenhangs zwischen zwei Variablen auf einer Skala von -1 bis 1 zu messen.                                           |
| QM-11-2_Spearman-Rangkorrelationskoeffizient        | Der Spearman-Rangkorrelationskoeffizient ist ein nichtparametrisches Maß für die Stärke und Richtung einer monotonen Beziehung zwischen zwei Rangreihen von Variablen, besonders geeignet für ordinal oder kontinuierlich skalierte Daten mit Ausreißern oder ohne Normalverteilung. |
| QM-11-4_Koeffizient der punktbiserialen Korrelation | Der punktbiseriale Korrelationskoeffizient ist geeignet, um die Stärke und Richtung des Zusammenhangs zwischen einer dichotomen (binären) Variable und einer kontinuierlichen Variable zu messen, wie etwa den Einfluss des Geschlechts auf das Einkommen.                           |
| QM-11-3_Kendalls Tau                                | Kendall's Tau ist ideal für die Analyse monotone Beziehungen zwischen ordinalen oder rangbasierten Variablen, insbesondere bei nichtlinearen Zusammenhängen, Ausreißern, kleinen Stichproben oder Ties.                                                                              |
| QM-11-5 Phi-Koeffizient                             | ist ein statistisches Maß für die Stärke des Zusammenhangs zwischen zwei dichotomen (binären) Variablen in einer 2x2-Kreuztabelle.                                                                                                                                                   |




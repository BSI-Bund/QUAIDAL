---
Name: QM-38_GewichteteMetriken
Title: QM-38 Gewichtete Metriken
TitleGer: QM-38 Gewichtete Metriken
shortdesc: "Gewichtete Metriken in ML passen Bedeutung von Klassen und Proben an. Jede Metrik lässt sich auch in einer gewichteten Variante darstellen. Bspw.: Weighted Accuracy"
tags:
  - Qualitätsmetrik
ID:
  - QM-38
ListMetricID: 
ListMeasureID:
  - "'MA-10'"
  - "'MA-04'"
MID: "47"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-38 Gewichtete Metriken

### Beschreibung

Gewichtete Metriken wie bspw.: 

- "Weighted Accuracy" oder 
- "Weighted F1 Score" 

sind besonders wertvoll in Situationen, in denen Datenklassen ungleich verteilt sind oder unterschiedliche Klassen von unterschiedlicher Wichtigkeit sind. Diese gewichteten Metriken ermöglichen eine differenziertere Bewertung der Leistung von Klassifizierungsmodellen, indem sie den Beitrag jeder Klasse zur Gesamtmetrik entsprechend ihrer Bedeutung oder ihrer relativen Häufigkeit anpassen. Hier sind einige Vorteile der Verwendung von gewichteten Metriken:

### Methode

#### 1. Ausgleich von Klassenungleichgewichten

In vielen realen Datensätzen sind einige Klassen häufiger als andere. Standardmetriken wie einfache Genauigkeit (Accuracy) können irreführend sein, da ein Modell, das hauptsächlich die Mehrheitsklasse vorhersagt, fälschlicherweise als hochpräzise erscheinen könnte. Gewichtete Metriken berücksichtigen die tatsächliche Verteilung der Klassen, indem sie jedem Beispiel oder jeder Klasse ein Gewicht geben, das ihrer Häufigkeit oder Bedeutung entspricht. Dadurch wird sichergestellt, dass das Modell alle Klassen angemessen berücksichtigt.

#### 2. Priorisierung wichtiger Klassen

In vielen Anwendungsfällen sind einige Klassen wichtiger als andere. Beispielsweise könnte in einem medizinischen Diagnosesystem die korrekte Erkennung einer seltenen, aber lebensbedrohlichen Krankheit wichtiger sein als die Erkennung häufigerer, weniger schwerwiegender Zustände. Gewichtete Metriken ermöglichen es, die Bedeutung jeder Klasse zu betonen, indem sie höhere Gewichte für kritischere Klassen verwenden.

#### 3. Verbesserung der Modellbewertung

Gewichtete Metriken bieten eine realistischere Bewertung der Modellleistung über ungleichmäßig verteilte Daten hinweg. Dies ist besonders nützlich für die Entwicklung und Bewertung von Modellen in vielschichtigen oder mehrklassigen Umgebungen, wo die Leistung in weniger häufigen Klassen entscheidend sein kann.

#### 4. Anpassungsfähigkeit

Gewichtete Metriken sind flexibel und können an verschiedene spezifische Bedürfnisse und Kriterien angepasst werden. Sie ermöglichen es Forschern und Entwicklern, Modelle zu erstellen und zu bewerten, die auf die spezifischen Anforderungen und Ziele ihrer Projekte zugeschnitten sind.

### Pythoncode "WeightedMetrics"

| RefID | Verweis                   |
| ----- | ------------------------- |
| 31    | QM-38_WeightedMetrics_div |




### Referenzen

| RefID | Verweis                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ----- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 196   |  Pattern recognition and machine learning  | Die Mustererkennung entstand aus dem Ingenieurwesen und maschinelles Lernen aus der Informatik, aber beide haben sich gemeinsam weiterentwickelt. Bayesianische Methoden, grafische Modelle und Kernel-basierte Modelle haben mit verbesserten Algorithmen wie Variations-Bayes eine zentrale Bedeutung erlangt. Dieses Lehrbuch stellt diese Themen für fortgeschrittene Studierende und Forscher vor, die Kenntnisse in Analysis und linearer Algebra erfordern. |



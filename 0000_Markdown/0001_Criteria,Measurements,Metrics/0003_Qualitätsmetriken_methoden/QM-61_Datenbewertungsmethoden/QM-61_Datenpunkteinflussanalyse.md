---
Name: QM-61 Datenpunkt-Einflussanalyse
Title: QM-61 Datenpunkt-Einflussanalyse
TitleGer: QM-61 Datenpunkt-Einflussanalyse
shortdesc: Verschiedene Methoden die den Einfluss von Datenpunkten auf das Ergebnis eines Modells bewerten.
tags:
  - Qualitätsmetrik
  - ML-Data-Valuation
ID:
  - QM-61
ListMetricID: 
ListMeasureID:
  - "'MA-14'"
  - "'MA-18'"
MID: "104"
lcstep: post
CodeEx: true
share: true
type:
  - method
---
## QM-61 Datenpunkt-Einflussanalyse

### Beschreibung

Die "Bewertung des Beitrags einzelner Datenpunkte oder Datensätze zur Gesamtleistung eines Modells" bezieht sich auf die Einschätzung, wie stark ein einzelner Datenpunkt oder ein Datensatz zur Leistung eines Modells beiträgt. Dieser Beitrag kann sich auf verschiedene Aspekte der Modellleistung beziehen, je nach den Zielen und Anforderungen der Anwendung. Im Allgemeinen kann die Bewertung des Beitrags einzelner Datenpunkte oder Datensätze zur Modellleistung auf folgende Weise erfolgen:

- **Relevanz für das Modell**: Ein Datenpunkt oder Datensatz wird als relevanter für das Modell angesehen, wenn sein Vorhandensein oder seine Abwesenheit einen signifikanten Einfluss auf die Modellleistung hat. Zum Beispiel könnten bestimmte Datenpunkte dazu beitragen, die Vorhersagegenauigkeit eines Modells zu verbessern, während andere weniger relevant sein könnten.
- **Informationsgehalt**: Ein Datenpunkt oder Datensatz wird anhand seines Informationsgehalts bewertet, d.h. wie viel neue oder einzigartige Informationen er dem Modell zur Verfügung stellt. Datenpunkte oder Datensätze mit höherem Informationsgehalt können für das Modell wertvoller sein, da sie dazu beitragen, ein besseres Verständnis der zugrundeliegenden Datenverteilung zu erlangen.
- **Robustheit gegenüber Störungen**: Ein Beitrag wird auch anhand seiner Auswirkungen auf die Robustheit des Modells bewertet. Datenpunkte oder Datensätze, deren Hinzufügung oder Entfernung die Robustheit des Modells gegenüber Störungen verbessert, werden als wertvoller betrachtet.
- **Interpretationsmöglichkeiten**: Ein weiterer Aspekt ist die Interpretierbarkeit des Beitrags eines Datenpunktes oder Datensatzes zur Modellleistung. Datenpunkte, die dazu beitragen, das Modell besser interpretierbar zu machen, indem sie Einblicke in die zugrunde liegenden Muster oder Zusammenhänge bieten, können als besonders wertvoll angesehen werden.

Die Bewertung des Beitrags einzelner Datenpunkte oder Datensätze zur Gesamtleistung eines Modells kann durch verschiedene Techniken wie Feature-Importance, Sensitivity Analysis oder den Marginal-Contribution-Approach erfolgen. Diese Bewertung hilft, wichtige Datenpunkte oder Datensätze zu identifizieren und ermöglicht eine gezielte Verbesserung der Modellleistung oder Anpassung der Datenanalysestrategie.


### Ansätze
| Tool                                   | Kurzbeschr.                                                                                      |
| -------------------------------------- | ------------------------------------------------------------------------------------------------ |
| QM-61 Datenpunkt-Einflussanalyse       | Verschiedene Methoden die den Einfluss von Datenpunkten auf das Ergebnis eines Modells bewerten. |
| QM-61-1 Marginal Contribution Approach | Bewertung des Datenbeitrags in Modellen.                                                         |
| QM-61-2 Data Re-weighting Strategies   | Anpassung von Datenpunkten zur Modellverbesserung und Fairness.                                  |
| QM-61-3_Neural Dynamic Data Valuation  | Bewertung mit neuronalen Werkzeugen von Datenpunkten in dynamischem Kontext.                     |



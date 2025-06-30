---
Name: MA-04_Over-Undersampling
Title: MA-04 Over-Undersampling
TitleGer: MA-04 Over-Undersampling
shortdesc: Oversampling erhöht die Anzahl der Minderheitenklasse durch kopierte oder synthetische Beispiele, oft mit SMOTE, während beim Undersampling Datenpunkte der Majoritätsklasse entfernt werden, um ein Klassen-Gleichgewicht zu erreichen.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-04
ListMetricID: 
ListMeasureID:
  - "'QB-13'"
  - "'QB-01'"
  - "'QB-06'"
share: true
---
## MA-04 Over- und Undersampling

### Beschreibung

Beim Oversampling wird die Anzahl der Beispiele einer Minderheitenklasse künstlich erhöht, indem kopierte oder synthetische Beispiele eingefügt werden. Ein beliebter Ansatz zur Generierung neuer Beispiele ist SMOTE (Synthetic Minority Over-sampling Technique). SMOTE generiert neue Beispiele durch Interpolation zwischen existierenden Beispielen der Minderheitenklasse. Für das Undersampling hingegen werden - nach einem strikten Vorgehen - Datenpunkte der Majoritätsklasse entfernt, um somit eine bessere Gleichgewichtung der Klassen zu erzeugen.

### Beispiele 

- Es liegt ein Datensatz mit 100000 Finanztransaktionen vor. Davon sind 99500 als legitim und 500 als betrügerisch klassifiziert. Durch den hohen Anteil an legitimen Datensätzen kann es zu einem Bias im Modell kommen der dazu führt, dass jegliche Datensätze als legitim gekennzeichnet werden. 
- Oversampling: Durch die Integration von kopierten oder synthetisch generierten Beispielen wird der Anteil der Minderheitenklasse künstlich erhöht. 
- Undersampling: Durch die Reduktion der Beispiele der Majoritätsklasse wird ein besseres Klassengleichgewicht angestrebt. 


### Metriken & Methoden

| ID                                                 | Kurzbeschr.                                                                                                                                                                                |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-34 Validierung der Feldgröße                    | Textfelder und Variablen auf erwartete Länge überprüfen. Automatisiert/expertengesteuert.                                                                                                  |
| QM-38_GewichteteMetriken                           | Gewichtete Metriken in ML passen Bedeutung von Klassen und Proben an. Jede Metrik lässt sich auch in einer gewichteten Variante darstellen. Bspw.: Weighted Accuracy                       |
| QM-57-1 Synthetic Minority Over-sampling Technique | eine Methode zur Erzeugung synthetischer Beispiele der Minderheitsklasse in einem unausgeglichenen Datensatz, um die Klassenverteilung auszugleichen und die Modellleistung zu verbessern. |




### Referenzen

| RefID | Verweis                                                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 74    |  Imbalanced learning: foundations, algorithms, and applications  | Dieses Werk bietet die erste umfassende Übersicht über das Lernen mit unausgewogenen Datensätzen, ein zentrales Thema in Bereichen wie Überwachung, Sicherheit, Finanzen und biomedizinischen Systemen. Es vermittelt Einblicke in modernste Techniken, Prinzipien und Anwendungen und unterstützt Wissenschaftler und Ingenieure dabei, Herausforderungen zu bewältigen und zukünftige Forschungsperspektiven zu erkunden. |

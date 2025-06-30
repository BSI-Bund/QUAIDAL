---
Name: QM-51-10_Kolmogorov Smirnov Test
Title: QM-51-10 Kolmogorov-Smirnov-Test
TitleGer: QM-51-10 Kolmogorov-Smirnov-Test
shortdesc: Der Kolmogorov-Smirnov-Test (KS-Test) ist ein statistischer Test, der die Übereinstimmung zwischen einer Stichprobe und einer theoretischen Verteilung oder zwischen zwei Stichproben vergleicht, indem er die maximale Differenz zwischen ihren kumulativen Verteilungsfunktionen misst. Er hilft dabei zu bestimmen, ob die Stichproben aus der gleichen Verteilung stammen oder signifikante Unterschiede bestehen.
tags:
  - Qualitätsmetrik
  - DA-Type
ID:
  - QM-51-10
ListMetricID: 
ListMeasureID:
  - "'MA-8'"
  - "'MA-08'"
  - "'MA-03'"
lcstep: pre
CodeEx: true
share: true
type:
  - method
---
## QM-51-10 Kolmogorov-Smirnov-Test

### Beschreibung

Der **Kolmogorov-Smirnov-Test (KS-Test)** ist ein nichtparametrischer statistischer Test, der verwendet wird, um die Übereinstimmung einer empirischen Verteilung mit einer theoretischen Verteilung zu überprüfen (Ein-Sample-KS-Test) oder um die Verteilungen zweier Stichproben zu vergleichen (Zwei-Sample-KS-Test).

#### Ein-Sample-KS-Test:
    
Dieser Test vergleicht die Verteilung einer Stichprobe mit einer vorgegebenen theoretischen Verteilung (z.B. einer Normalverteilung), um zu überprüfen, ob die Stichprobe aus dieser Verteilung stammt.

#### Zwei-Sample-KS-Test
    
Hier wird die Verteilung von zwei unabhängigen Stichproben miteinander verglichen, um zu beurteilen, ob sie aus derselben Verteilung stammen.


### Methode

- Der KS-Test basiert auf der maximalen Differenz zwischen der empirischen Verteilungsfunktion der Stichprobe und der kumulativen Verteilungsfunktion der theoretischen Verteilung oder zwischen den Verteilungsfunktionen zweier Stichproben.
- Der Test berechnet einen **KS-Statistik-Wert**, der die maximale Abweichung zwischen den Verteilungsfunktionen darstellt.
- Diese maximale Abweichung wird mit einem kritischen Wert verglichen, der von der Größe der Stichprobe abhängt. Ein signifikanter KS-Statistik-Wert (größer als der kritische Wert) deutet darauf hin, dass die Verteilung der Stichprobe signifikant von der theoretischen Verteilung abweicht.

### Sourcecode "Kolmogorov Smirnov Test"

| RefID | Verweis                                 |
| ----- | --------------------------------------- |
| 53    | QM-51-10_Kolmogorov Smirnov Test_python |



### Referenzen

| RefID | Verweis                                                                                              | Kurzbeschr.                                                                                                                                                                                                                                                                                             |
| ----- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 197   |  Distributional Ground Truth: Non-Redundant Crowdsourcing Data Quality Control in UI Labeling Tasks  | Das Papier präsentiert ein nicht-redundantes Verfahren zur Vorhersage der Qualität von Crowdworker-Labels bei Web-UI-Annotationen, das Verteilungen per Kolmogorov-Smirnov-Test vergleicht und so bei einer Trusted-Set-Größe von 17–27 % R²-Werte über 0,8 erreicht und redundante Kontrollen ersetzt. |



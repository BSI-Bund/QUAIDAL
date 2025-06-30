---
Name: QM-23 Mittlerer quadratische Abweichung
Title: QM-23 Mittlerer quadratischer Abweichung
TitleGer: QM-23 Mittlerer quadratischer Abweichung
shortdesc: Maß für mittlere quadratischen Abweichung zwischen geschätzten und wahren Werten.
tags:
  - Qualitätsmetrik
ID:
  - QM-23
ListMetricID: 
ListMeasureID:
  - "'MA-27'"
MID: 
type:
  - metrik
lcstep: post
CodeEx: true
share: true
---
## QM-23 Mittlerer quadratischer Fehler
### Beschreibung

Der Mean Squared Error (MSE) misst die durchschnittliche Quadratsumme der Fehler, also die durchschnittliche quadrierte Differenz zwischen den geschätzten Werten und dem tatsächlichen Wert. Er ist immer positiv und nähert sich Null an, je genauer das Modell ist. MSE berücksichtigt sowohl die Varianz des Schätzers als auch dessen Verzerrung (Bias), wobei für unverzerrte Schätzer MSE und Varianz gleich sind. Der MSE ist ein wichtiges Maß für die Qualität eines Schätzers oder Vorhersagemodells

### Methode

- **Vorhersagen und tatsächliche Werte:** Eine Reihe von Modellvorhersagen und die entsprechenden tatsächlichen Werte werden erfasst.
- **Abweichungen berechnen:** Für jeden Datenpunkt wird die Differenz zwischen dem vorhergesagten Wert und dem tatsächlichen Wert ermittelt.
- **Quadrieren der Abweichungen:** Jede ermittelte Abweichung wird quadriert, um sicherzustellen, dass alle Werte positiv sind und größere Abweichungen stärker gewichtet werden.
- **Mitteln der quadrierten Abweichungen:** Alle quadrierten Abweichungen werden summiert und die Summe durch die Gesamtzahl der Datenpunkte geteilt. Auf diese Weise ergibt sich der durchschnittliche Fehler.
- **Interpretation:** Je niedriger der MSE-Wert, desto genauer gilt das Modell. Ein höherer Wert weist auf größere Abweichungen und damit auf eine geringere Modellgenauigkeit hin.

### Beispiel - MSE bei der Vorhersage von Immobilienpreisen

Nachdem ein Modell für die Vorhersage von Immobilienpreisen trainiert wurde, berechnet man den MSE um den durchschnittlichen quadratischen Fehler zwischen den vorhergesagten und tatsächlichen Verkaufspreisen zu ermitteln. 

Angenommen, für ein Haus in den Trainingsdaten beträgt der tatsächliche Verkaufspreis 300.000 Euro. Das Modell sagt für dieses Haus einen Preis von 320.000 Euro vorher.

- Der Fehler für dieses Haus beträgt (320.000 - 300.000)² = 400.000.000 Euro².

Man berechnet diesen quadratischen Fehler für jedes Haus in den Trainingsdaten und ermittelt den Durchschnitt aller dieser Fehler, was den MSE ergibt.

#### Interpretation:

Ein niedriger MSE deutet darauf hin, dass das Modell die Preise der Häuser in den Trainingsdaten gut vorhersagen kann. Ein hoher MSE hingegen weist darauf hin, dass es große Abweichungen zwischen den tatsächlichen und den vorhergesagten Preisen gibt, was bedeutet, dass das Modell möglicherweise nicht gut genug ist.

### Referenzen
| RefID | Verweis                            | Kurzbeschr.                                                                                                                                                                                           |
| ----- | ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 243   |  Mittlere quadratische Abweichung  | Die mittlere quadratische Abweichung (MSE) ist ein zentrales Qualitätskriterium in der Statistik, das die Streuung eines Punktschätzers um den wahren Wert als erwarteten quadratischen Fehler misst. |

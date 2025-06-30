---
Name: QM-58-2 Exponentialmechanismus
Title: QM-58-2 Exponentialmechanismus
TitleGer: QM-58-2 Exponentialmechanismus
shortdesc: Methode zur Gewährleistung der "Differential Privacy"
tags:
  - Qualitätsmetrik
  - DifferentialPrivacy
ID:
  - QM-58-2
ListMetricID: 
ListMeasureID:
  - "'MA-25'"
MID: "100"
type:
  - method
lcstep: post
CodeEx: true
share: true
---
## QM-58-2 Exponentialmechanismus

### Beschreibung

Der Exponentialmechanismus ist ein Algorithmus zur Gewährleistung der "Differential Privacy". Er ermöglicht, private Informationen in Daten zu verarbeiten, während gleichzeitig die Privatsphäre der individuellen Datenpunkte geschützt wird.

Im Gegensatz zum Laplaceschen Mechanismus, der Rauschen zu den echten Daten addiert, funktioniert der Exponentialmechanismus durch die Berechnung einer Wahrscheinlichkeitsverteilung über die möglichen Ergebnisse einer Abfrage. Diese Wahrscheinlichkeitsverteilung wird dann so verzerrt, dass die Wahrscheinlichkeit von Ergebnissen, die die Privatsphäre gefährden könnten, reduziert wird. 

Der Exponentialmechanismus ist besonders geeignet für Situationen, in denen eine optimale Antwort aus einer Menge möglicher Optionen gewählt werden soll, das direkte Hinzufügen von Rauschen zu dieser Antwort jedoch ihren Wert oder ihre Aussagekraft erheblich beeinträchtigen würde.

### Methode

Hier sind die grundlegenden Schritte des Exponentialmechanismus:

- **Eingaben festlegen**: Du hast eine Liste von möglichen Optionen (z. B. Antworten) und eine Bewertungsfunktion, die jeder Option einen Nutzen zuweist. Außerdem gibt es zwei Parameter:
    - **Epsilon** (wie viel Privatsphäre du wahren willst)
    - **Sensitivität** (wie stark sich die Bewertung ändern kann, wenn sich die Daten ändern).

- **Gewichte berechnen**: Optionen mit höheren Bewertungen sollten bevorzugt werden, daher berechnest du für jede Option ein Gewicht. Dieses Gewicht sagt aus, wie wahrscheinlich die Auswahl dieser Option ist.
    
- **Wahrscheinlichkeiten normalisieren**: Die berechneten Gewichte werden so angepasst, dass ihre Summe 1 ergibt. Damit hast du eine Wahrscheinlichkeitsverteilung, die festlegt, wie wahrscheinlich es ist, jede Option zu wählen.
    
- **Option auswählen**: Schließlich wählst du eine Option zufällig aus, wobei die Wahrscheinlichkeiten aus dem vorherigen Schritt genutzt werden. Optionen mit besseren Bewertungen haben eine höhere Chance, ausgewählt zu werden, aber es bleibt Zufall im Spiel.

Der Exponentialmechanismus bietet den Vorteil, dass er eine feinere Steuerung über die Verzerrung der Ergebnisse ermöglicht und daher möglicherweise eine bessere Nützlichkeit im Vergleich zum Laplaceschen Mechanismus bietet. Er wird häufig in Situationen eingesetzt, in denen die Sensitivität der Abfrage hoch ist oder in denen ein subtileres Datenschutzmaß erforderlich ist.

### Sourcecode "Exponentialmechanismus"
| RefID | Verweis                               | Inhalt                          |
| ----- | ------------------------------------- | ------------------------------- |
| 80    | QM-58-2_Exponentialmechanismus_python | Exponentialmechnismus in Python |




### Referenzen
| RefID | Verweis                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 292   |  The Algorithmic Foundations of Differential Privacy  | The Algorithmic Foundations of Differential Privacy definiert das Konzept der differentiellen Privatsphäre, erläutert zentrale Mechanismen wie den Laplaceschen und Exponentialmechanismus, führt Kompositionstheoreme für wiederholte Abfragen an, diskutiert die Balance zwischen Datenschutz und Genauigkeit und bietet damit sowohl eine fundierte theoretische Grundlage als auch praxisrelevante Einsichten für die Entwicklung datenschutzfreundlicher Algorithmen. |



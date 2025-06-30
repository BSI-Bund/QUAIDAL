---
Name: QM-58-1 Laplacescher Mechanismus
Title: QM-58-1 Laplacescher Mechanismus
TitleGer: QM-58-1 Laplacescher Mechanismus
shortdesc: Fügt Rauschen hinzu, um differenzielle Privatsphäre zu gewährleisten.
tags:
  - Qualitätsmetrik
  - DifferentialPrivacy
ID:
  - QM-58-1
ListMetricID: 
ListMeasureID:
  - "'MA-25'"
MID: "99"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-58-1 Laplacescher Mechanismus

### Beschreibung

Der Laplacesche Mechanismus ist eine Methode zur Umsetzung von differentieller Privatsphäre, einem Konzept aus der Kryptographie und Datenschutzforschung. Der Laplacesche Mechanismus fügt dem Ergebnis einer Abfrage ein zufälliges Rauschen aus einer Laplace-Verteilung hinzu. Die Stärke des Rauschens wird durch den sogenannten "Differential Privacy Parameter" gesteuert, der das Maß des Datenschutzes angibt. Je größer der Wert dieses Parameters ist, desto mehr Rauschen wird hinzugefügt, was zu einem höheren Grad an Datenschutz führt, aber auch zu einer geringeren Genauigkeit der Abfrageergebnisse.

Durch die Anwendung des Laplaceschen Mechanismus kann differentielle Privatsphäre gewährleistet werden, indem die Privatsphäre der einzelnen Datenpunkte geschützt wird, während gleichzeitig nützliche Informationen aus den aggregierten Abfrageergebnissen gewonnen werden können. 

### Methode

Die Laplacesche Methode zur Implementierung von Differential Privacy (DP) nutzt die Laplace-Verteilung, um Rauschen in die Daten einzufügen, wodurch der Schutz der Privatsphäre von Individuen in einem Datensatz gewährleistet wird. Differential Privacy ist ein mathematischer Ansatz, der sicherstellt, dass die Wahrscheinlichkeit, ob ein bestimmtes Individuum in einem Datensatz enthalten ist oder nicht, durch die Ausgabe eines statistischen Modells oder Algorithmus nur geringfügig beeinflusst wird.

#### 1. Bestimme die Sensitivität der Funktion
Finde heraus, wie sehr sich das Ergebnis der Funktion ändert, wenn ein einzelner Dateneintrag geändert wird. Das ist die maximale Auswirkung, die ein Individuum auf das Ergebnis hat.

#### 2. Wähle den Datenschutzparameter (ϵ)
Bestimme, wie viel Privatsphäre du schützen möchtest. Ein kleinerer Wert bietet mehr Schutz, erhöht jedoch das Rauschen im Ergebnis.

#### 3. Füge Laplace-Rauschen hinzu
Generiere eine zufällige Störung (Rauschen) basierend auf der Sensitivität und dem gewählten epsilon-Wert. Das Rauschen sorgt dafür, dass einzelne Datenpunkte schwerer zu identifizieren sind.

#### 4. Berechne die geschützte Ausgabe
Addiere das erzeugte Rauschen zum ursprünglichen Ergebnis. Dadurch wird die Privatsphäre geschützt, und es entsteht ein "privates" Ergebnis.


### Sourcecode "Laplacescher Mechanismus"
| RefID | Verweis                                 | Inhalt                             |
| ----- | --------------------------------------- | ---------------------------------- |
| 79    | QM-58-1_Laplacescher Mechanismus_python | Laplaceschen Mechanismus in Python |



### Referenzen
| RefID | Verweis                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 292   |  The Algorithmic Foundations of Differential Privacy  | The Algorithmic Foundations of Differential Privacy definiert das Konzept der differentiellen Privatsphäre, erläutert zentrale Mechanismen wie den Laplaceschen und Exponentialmechanismus, führt Kompositionstheoreme für wiederholte Abfragen an, diskutiert die Balance zwischen Datenschutz und Genauigkeit und bietet damit sowohl eine fundierte theoretische Grundlage als auch praxisrelevante Einsichten für die Entwicklung datenschutzfreundlicher Algorithmen. |


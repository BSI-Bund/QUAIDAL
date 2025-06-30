---
Name: QM-63-3_Federated Transfer Learning
Title: QM-63-3 Federated Transfer Learning
TitleGer: QM-63-3 Federated Transfer Learning
shortdesc: Federated Transfer Learning erweitert Federated Learning, um flexible Zusammenarbeit bei Parteien mit teils unterschiedlichen Merkmalen und Datensätzen zu ermöglichen.
tags:
  - Qualitätsmetrik
  - "#ML-FedLearn"
  - ML-FedLearn
ID:
  - QM-63-3
ListMetricID: 
ListMeasureID:
  - "'MA-26'"
MID: 
type:
  - metrik
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-63-3 Federated Transfer Learning

### Beschreibung

Federated Transfer Learning (FTL) ist eine Erweiterung von Federated Learning, die in Szenarien eingesetzt wird, in denen sowohl die Merkmale (Features) als auch die Datensätze (Samples) zwischen verschiedenen Parteien nicht vollständig überlappen. Dies macht es zu einem flexiblen Ansatz für die Zusammenarbeit zwischen Parteien mit heterogenen und teilweise korrelierten Datensätzen.

FTL kombiniert die Konzepte von Federated Learning und Transfer Learning, indem es Modelle von einer Partei auf eine andere überträgt, um Wissenslücken zu schließen.

### Methode

- Teilweise überlappende Datenpunkte:
    Nur ein Teil der Datensätze (Samples) ist zwischen den Parteien identisch. Andere Datenpunkte unterscheiden sich.

- Unterschiedliche Features:
    Die Feature-Sets können sich zwischen den Parteien unterscheiden oder nur teilweise überlappen.

- Transfer Learning-Komponente:
    Wissen, das durch das Training eines Modells auf den Daten einer Partei gewonnen wurde, wird genutzt, um das Training bei der anderen Partei zu verbessern.

- Kooperation trotz Heterogenität:
    Selbst bei minimalen Gemeinsamkeiten zwischen den Datensätzen können die Parteien ein verbessertes Modell trainieren.

### Beispiel 

#### Kontext:

- **Krankenhaus A** hat Daten über klinische Tests (z. B. Blutwerte) von Patienten.
- **Krankenhaus B** hat Daten über Bildgebungsverfahren (z. B. Röntgenbilder) derselben Patienten, jedoch auch Daten über weitere Patienten, die Krankenhaus A nicht kennt.

Federated Learning Ansatz: 
- Beide Krankenhäuser möchten ein Modell trainieren, um Krankheitsdiagnosen zu verbessern.
- Federated Transfer Learning ermöglicht die gemeinsame Nutzung von Wissen zwischen den beiden Parteien:
    - Krankenhaus A trainiert ein Modell auf seinen klinischen Daten.
    - Dieses Wissen wird an Krankenhaus B übertragen, das es mit seinen Bildgebungsdaten kombiniert, um ein globales Modell zu erstellen.



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 165   |  Federated Machine Learning: Concept and Applications  | Der Text identifiziert Datensilos und Datenschutz als zentrale KI-Herausforderungen und schlägt ein erweitertes sicheres Federated Learning (horizontal, vertikal und transferbasiert) vor, um Wissensaustausch zwischen Organisationen ohne Verletzung der Privatsphäre zu ermöglichen. |


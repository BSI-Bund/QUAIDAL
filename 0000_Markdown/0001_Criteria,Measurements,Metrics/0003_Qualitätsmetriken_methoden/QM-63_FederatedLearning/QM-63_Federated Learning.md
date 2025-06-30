---
Name: QM-63_Federated Learning
Title: QM-63 Federated Learning
TitleGer: QM-63 Federated Learning
shortdesc: Federated Learning (FL) ist ein maschinelles Lernverfahren, bei dem Modelle trainiert werden, ohne dass die Trainingsdaten einen zentralen Speicherort verlassen
tags:
  - Qualitätsmetrik
ID:
  - QM-63
ListMetricID: 
ListMeasureID:
  - "'MA-26'"
MID: 
type:
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-63 Federated Learning

### Beschreibung

Federated Learning (FL) ist ein maschinelles Lernverfahren, bei dem Modelle trainiert werden, ohne dass die Trainingsdaten einen zentralen Speicherort verlassen. Stattdessen wird das Modell direkt auf den Geräten oder lokalen Servern der Datenbesitzer trainiert. Dieser Ansatz fördert den Datenschutz, da die sensiblen Daten lokal bleiben, während das Wissen durch aggregierte Modelle geteilt wird.

|Kriterium|Horizontal FL (HFL)|Vertical FL (VFL)|Federated Transfer Learning (FTL)|
|---|---|---|---|
|Merkmale (Features)|Identisch zwischen den Parteien.|Unterschiedlich zwischen den Parteien.|Teilweise unterschiedlich oder nur teilweise überlappend.|
|Datenpunkte (Samples)|Unterschiedliche Entitäten.|Gleiche Entitäten.|Teilweise überlappende Entitäten.|
|Überlappung der Daten|Hohe Überlappung der Features, keine der Samples.|Hohe Überlappung der Samples, keine der Features.|Geringe Überlappung bei Samples und/oder Features.|
|Transfer von Wissen|Nicht erforderlich.|Nicht erforderlich.|Transfer-Learning-Mechanismen werden verwendet.|
|Beispielanwendung|Banken mit Kundendaten und gleichen Features.|Bank und E-Commerce-Unternehmen mit gleichen Kunden.|Krankenhaus und Bilddatenbank mit begrenzter Überlappung.|

### Methoden

- Dezentrales Training:
	Anstatt die Daten zu einem zentralen Server zu senden, wird das Modell auf lokalen Daten trainiert (z. B. auf Smartphones, IoT-Geräten oder klinischen Datenbanken).

- Zentrale Aggregation:
    Nach einer lokalen Trainingsphase werden die Modellupdates (Gewichte oder Gradienten) an einen zentralen Server geschickt, der die Updates aggregiert, typischerweise durch Mittelwertbildung (z. B. Federated Averaging).

- Iterative Optimierung:
    Der aggregierte globale Modellzustand wird an die Geräte zurückgesandt, um weitere lokale Trainingsrunden durchzuführen. Dieser Prozess wird iterativ wiederholt.

- Privatsphäre und Sicherheit:
    Techniken wie Differential Privacy und Secure Aggregation werden eingesetzt, um sicherzustellen, dass individuelle Daten nicht aus den Modellupdates rekonstruiert werden können.


### Beispiele 

#### Beispiel 1 - Mobile Geräte:
- Verbesserung personalisierter Modelle für Texteingaben (z. B. Tastaturvorhersagen) oder Sprachassistenten (z. B. Google Assistant).

#### Beispiel 2 - Gesundheitswesen
- Training von Modellen zur Krankheitsdiagnose auf Daten aus verschiedenen Krankenhäusern, ohne die sensiblen Patientendaten auszutauschen.

### Ansätze
| Tool                                  | Kurzbeschr.                                                                                                                                                                                                                                                                     |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-63-1_Horizontal Federated Learning | Horizontal Federated Learning ist ein Ansatz, bei dem verschiedene Parteien Datensätze mit ähnlichen Merkmalen, aber unterschiedlichen Individuen besitzen, was ihn ideal für Szenarien macht, in denen identische Informationen über verschiedene Personen verteilt vorliegen. |
| QM-63-2_Vertical Federated Learning   | Vertical Federated Learning ermöglicht Parteien, überlappende Individuendaten mit unterschiedlichen Merkmalen gemeinsam auszuwerten, um ergänzende Informationen über dieselben Entitäten zu nutzen.                                                                            |
| QM-63-3_Federated Transfer Learning   | Federated Transfer Learning erweitert Federated Learning, um flexible Zusammenarbeit bei Parteien mit teils unterschiedlichen Merkmalen und Datensätzen zu ermöglichen.                                                                                                         |



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 165   |  Federated Machine Learning: Concept and Applications  | Der Text identifiziert Datensilos und Datenschutz als zentrale KI-Herausforderungen und schlägt ein erweitertes sicheres Federated Learning (horizontal, vertikal und transferbasiert) vor, um Wissensaustausch zwischen Organisationen ohne Verletzung der Privatsphäre zu ermöglichen. |



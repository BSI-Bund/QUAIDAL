---
Name: QM-63-1_Horizontal Federated Learning
Title: QM-63-1 Horizontal Federated Learning
TitleGer: QM-63-1 Horizontal Federated Learning
shortdesc: Horizontal Federated Learning ist ein Ansatz, bei dem verschiedene Parteien Datensätze mit ähnlichen Merkmalen, aber unterschiedlichen Individuen besitzen, was ihn ideal für Szenarien macht, in denen identische Informationen über verschiedene Personen verteilt vorliegen.
tags:
  - Qualitätsmetrik
  - "#ML-FedLearn"
  - ML-FedLearn
ID:
  - QM-63-1
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
## QM-63-1 Horizontal Federated Learning

### Beschreibung

Horizontal Federated Learning (HFL), auch bekannt als Sample-based Federated Learning, ist ein Ansatz im Federated Learning, bei dem verschiedene Parteien Datensätze mit ähnlichen Merkmalen (Features), aber unterschiedlichen Datensätzen von Individuen (Samples) besitzen. Dieser Ansatz eignet sich für Szenarien, in denen die Daten von verschiedenen Parteien die gleichen Arten von Informationen (z. B. identische Spalten oder Attribute) enthalten, aber von unterschiedlichen Personen stammen. Vorteile des HFL sind: 

- Datenschutz und Compliance:
	- Daten verbleiben lokal bei den Dateninhabern, wodurch Datenschutzrichtlinien wie die DSGVO eingehalten werden.
- Kollaboratives Lernen:
	- Parteien können gemeinsam ein leistungsfähigeres Modell trainieren, ohne ihre Daten direkt zu teilen.
- Einfachere Integration:
	- Da die Feature-Sets identisch sind, ist die Integration von Modellen und das Aggregieren von Updates weniger komplex.

### Methode

- Gleiche Feature-Sets
	- Alle Teilnehmer (z. B. Organisationen oder Geräte) teilen denselben Satz von Merkmalen. Ein Beispiel wäre ein Datensatz, der Informationen über Alter, Geschlecht und Einkommen enthält.
- Verschiedene Datenpunkte:
	- Die Teilnehmer haben Daten zu unterschiedlichen Individuen oder Einheiten. Es gibt keine oder nur minimale Überlappung zwischen den Datenpunkten (Zeilen) der verschiedenen Parteien.
- Dezentraler Ansatz:
    - Wie bei allgemeinem Federated Learning wird das Training des Modells auf den lokalen Daten durchgeführt, und nur die Modellupdates werden an einen zentralen Server geschickt.


### Beispiele 

#### Beispiel 1 

Zwei Banken, Bank A und Bank B, möchten ein Modell trainieren, um Kreditrisiken vorherzusagen.

- Beide Banken haben ähnliche Informationen über ihre Kunden (z. B. Einkommen, Alter, Kredithistorie).
- Die Kunden der beiden Banken überschneiden sich jedoch nicht.

Federated Learning Ansatz: 
- Jede Bank trainiert ein Modell auf ihren eigenen Kundendaten.
- Die Modellparameter (z. B. Gewichte) werden mit einem zentralen Server aggregiert, ohne dass Kundendaten ausgetauscht werden.
- Das globale Modell wird iterativ verbessert und zurück an die Banken gesendet.



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 165   |  Federated Machine Learning: Concept and Applications  | Der Text identifiziert Datensilos und Datenschutz als zentrale KI-Herausforderungen und schlägt ein erweitertes sicheres Federated Learning (horizontal, vertikal und transferbasiert) vor, um Wissensaustausch zwischen Organisationen ohne Verletzung der Privatsphäre zu ermöglichen. |



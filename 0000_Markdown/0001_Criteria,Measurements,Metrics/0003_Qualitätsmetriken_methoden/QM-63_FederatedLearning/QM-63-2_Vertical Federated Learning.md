---
Name: QM-63-2_Vertical Federated Learning
Title: QM-63-2 Vertical Federated Learning
TitleGer: QM-63-2 Vertical Federated Learning
shortdesc: Vertical Federated Learning ermöglicht Parteien, überlappende Individuendaten mit unterschiedlichen Merkmalen gemeinsam auszuwerten, um ergänzende Informationen über dieselben Entitäten zu nutzen.
tags:
  - Qualitätsmetrik
  - "#ML-FedLearn"
  - ML-FedLearn
ID:
  - QM-63-2
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
## QM-63-2 Vertical Federated Learning

### Beschreibung

Vertical Federated Learning (VFL), auch bekannt als Feature-based Federated Learning, ist ein Ansatz im Federated Learning, bei dem verschiedene Parteien Datensätze mit unterschiedlichen Merkmalen (Features), aber überlappenden Datensätzen von Individuen (Samples) besitzen. Dieser Ansatz wird in Szenarien verwendet, in denen verschiedene Organisationen oder Geräte Informationen über dieselben Entitäten (z. B. Kunden) speichern, aber unterschiedliche Arten von Attributen (z. B. Einkommensdaten vs. Einkaufsdaten) besitzen.

- Verschiedene Feature-Sets:
	Die Dateninhaber haben unterschiedliche Merkmale zu denselben Entitäten. Ein Beispiel wäre ein Unternehmen, das Einkommensdaten hat, und ein anderes Unternehmen, das Einkaufsverhalten kennt.

- Gleiche Datenpunkte (Samples):
	Die Datensätze der Parteien überschneiden sich hinsichtlich der Entitäten, z. B. haben beide Informationen über denselben Kunden.

- Koordination durch Identifikatoren:
	Ein gemeinsamer Schlüssel oder eine Methode zur sicheren Identifikation (z. B. Hashing) wird verwendet, um die Entitäten zwischen den Parteien abzugleichen, ohne sensible Informationen preiszugeben.

- Gemeinsames Modelltraining:
	Das Modell wird durch das kombinierte Wissen der verschiedenen Features trainiert. Dies geschieht, ohne dass die Rohdaten zwischen den Parteien ausgetauscht werden.

### Beispiele 

#### Beispiel 1 

Zwei Unternehmen, Bank A und E-Commerce-Unternehmen B, möchten ein Modell trainieren, um das Kreditrisiko ihrer gemeinsamen Kunden vorherzusagen.

- Bank A hat Informationen über das Einkommen und die Kredithistorie der Kunden.
- Unternehmen B hat Daten über das Einkaufsverhalten und die Online-Aktivitäten der gleichen Kunden.
- Beide Parteien möchten ihre Daten kombinieren, um ein leistungsfähigeres Modell zu trainieren, ohne ihre Rohdaten direkt auszutauschen.

Federated Learning Ansatz: 

- Beide Parteien stimmen ihre Kundenlisten ab (z. B. durch Hashing von Kundendaten).
- Ein gemeinsames Modell wird trainiert, wobei die Merkmale von Bank A und Unternehmen B kombiniert werden.
- Die Modellupdates werden iterativ aggregiert und verbessert.



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 165   |  Federated Machine Learning: Concept and Applications  | Der Text identifiziert Datensilos und Datenschutz als zentrale KI-Herausforderungen und schlägt ein erweitertes sicheres Federated Learning (horizontal, vertikal und transferbasiert) vor, um Wissensaustausch zwischen Organisationen ohne Verletzung der Privatsphäre zu ermöglichen. |


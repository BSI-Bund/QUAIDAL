---
Name: MA-26_Federated Learning
Title: MA-26 Federated Learning
TitleGer: MA-26 Federated Learning
shortdesc: Federated Learning ermöglicht das gemeinsame Trainieren von Modellen, ohne dass sensible Daten zentralisiert werden, um Datenschutz und Sicherheit zu gewährleisten.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-26
ListMetricID: 
ListMeasureID:
  - "'QB-10'"
MID: 
share: true
---
## MA-26 Federated Learning

### Beschreibung

Federated Learning (FL) ist ein maschinelles Lernverfahren, bei dem mehrere Geräte oder Server zusammenarbeiten, um ein gemeinsames Modell zu trainieren, ohne dass die Daten zentralisiert werden müssen. Statt alle Daten an einen zentralen Server zu senden, bleibt jede Datenquelle (zum Beispiel Smartphones, IoT-Geräte oder lokale Server) lokal. Diese Geräte trainieren das Modell individuell auf ihren lokalen Daten, und nur die trainierten Modellparameter (nicht die eigentlichen Daten) werden an den zentralen Server geschickt, wo sie aggregiert werden, um das globale Modell zu aktualisieren.

Das Ziel von Federated Learning ist es, Datenschutz und Sicherheit zu gewährleisten, indem sensible Daten nicht übertragen oder zentral gespeichert werden, während gleichzeitig die Vorteile gemeinsamer maschineller Lernmodelle genutzt werden. FL wird oft in Bereichen wie Gesundheit, Finanzen oder mobilen Anwendungen eingesetzt, wo der Schutz personenbezogener Daten wichtig ist.


### Beispiele 

#### Beispiel 1 - Personalisierte Texteingabe auf Smartphones

**Szenario**: Eine Smartphone-Tastatur-App lernt aus dem Schreibverhalten der Nutzer, um Wortvorschläge und Autokorrekturen zu verbessern. 

**Traditionell**: Alle Texteingaben der Nutzer müssten an einen zentralen Server gesendet werden, um das Modell zu verbessern. 

**Federated Learning**: Jedes Smartphone trainiert das Modell lokal basierend auf dem individuellen Schreibverhalten des Nutzers. Die trainierten Modellparameter werden an den Server gesendet, der sie aggregiert, um das globale Modell zu verbessern – ohne die privaten Texte der Nutzer zu teilen.

#### Beispiel 2 - Medizinische Forschung

**Szenario**: Verschiedene Nutzer verwenden Sprachassistenten in ihren Smart Homes, und die Assistenten sollen sich verbessern, um personalisierte Befehle besser zu verstehen. 

**Traditionell**: Sprachdaten der Nutzer müssten an einen zentralen Server geschickt werden, um die Spracherkennung zu verbessern. 

**Federated Learning**: Jeder Sprachassistent trainiert das Modell lokal auf den Sprachdaten des Nutzers. Die trainierten Parameter werden gesammelt und aggregiert, um die Erkennungsleistung zu verbessern, ohne dass die Audiodaten selbst jemals übertragen werden.


### Metriken & Methoden

| ID                                    | Kurzbeschr.                                                                                                                                                                                                                                                                     |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-63_Federated Learning              | Federated Learning (FL) ist ein maschinelles Lernverfahren, bei dem Modelle trainiert werden, ohne dass die Trainingsdaten einen zentralen Speicherort verlassen                                                                                                                |
| QM-63-1_Horizontal Federated Learning | Horizontal Federated Learning ist ein Ansatz, bei dem verschiedene Parteien Datensätze mit ähnlichen Merkmalen, aber unterschiedlichen Individuen besitzen, was ihn ideal für Szenarien macht, in denen identische Informationen über verschiedene Personen verteilt vorliegen. |
| QM-63-2_Vertical Federated Learning   | Vertical Federated Learning ermöglicht Parteien, überlappende Individuendaten mit unterschiedlichen Merkmalen gemeinsam auszuwerten, um ergänzende Informationen über dieselben Entitäten zu nutzen.                                                                            |
| QM-63-3_Federated Transfer Learning   | Federated Transfer Learning erweitert Federated Learning, um flexible Zusammenarbeit bei Parteien mit teils unterschiedlichen Merkmalen und Datensätzen zu ermöglichen.                                                                                                         |



### Referenzen

| RefID | Verweis                                                | Kurzbeschr.                                                                                                                                                                                                                                                                              |
| ----- | ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 165   |  Federated Machine Learning: Concept and Applications  | Der Text identifiziert Datensilos und Datenschutz als zentrale KI-Herausforderungen und schlägt ein erweitertes sicheres Federated Learning (horizontal, vertikal und transferbasiert) vor, um Wissensaustausch zwischen Organisationen ohne Verletzung der Privatsphäre zu ermöglichen. |

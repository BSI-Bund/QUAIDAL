---
Name: QM-70 Datasheet
Title: QM-70 Datasheet
TitleGer: QM-70 Datasheet
shortdesc: Datasheets beschreiben den Aufbau und Zweck von Datensätzen, definieren eine Vollständigkeitsmetrik und veranschaulichen deren Anwendung anhand konkreter Beispiele.
tags:
  - Qualitätsmetrik
ID:
  - QM-70
ListMetricID: 
ListMeasureID:
  - "'MA-18'"
  - "'MA-06'"
MID: 
type:
  - method
CodeEx: false
share: true
lcstep: pre
---
## QM-70 Datasheet

### Beschreibung
Datasheets für Datensätze sind strukturierte Dokumente, die den gesamten Lebenszyklus eines Datensatzes transparent machen – von Motivation und Komposition über Erhebungs- und Vorverarbeitungsprozesse bis hin zu empfohlenen Verwendungen und Wartungshinweisen. 

Im „QM-70_Datasheet“ fassen wir diese Informationen so zusammen, dass sie sowohl Dataset-Erstellern als auch -Nutzern ermöglichen, fundierte Entscheidungen zu treffen und unbeabsichtigten Missbrauch zu vermeiden. 

Datasheets fördern die Reproduzierbarkeit, da externe Forschende anhand der Dokumentation vergleichbare Datensätze mit ähnlichen Eigenschaften konstruieren können. 

Oft werden Datasheets für Datensätze auch als Data Statements (insbesondere im NLP-Bereich, vgl. Bender & Friedman 2018), Data Cards (leichtgewichtiges Pendant, vgl. Google Open Images) oder Factsheets (für AI-Services, vgl. IBM) bezeichnet.

– **Model Cards** dokumentieren Machine-Learning-Modelle, nicht den zugrundeliegenden Datensatz

– **Dataset Nutrition Labels** fokussieren auf statistische Eigenschaften und Risikoindikatoren, während Datasheets einen umfassenderen Lebenszyklus-Überblick bieten 

– **Automatisierte Dokumentationsprozesse** stehen im Widerspruch zum Ziel, dass Dataset-Ersteller bewusst über Annahmen und Risiken reflektieren sollten; Datasheets sollen daher manuell und nicht vollautomatisch erstellt werden

### Beispiele 

#### Beispiel 1 - Labeled Faces in the Wild (LFW)  

Gebru et al. haben eine Beispiel-Datasheet für LFW erstellt, in der sie Motivation, Komposition (Fotos von Gesichtern „in the wild“), Erhebungsprozess (Internet-Websites), Vorverarbeitungsschritte (Gesichtserkennung, Normalisierung) und Verwendungszwecke (Benchmarking von Gesichtserkennungsalgorithmen) dokumentieren:
- Beantwortete Fragen $n_(beantwortet)$: 42 von 50 → \(C = 84\%\)

#### Beispiel 2 - Pang & Lee’s Polarity Dataset  

In der Beispiel-Datasheet zu den Movie-Review-Daten beschreiben Pang & Lee, dass sie nur stark positive und negative Reviews extrahiert haben, wie sie die Sternebewertungen in Labels umwandeln und welche Vorverarbeitungsschritte (HTML-Entfernung, Boilerplate-Filterung) nötig waren:
- Beantwortete Fragen $n_(beantwortet)$: 48 von 50 → \(C = 96\%\)


### Referenzen

| RefID | Verweis                   | Kurzbeschr.                                                                                                                                                                                                                                                                          |
| ----- | ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 200   |  Datasheets for datasets  | Um Transparenz in der Machine-Learning-Community zu fördern, schlagen die Autoren standardisierte „Datasheets for Datasets“ vor, die analog zu technischen Datenblättern umfassende Informationen über Motivation, Zusammensetzung und Nutzung von Datensätzen dokumentieren sollen. |

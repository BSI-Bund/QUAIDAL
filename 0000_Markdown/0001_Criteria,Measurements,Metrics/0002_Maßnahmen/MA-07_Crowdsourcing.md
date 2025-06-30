---
Name: MA-07 Crowdsourcing
Title: MA-07 Crowdsourcing
TitleGer: MA-07 Massenbeteiligung
shortdesc: Einbeziehung größerer Menschengruppen zur Prüfung der Daten.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - unsicher
ID:
  - MA-07
ListMetricID: 
ListMeasureID:
  - "'QB-02'"
  - "'QB-06'"
share: true
---
## MA-07 Crowdsourcing

### Beschreibung

Crowdsourcing ist eine Methode, bei der Aufgaben, Datenannotation oder Informationsbeschaffung an eine große, heterogene Gruppe von Teilnehmenden („Crowd“) ausgelagert werden. Im Machine-Learning-Kontext wird Crowdsourcing häufig für Annotationen (z. B. Bild-, Text- oder Audio-Labels), Datensammlung und Validierung verwendet. Durch den Einsatz skalierbarer Online-Plattformen (wie Amazon Mechanical Turk, Prolific oder spezialisierte Data-Labeling-Dienste) lassen sich große Datenmengen schnell und kosteneffizient generieren. 

Synonyme für Crowdsourcing sind Schwarmintelligenz, Massenbeteiligung, Mitmach-Plattform oder Crowd-basierte Datenerhebung. Allen gemeinsam ist das Prinzip, Arbeit oder Wissen nicht intern im Projektteam, sondern dezentral über eine Community zu beziehen.

Ein zentrales Thema im Crowdsourcing ist Bias:
- **Demografischer Bias** entsteht, wenn die Crowd nicht repräsentativ für die Zielpopulation ist (z. B. nur bestimmte Alters- oder Bildungsgruppen).
- **Motivations- und Selektionsbias** tritt auf, wenn Teilnehmende Aufgaben aus reiner Monetarisierung erledigen und dabei Qualität vernachlässigen.
- **Instruction Bias** resultiert aus unklaren oder irreführenden Anweisungen, die unterschiedliche Interpretationen zulassen.
    
Diese Bias-Quellen können zu verzerrten Datensätzen führen, die wiederum Modelle in ihrer Generalisierbarkeit und Fairness einschränken. Beispielsweise kann ein sentiment-klassifizierter Text-Corpus, der überwiegend von jungen, technikaffinen Annotator:innen bearbeitet wurde, in anderen Alters- oder Zielgruppen schlechtere Ergebnisse liefern.

Abzugrenzen ist Crowdsourcing von Experten-Evaluation (MA-06): Während Crowdsourcing auf eine große, oft nicht-fachliche Gruppe setzt, erfolgen Expert:innen-Reviews durch wenige hochqualifizierte Fachleute. Ebenso unterscheidet es sich von automatisierten Data-Scraping-Verfahren, die Daten ohne menschliche Annotation sammeln, und von Active Learning, bei dem das Modell selbst die informativsten Beispiele zur Annotation auswählt. Crowdsourcing stellt somit einen Mittelweg zwischen reiner Automatisierung und spezialisierter Expertenarbeit dar.

### Beispiel - Klassifizierung von Daten 

Ein praktisches Beispiel für Crowdsourcing ist die Überprüfung und Klassifizierung von Daten, wie es in der Astronomie bei der Identifizierung von Galaxien oder in der Biologie bei der Katalogisierung von Arten verwendet wird. Teilnehmer, oft Laienforscher, tragen durch ihre Mitwirkung dazu bei, große Datenmengen effizienter zu verarbeiten, als es Wissenschaftler allein könnten. Diese Strategie fördert nicht nur die wissenschaftliche Forschung, sondern ermöglicht es auch Einzelpersonen, aktiv an Projekten teilzunehmen, die sie interessieren, und trägt zu ihrem Gefühl der Zugehörigkeit und des Beitrags zu einem größeren Ziel bei. Dieser Aspekt des Zugehörigkeitsgefühls lässt auch parallel die gefühlte Verantwortung für die Qualität der Daten wachsen. 

### Metriken & Methoden

Die Wirksamkeit von Crowdsourcing Maßnahmen kann durch unterschiedliche Maßnahmen geprüft werden.

| ID                               | Kurzbeschr.                                                                                                                                                                                    |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QM-03_F-Measure                  | F-Maß vereint Präzision und Trefferquote für Vorhersageleistung.                                                                                                                               |
| QM-16 Zuverlässigkeit            | Die Anzahl der Daten aus zuverlässigen Quellen bestimmt die Zuverlässigkeit                                                                                                                    |
| QM-16-1 Interrater-Reliabilität  | Inter-Rater-Reliabilität misst die Übereinstimmung zwischen verschiedenen Beurteilern oder Bewertern                                                                                           |
| QM-16-2 Test-Retest-Reliabilität | Die Test-Retest-Reliabilität wird durch Korrelation der Messwerte bei zwei verschiedenen Zeitpunkten berechnet                                                                                 |
| QM-16-3 Split-Half-Reliability   |  Maß für Konsistenz durch Aufteilung in zwei Hälften der Daten.                                                                                                                                |
| QM-16-4 Cronsbachsches Alpha     | Statistisches Maß zur Beurteilung der internen Konsistenz (Zuverlässigkeit) einer Skala oder eines Fragebogens, das angibt, wie eng verwandt die einzelnen Items einer Skala miteinander sind. |
| QM-43 Kreuzabgleich              | Ergebnisprüfung durch Kreuzabgleich verschiedener Quellen.                                                                                                                                     |



### Referenzen

| RefID | Verweis                                                                                                          | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ----- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 184   |  Quality Control in Crowdsourcing: A Survey of Quality Attributes, Assessment Techniques, and Assurance Actions  | Crowdsourcing nutzt große Gruppen, um Aufgaben wie Bildbeschriftung oder Texttranskription zu lösen, bei denen Computer Schwierigkeiten haben. Allerdings ist die Qualitätskontrolle aufgrund der unterschiedlichen Fähigkeiten und Motivationen der Teilnehmer eine Herausforderung. Diese Umfrage definiert die Crowdsourcing-Qualität, stellt ein Qualitätsmodell vor und untersucht Methoden zur Bewertung und Verbesserung der Qualität. Darüber hinaus werden aktuelle Lücken identifiziert und zukünftige Forschungsrichtungen vorgeschlagen. |
| 198   |  Deep Learning with Differential Privacy                                                                         | ML-Modelle, die neuronale Netzwerke verwenden, benötigen große Datensätze, die oft sensible Informationen enthalten. Um die Privatsphäre zu schützen, werden innerhalb des Rahmens der differentiellen Privatsphäre neue Techniken entwickelt. Dieser Ansatz ermöglicht das Training von tiefen neuronalen Netzwerken mit nicht-konvexen Zielen, während Privatsphäre, Softwarekomplexität, Trainingseffizienz und Modellqualität ausbalanciert werden.                                                                                              |

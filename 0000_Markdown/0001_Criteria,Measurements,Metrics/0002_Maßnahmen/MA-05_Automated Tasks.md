---
Name: MA-05 Automatisierte Aufgaben
Title: MA-05 Automatisierte Aufgaben
TitleGer: MA-05 Automatisierte Aufgaben
shortdesc: Skripte können wiederkehrende Aufgaben automatisieren
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - "#unsicher"
  - unsicher
ID:
  - MA-05
ListMetricID: 
ListMeasureID:
  - "'QB-10'"
  - "'QB-01'"
  - "'QB-02'"
lcstep: pre
share: true
---
## MA-05 Automatisierte Tasks auf Datensätzen

### Beschreibung

Automatisierte Tasks können bei der Beurteilung der Qualität und der Vorverarbeitung von Trainingsdaten verschiedene Formen annehmen. Je nach Zielprüfung werden andere Werkzeuge oder Methoden genutzt. 

Im Rahmen der Datenvorverarbeitung können bestimmte, als "Best Practice" identifizierte Prozesse automatisiert werden. Wiederkehrende Aufgaben im Lebenszyklus des KI-Systems können somit mit gleichbleibender Qualität automatisiert werden. 

### Beispiele 

#### Beispiel 1 - Integritätsprüfung

Im Vorfeld werden Richtlinien an die Daten definiert, die vor der manuellen Prüfung der Trainingsdaten automatisch durch autarke Systeme geprüft und evaluiert werden. Siehe MA-02 und MA-03.


#### Beispiel 2 - Feature Engineering Tests

Überprüfung der Korrelation zwischen Features, um multikolineare Features zu identifizieren und zu behandeln.


#### Beispiel 3 - Daten mit Personenbezug identifizieren

Durch Constraints können sie sicherstellen, dass alle personenbezogenen Daten anonymisiert oder pseudonymisiert sind. In diesem Kontext sind Constraints als "Best Practice" Regeln im Daten Lifecycle zu verstehen. 


#### Beispiel 4 - Automatisierte Generierung zusätzlicher Trainingsdaten 

Durch Techniken wie Rotation, Skalierung oder Hinzufügen von Rauschen in Bildern entsteht größere Variation auf den Datensätzen. 

#### Beispiel 5 - Semantische Ähnlichkeitsmessung mittels Embeddings  

Moderne Natural Language Processing (NLP)-Ansätze verwenden Wort- oder Satzvektoren (z.B. Word2Vec, BERT-Embeddings), um die semantische Nähe zwischen Texten zu berechnen. Mit diesen Methoden kann überprüft werden, ob Texte innerhalb derselben Kategorie oder mit demselben Label ähnliche semantische Repräsentationen besitzen.


### Metriken & Methoden


| ID                              | Kurzbeschr.                                                                                                                                                                                                                                                                                                              |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-10 Dimension Reduction       | hochdimensionale Trainingsdaten werden handhabbarer und interpretierbarer                                                                                                                                                                                                                                                |
| QM-34 Validierung der Feldgröße | Textfelder und Variablen auf erwartete Länge überprüfen. Automatisiert/expertengesteuert.                                                                                                                                                                                                                                |
| QM-64_Similarity Scores         | Die Wahl der Metrik zur Messung semantischer Ähnlichkeit ist kontextabhängig und reicht von Cosinus- und Soft-Cosine-Varianten bei Embeddings über den Jaccard-Koeffizienten bei spärlichen Darstellungen bis hin zu fortgeschrittenen Verfahren wie Word Mover’s Distance oder BERTScore für feine semantische Nuancen. |



### Referenzen

| RefID | Verweis                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                      |
| ----- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods  | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                                                              |
| 173   |  OWASP - Development-time threats – AI Exchange                                                            | Die OWASP-Seite beschreibt Risiken während der Entwicklung von KI-Systemen, wie Datenvergiftung, geistigen Diebstahl und Supply-Chain-Angriffe. Sie empfiehlt Schutzmaßnahmen wie Verschlüsselung, Datenisolation und Integritätsprüfungen, um Modelle und Daten zu sichern.                                     |
| 181   |  Data Quality Toolkit: Automatic assessment of data quality and remediation for machine learning datasets  | Das Data Quality Toolkit hilft dabei, Probleme mit Daten für maschinelles Lernen zu erkennen und zu beheben, indem es Bewertungen automatisiert und die Datenvorbereitung beschleunigt. Es ist über den IBM API Hub verfügbar, mit Tutorials auf dem IBM Learning Path.                                          |
| 182   |  QI2 -- an Interactive Tool for Data Quality Assurance                                                     | Der Artikel stellt einen Ansatz zur Sicherung und Überprüfung von Datenqualität vor, der am MNIST-Datensatz demonstriert wird. Dies wird im Kontext steigender Anforderungen durch ML-Systeme und den geplanten AI Act der EU behandelt.                                                                         |
| 222   |  Automatisiertes maschinelles Lernen (AutoML) \| Machine Learning \| Google for Developers                 | Der Google Machine Learning Crashkurs zu AutoML erklärt, wie man maschinelle Lernaufgaben wie Datenvorbereitung, Modellauswahl und Feinabstimmung automatisieren kann, was es Nicht-Experten erleichtert, präzise Modelle zu erstellen. Der Kurs behandelt wichtige AutoML-Komponenten und praktische Beispiele. |

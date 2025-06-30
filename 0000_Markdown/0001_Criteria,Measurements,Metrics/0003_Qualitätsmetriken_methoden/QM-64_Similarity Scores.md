---
Name: QM-64_Similarity Scores
Title: QM-64 Similarity Scores
TitleGer: QM-64 Similarity Scores
shortdesc: Die Wahl der Metrik zur Messung semantischer Ähnlichkeit ist kontextabhängig und reicht von Cosinus- und Soft-Cosine-Varianten bei Embeddings über den Jaccard-Koeffizienten bei spärlichen Darstellungen bis hin zu fortgeschrittenen Verfahren wie Word Mover’s Distance oder BERTScore für feine semantische Nuancen.
tags:
  - Qualitätsmetrik
ID:
  - QM-64
ListMetricID: 
ListMeasureID:
  - "'MA-05'"
MID: 
type:
  - metrik
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-64 Kennzahlen für Semantische Ähnlichkeit

### Beschreibung

Die Auswahl der geeigneten Metrik zur Messung der semantischen Ähnlichkeit in Trainingsdaten ist stark kontextabhängig. Für embeddingsbasierte Ansätze dominieren die Cosinus-Ähnlichkeit und Varianten davon (z.B. Soft-Cosine), während bei spärlichen Darstellungen häufig Metriken wie der Jaccard-Koeffizient Anwendung finden. Weiterhin können fortgeschrittene Methoden wie der Word Mover's Distance oder BERTScore in Szenarien, in denen semantische Nuancen im Vordergrund stehen, sehr hilfreich sein. Diese Vielfalt an Metriken ermöglicht es, je nach Datencharakteristik und Zielsetzung den optimalen Ansatz für die Messung der semantischen Ähnlichkeit zu wählen.

### Beispiele 

#### Beispiel 1 - Vektorraum-basierte Metriken

**a) Cosinus-Ähnlichkeit**

- **Beschreibung:** Diese Metrik misst den Winkel zwischen zwei Vektoren im Vektorraum und gibt einen Wert zwischen –1 und 1 zurück (bei positiv skalierenden Repräsentationen meist zwischen 0 und 1).
    
- **Anwendung:** Besonders beliebt bei der Arbeit mit dichten Vektor-Darstellungen (z.B. Word2Vec, GloVe, BERT), da sie unabhängig von der Vektorgröße ist und sich gut für semantische Vergleiche eignet.
    

**b) Euklidische Distanz**

- **Beschreibung:** Misst den "geraden" Abstand zwischen zwei Punkten im Vektorraum.
    
- **Anwendung:** Obwohl sie intuitiv verständlich ist, wird sie seltener für semantische Aufgaben gewählt, da der Abstand stark durch die Dimension und Skalierung der Vektoren beeinflusst wird.
    

**c) Manhattan-Distanz (Taxicab-Geodistanz)**

- **Beschreibung:** Anstatt der geraden Linie wird die Summe der absoluten Differenzen der Koordinaten berechnet.
    
- **Anwendung:** Kann in bestimmten Kontexten sinnvoll sein, insbesondere wenn man die Dimensionen einzeln betrachten möchte.
    

**d) Minkowski-Distanz**

- **Beschreibung:** Eine Verallgemeinerung von euklidischer und Manhattan-Distanz, die einen Parameter p verwendet.
    
- **Anwendung:** Ermöglicht Anpassungen an den spezifischen Abstand, den man messen möchte, wobei bei p=2 die euklidische und bei p=1 die Manhattan-Distanz entstehen.


#### Beispiel 2 - Ähnlichkeiten in diskreten oder sparsamen Darstellungen

**a) Jaccard-Ähnlichkeit**

- **Beschreibung:** Misst die Schnittmenge geteilter Elemente (zum Beispiel Wörter in Dokumenten) in Relation zur Vereinigungsmenge beider Mengen.
    
- **Anwendung:** Häufig genutzt in der Analyse von Bag-of-Words-Modellen oder bei der Arbeit mit Mengen, bei denen syntaktische Überlappungen wichtig sind.
    

**b) Overlap-Koeffizient (Satz-Overlap)**

- **Beschreibung:** Berechnet den Anteil der gemeinsamen Elemente relativ zur kleinsten Menge.
    
- **Anwendung:** Besonders nützlich, wenn der Fokus auf der Vollständigkeit von Elementen in kürzeren Texten liegt.


### Referenzen

| RefID | Verweis                                  | Kurzbeschr.                                                                                                                               |
| ----- | ---------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 193   |  Papers with Code - Semantic Similarity  | Die semantische Ähnlichkeit misst den Bedeutungsabstand sprachlicher Einheiten mittels wissensbasierter und verteilungsbasierter Ansätze. |

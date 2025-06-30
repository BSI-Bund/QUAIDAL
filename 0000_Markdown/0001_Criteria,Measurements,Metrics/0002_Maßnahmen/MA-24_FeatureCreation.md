---
Name: MA-24 Merkmalserstellung
Title: MA-24 Merkmalserstellung
TitleGer: MA-24 Merkmalserstellung
shortdesc: Methoden zur Generierung neuer Merkmale aus Rohdaten, um die Leistung von maschinellen Lernmodellen zu verbessern.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
ID:
  - MA-24
ListMetricID: 
ListMeasureID:
  - "'QB-12'"
  - "'QB-13'"
  - "'QB-06'"
MID: 
share: true
---
## MA-24 Merkmalserstellung / -entfernung

### Beschreibung

Hierbei werden neue aussagekräftige Merkmale (Features) aus den vorhandenen Rohdaten generiert, um die Leistung der anvisierten Modelle zu verbessern. In der Praxis bedeutet dies, dass zusätzliche oder unnütze Informationen oder Transformationen den vorhandenen Daten hinzugefügt oder entfernt werden, die dem Modell helfen, Muster besser zu erkennen und genauere Vorhersagen zu treffen. 

#### Filter-Methoden (Univariate Auswahl)

- **Varianz-Threshold:** Merkmale mit zu geringer Varianz werden entfernt, da sie kaum Information tragen. (QM-25-1) 
- **Pearson- und Spearman-Korrelation:** Numerische Merkmale werden auf linearen beziehungsweise monotonen Zusammenhang mit der Zielvariable untersucht.   (QM-11-1, QM-11-2)
- **Mutual Information:** Misst die allgemeine (nichtlineare) Abhängigkeit zwischen Merkmal und Ziel.  (QM-25, QM-27, QM-28)
- **Chi-Quadrat-Test:** Unabhängigkeitstest zwischen kategorialen Merkmalen und Zielklassen.  (QM-51-5)
- **ANOVA (Analysis of Variance) F-Wert:** Vergleich der Mittelwerte einer numerischen Variablen über verschiedene Zielklassen. 

#### Wrapper-Methoden

- **Recursive Feature Elimination (RFE):** Iteratives Entfernen der Merkmale mit geringster Wichtigkeit basierend auf einem zugrundeliegenden Modell.  
- **Forward Selection:** Beginnend mit leerer Merkmalsmenge werden sukzessive diejenigen Features hinzugefügt, die das Modell am stärksten verbessern.  
- **Backward Selection:** Beginnend mit allen Features werden sukzessive die unwichtigsten Merkmale entfernt.

#### Embedded-Methoden

- **LASSO (L1-Regularisierung):** Setzt Koeffizienten unwichtiger Features auf exakt null.  
- **Tree-basierte Modelle:** Random Forest oder Gradient Boosting liefern Feature Importances direkt aus den Splits.

#### Transformationstechniken (Feature Construction)

| Technik                         | Beschreibung                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------- |
| **Polynomiale Features**        | Erzeugung von Potenzen und Produkten wie x² oder x·y                            |
| **Interaktionsmerkmale**        | Kombination zweier Merkmale durch Produkt oder Quotient                         |
| **Skalierung / Normalisierung** | Min-Max-Skalierung oder Standardisierung (z-Transformation)                     |
| **Zeitbasierte Features**       | Extraktion von Wochentag, Monat, Stunde, Saison oder Zeit seit letztem Ereignis |
| **Text-Features (NLP)**         | Token-Counts, TF-IDF, Word2Vec/Doc2Vec oder BERT-Embeddings                     |
| **Decomposition**               | Dimensionsreduktion mittels PCA, t-SNE, UMAP oder Kernel-PCA                    |
| **Clustering**                  | Cluster-Labels als neue kategoriale Merkmale (z. B. K-Means, DBSCAN)            |
### Metriken & Methoden

| ID                                           | Kurzbeschr.                                                                                                                                                                                                                                                                          |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-11 Korrelationskoeffizient(diverse)       | Maß für lineare Beziehung zwischen Variablen.                                                                                                                                                                                                                                        |
| QM-11-1_Pearson-Korrelationskoeffizient      | Der Pearson-Korrelationskoeffizient ist ideal für kontinuierliche Daten auf einer Intervall- oder Verhältnisskala, um die Stärke und Richtung eines linearen Zusammenhangs zwischen zwei Variablen auf einer Skala von -1 bis 1 zu messen.                                           |
| QM-11-2_Spearman-Rangkorrelationskoeffizient | Der Spearman-Rangkorrelationskoeffizient ist ein nichtparametrisches Maß für die Stärke und Richtung einer monotonen Beziehung zwischen zwei Rangreihen von Variablen, besonders geeignet für ordinal oder kontinuierlich skalierte Daten mit Ausreißern oder ohne Normalverteilung. |
| QM-25-1_Variance-Treshold                    | Merkmale mit einer Varianz unter einem bestimmten Schwellenwert (Threshold) werden aus dem Datensatz entfernt.                                                                                                                                                                       |
| QM-26 Gini-Importance                        | Die Gini-Importance gibt an, wie viel eine Variable im Durchschnitt zur Verringerung der Gini-Unreinheit über alle Splits und alle Bäume eines Modells beiträgt und quantifiziert so ihre relative Bedeutung.                                                                        |
| QM-51-5 Chi-Quadrat Verteilung               | Verteilung zur Beschreibung quadratischer Abhängigkeiten von Zufallsvariablen                                                                                                                                                                                                        |
| QM-71 Polynomiale Features                   | Die polynomiale Feature-Erweiterung ist eine Technik zur Darstellung nicht-linearer Zusammenhänge in Daten durch Bildung höherer Potenzen und Kreuzterme aus ursprünglichen Merkmalen, um linearen Modellen komplexere Strukturen zugänglich zu machen.                              |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                           | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 89    |  Feature Engineering and Selection: A Practical Approach for Predictive Models: by Max Kuhn and Kjell Johnson. Boca Raton, FL: Chapman & Hall/CRC Press, 2019, xv + 297 pp., $79.95(H), ISBN: 978-1-13-807922-9.  | Der Prozess der Entwicklung prädiktiver Modelle umfasst viele Phasen. Die meisten Ressourcen konzentrieren sich auf Modellierungsalgorithmen, vernachlässigen jedoch andere entscheidende Aspekte des Prozesses. Dieses Buch beschreibt Techniken zur optimalen Darstellung von Prädiktoren für die Modellierung und zur Auswahl der besten Teilmenge von Prädiktoren, um die Modellleistung zu verbessern. |
| 157   |  It Is All about Data: A Survey on the Effects of Data on Adversarial Robustness                                                                                                                                  | Adversarial examples sind absichtlich gestaltete Eingaben, die maschinelle Lernmodelle verwirren, und dieses Survey untersucht, wie Eigenschaften von Trainingsdaten die Anfälligkeit für solche Angriffe beeinflussen sowie Methoden zur Verbesserung der adversarialen Robustheit durch verbesserte Datenrepräsentation und Lernverfahren.                                                                |

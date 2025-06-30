---
Name: MA-12 Abdeckung relevanter Merkmale
Title: MA-12 Abdeckung relevanter Merkmale
TitleGer: MA-12 Abdeckung relevanter Merkmale
shortdesc: Abdeckung aller wichtigen Merkmale im Datensatz zur Modellierung.
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - unsicher
ID:
  - MA-12
ListMetricID: 
ListMeasureID:
  - "'QM-65'"
  - "'QB-12'"
  - "'QB-05'"
  - "'QB-07'"
  - "'QB-04'"
  - "'QB-03'"
  - "'QB-06'"
lcstep: pre
share: true
---
## MA-12 Abdeckung relevanter Merkmale

### Beschreibung
Die **Abdeckung relevanter Merkmale** („Relevant Feature Coverage“) stellt sicher, dass der Trainingsdatensatz alle Variablen enthält, die für die zu lösende Fragestellung entscheidend sind. Ein unvollständiger Merkmals­raum führt sonst dazu, dass das Modell wichtige Zusammenhänge nicht lernt und folglich unzuverlässige Vorhersagen liefert.

#### Was bedeutet „Abdeckung“?

- **Vollständigkeit**: Alle identifizierten, für das Problem wesentlichen Features sind im Datensatz vorhanden.
- **Repräsentativität**: Jedes dieser Merkmale liegt in allen notwendigen Ausprägungen oder Wertebereichen vor (z. B. komplette Altersklassen, alle kategoriespezifischen Labels).
- **Qualität**: Die Daten für jedes Feature sind korrekt, valide und frei von systematischen Ausreißern oder Messfehlern.
    
#### Identifikation relevanter Merkmale

- **Domänenwissen** (MA-06)
    - Workshops mit Fachexpert*innen, um Hypothesen über Einflussgrößen zu sammeln.
- **Explorative Datenanalyse (EDA)** (MA-14)
    - Statistische Zusammenfassungen (z. B. Verteilung, fehlende Werte) pro Feature.
    - Visualisierungen (Boxplots, Histogramme, Scatterplots) zur Detektion relevanter Muster.
        
#### Methoden zur Überprüfung der Abdeckung

- **Feature-Importance-Analysen**
    - **Modellbasierte Ansätze** (z. B. Entscheidungsbäume, Random Forest): Ermitteln automatisch, welche Features den größten Beitrag zur Vorhersage leisten.
    - **Permutation Importance**: Misst, wie stark die Modellleistung leidet, wenn ein Feature zufällig permutiert wird.
    - **SHAP-Values** (SHapley Additive exPlanations): Zerlegt die Vorhersage jedes Datenpunkts in den Beitrag jedes Features und stellt so globale und lokale Wichtigkeit dar.
        
- **Korrelation und Redundanz**
    - **Korrelationsmatrizen**: Aufdeckung stark linear zusammenhängender Features, um sicherzugehen, dass kein relevantes Merkmal durch ein anderes überdeckt wird.
    - **Dimensionality Reduction** (z. B. PCA, t-SNE): Sichtbarmachung der wichtigsten Richtungen in den Daten; Hinweise auf fehlende Richtungskomponenten im Feature-Raum.
        
- **Coverage-Metriken**
    - **Wertebereichs-Check**: Prüfen, ob numerische Features im erwarteten Intervall vollständig vertreten sind (z. B. Alter 18–99).
    - **Kategorie-Balance**: Sicherstellen, dass nominale Merkmalsausprägungen (z. B. Bundesländer, Produktkategorien) nicht fehlen oder stark unterrepräsentiert sind.
        
- **Feature-Engineering-Audit**
    - Überprüfung, ob abgeleitete Features (z. B. Interaktions­terme, Zeitfensterkennzahlen) systematisch erzeugt und vollständig dokumentiert wurden.
        
#### Typische Fehlerquellen

- **Unentdeckte Einflussgrößen**: Manche wichtigen Features sind im Rohdatensatz gar nicht vorhanden und müssen extern erhoben oder abgeleitet werden.
- **Messausfälle**: Teilweise fehlende Werte in kritischen Features („Missing Not At Random“), die das Modell verzerren können.
- **Redundanz statt Abdeckung**: Viele hochkorrelierte Features, aber eigentlich fehlende echte Informationsdimensionen.
    

#### Best Practices

- **Iterativer Zyklus**: Abdeckungsmessung, Modelltraining, Analyse der Residualfehler – daraus neue Features ableiten.
- **Dokumentation**: Jede Feature-Quelle, jede Transformationsregel und jeder Abdeckungs-Check wird lückenlos protokolliert.
- **Automatisierte Prüfungen**: Deployment-Pipelines integrieren Skripte, die bei neuen Daten automatisch Coverage-Reports generieren und Grenzwert-Alarme auslösen.


### Metriken & Methoden

| ID                                                  | Kurzbeschr.                                                                                                                                                                                                                                                                          |
| --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| QM-10-1_PrincipalComponentAnalysis                  | PCA/HKA reduziert Dimensionalität, ermittelt Zusammenhänge durch Merkmalskorrelation.                                                                                                                                                                                                |
| QM-10-3_RobustPrincipalComponentAnalysis            | Robust Principal Component Analysis (RPCA) erweitert die klassische PCA, um robuster gegenüber Ausreißern und Störungen zu sein.                                                                                                                                                     |
| QM-11 Korrelationskoeffizient(diverse)              | Maß für lineare Beziehung zwischen Variablen.                                                                                                                                                                                                                                        |
| QM-11-1_Pearson-Korrelationskoeffizient             | Der Pearson-Korrelationskoeffizient ist ideal für kontinuierliche Daten auf einer Intervall- oder Verhältnisskala, um die Stärke und Richtung eines linearen Zusammenhangs zwischen zwei Variablen auf einer Skala von -1 bis 1 zu messen.                                           |
| QM-11-2_Spearman-Rangkorrelationskoeffizient        | Der Spearman-Rangkorrelationskoeffizient ist ein nichtparametrisches Maß für die Stärke und Richtung einer monotonen Beziehung zwischen zwei Rangreihen von Variablen, besonders geeignet für ordinal oder kontinuierlich skalierte Daten mit Ausreißern oder ohne Normalverteilung. |
| QM-11-3_Kendalls Tau                                | Kendall's Tau ist ideal für die Analyse monotone Beziehungen zwischen ordinalen oder rangbasierten Variablen, insbesondere bei nichtlinearen Zusammenhängen, Ausreißern, kleinen Stichproben oder Ties.                                                                              |
| QM-11-4_Koeffizient der punktbiserialen Korrelation | Der punktbiseriale Korrelationskoeffizient ist geeignet, um die Stärke und Richtung des Zusammenhangs zwischen einer dichotomen (binären) Variable und einer kontinuierlichen Variable zu messen, wie etwa den Einfluss des Geschlechts auf das Einkommen.                           |
| QM-11-5 Phi-Koeffizient                             | ist ein statistisches Maß für die Stärke des Zusammenhangs zwischen zwei dichotomen (binären) Variablen in einer 2x2-Kreuztabelle.                                                                                                                                                   |
| QM-13 Linear Discriminant Analysis                  | Die Lineare Diskriminanzanalyse (LDA) ist ein Verfahren zur Klassifikation, das lineare Trennlinien findet, um Datenpunkte anhand ihrer Merkmale optimal in vordefinierte Klassen zu unterteilen.                                                                                    |
| QM-25 Feature Importance Scores (diverse)           | Bewertet die Bedeutung für Merkmalen für ein bestimmtes Ergebnis                                                                                                                                                                                                                     |
| QM-26 Gini-Importance                               | Die Gini-Importance gibt an, wie viel eine Variable im Durchschnitt zur Verringerung der Gini-Unreinheit über alle Splits und alle Bäume eines Modells beiträgt und quantifiziert so ihre relative Bedeutung.                                                                        |
| QM-27 Permutation Feature Importance                | Methode zur Bestimmung der Bedeutung von Merkmalen                                                                                                                                                                                                                                   |
| QM-28 Koeffizienten linearer Modelle                | Gewichtungen für Merkmale in linearer Regressionsanalyse                                                                                                                                                                                                                             |
| QM-29 SHAP Feature Importance                       | SHAP misst den individuellen Beitrag jedes Features zur Modellvorhersage.                                                                                                                                                                                                            |



### Referenzen

| RefID | Verweis                                                                                   | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                      |
| ----- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 72    |  Feature engineering for machine learning: principles and techniques for data scientists  | Feature Engineering, ein entscheidender, jedoch oft übersehener Schritt in der Machine-Learning-Pipeline, umfasst die Extraktion und Transformation von Rohdaten in numerische Formate, die für Modelle geeignet sind. Dieses praxisorientierte Buch veranschaulicht dies anhand problembezogener Beispiele wie der Darstellung von Text- oder Bilddaten.                        |
| 157   |  It Is All about Data: A Survey on the Effects of Data on Adversarial Robustness          | Adversarial examples sind absichtlich gestaltete Eingaben, die maschinelle Lernmodelle verwirren, und dieses Survey untersucht, wie Eigenschaften von Trainingsdaten die Anfälligkeit für solche Angriffe beeinflussen sowie Methoden zur Verbesserung der adversarialen Robustheit durch verbesserte Datenrepräsentation und Lernverfahren.                                     |
| 191   |  The Effects of Data Quality on Machine Learning Performance                              | Moderne KI-Anwendungen erfordern große Mengen hochwertiger Daten. Unvollständige oder fehlerhafte Daten führen zu unzuverlässigen Modellen und schlechten Entscheidungen. Eine vertrauenswürdige KI ist auf genaue, vollständige und konsistente Daten angewiesen.                                                                                                               |
| 256   |  A Unified Approach to Interpreting Model Predictions                                     | SHAP (SHapley Additive exPlanations) ist ein einheitliches Rahmenwerk zur Interpretation von Modellvorhersagen, das einzelnen Merkmalen Wichtigkeitswerte zuweist, eine neue Klasse additiver Maße mit einer einzigartigen Lösung und erwünschten Eigenschaften einführt, bestehende Methoden vereinheitlicht und zudem die Rechenleistung sowie Interpretierbarkeit verbessert. |

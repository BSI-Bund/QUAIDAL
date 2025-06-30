---
Name: QM-29 SHAP Feature Importance
Title: QM-29 SHAP Feature Importance
TitleGer: QM-29 SHAP Feature Importance
shortdesc: SHAP misst den individuellen Beitrag jedes Features zur Modellvorhersage.
tags:
  - Qualitätsmetrik
  - ML-FeatureImpScore
ID:
  - QM-29
ListMetricID: 
ListMeasureID:
  - "'MA-10'"
  - "'MA-12'"
  - "'MA-14'"
MID: "38"
lcstep: post
CodeEx: true
share: true
type:
  - metrik
---
## QM-29 SHAP Feature Importance

### Beschreibung

SHAP (SHapley Additive exPlanations) Feature Importance erklärt, wie jedes Feature einen Beitrag zum Ergebnis eines Modells beiträgt. Es weist jedem Feature einen Shapley-Wert zu, der den durchschnittlichen Beitrag dieses Features über alle möglichen Kombinationen beschreibt. Damit bietet SHAP eine konsistente und faire Methode zur Interpretation der Feature-Wichtigkeit, indem es sowohl positive als auch negative Einflüsse auf die Modellvorhersage berücksichtigt.

#### Datenqualitätsverbesserung 

##### Erkennung von Verzerrungen 
Bei unausgeglichenen Trainingsdaten zeigen SHAP-Analysen, ob das Modell übermäßig stark auf Merkmale der dominanten Klasse zurückgreift. Dies eröffnet Möglichkeiten für gezieltes Resampling (z. B. durch SMOTE, siehe QM-57) oder die Nachjustierung betroffener Features.

##### Fehleranalyse  
Auffällige SHAP-Beiträge bei fehlerhaften Vorhersagen weisen auf potenzielle Schwächen in den Daten hin – etwa unzureichend repräsentierte Wertebereiche oder Messfehler.

#### Feature-Optimierung

##### Identifikation irrelevanter Features  
SHAP-Werte machen sichtbar, welche Merkmale über viele Vorhersagen hinweg nur geringen oder inkonsistenten Einfluss haben. Solche Features können entfernt werden, um Datenrauschen zu minimieren und die Komplexität des Modells zu reduzieren.

##### Entdeckung von Feature-Interaktionen  
Mithilfe von SHAP-Abhängigkeitsdiagrammen lassen sich nicht-lineare Zusammenhänge sowie Wechselwirkungen zwischen Features aufdecken. Diese Erkenntnisse ermöglichen die Konstruktion kombinierter, informativer Merkmale.

##### Priorisierung wichtiger Merkmale  
Der durchschnittliche absolute SHAP-Wert (Mean |SHAP|) dient als verlässliches Maß für die globale Bedeutung einzelner Features. Dadurch lassen sich gezielt die 20% der Merkmale identifizieren, die typischerweise 80% des Gesamtbeitrags zur Modellleistung liefern.

### Methode

- Trainieren des Modells: Ein Machine-Learning-Modell wird auf den Trainingsdaten trainiert, um Vorhersagen zu treffen.
    
- Berechnung der Shapley-Werte: Für jede Vorhersage werden Shapley-Werte für jedes Feature berechnet, indem die Vorhersageergebnisse mit und ohne dieses Feature für alle möglichen Kombinationen von Features verglichen werden. Diese Werte geben den Einfluss jedes Features auf die Modellvorhersage an.
    
- Aggregieren der Werte: Die Shapley-Werte werden über alle Vorhersagen und Datenpunkte aggregiert, um die durchschnittliche Bedeutung jedes Features zu berechnen. Diese aggregierten Werte können dann genutzt werden, um die Feature Importance im Modell zu interpretieren und zu visualisieren.

### Beispiele 

#### Beispiel - Kreditscoring

Es wurde ein Modell zur Vorhersage der Wahrscheinlichkeit entwickelt, dass ein Kunde einen Kredit nicht zurückzahlt. Das Modell verwendet mehrere Merkmale, wie etwa das Alter, das monatliche Einkommen, die Kreditsumme, die Beschäftigungsdauer und den Schufa-Score.

##### Beispielhafte Erklärung anhand eines Kundenprofils:

- **Kundenprofil:**
    - Alter: 45 Jahre
    - Monatliches Einkommen: 3.000€
    - Kreditsumme: 20.000€
    - Beschäftigungsdauer: 5 Jahre
    - Schufa-Score: 95

##### SHAP-Feature Importance erklärt:

SHAP (SHapley Additive exPlanations) berechnet für jedes Merkmal den Beitrag zur Vorhersage des Modells. Dabei wird untersucht, wie sich die Vorhersage ändert, wenn ein Merkmal zu einem "leeren" Modell hinzugefügt wird. Dieser Beitrag wird als SHAP-Wert dargestellt. Ein "leeres" Modell bezieht sich in diesem Kontext auf einen Ausgangszustand oder Basiswert eines Vorhersagemodells, bei dem noch keine spezifischen Eingabemerkmale berücksichtigt wurden. Das leere Modell stellt also eine Art Nullhypothese dar, von der aus man den Einfluss jedes einzelnen Merkmals messen kann. 


##### Beispielhafte SHAP-Werte:  

Angenommen, für unser Kundenprofil ergeben sich folgende vereinfachte SHAP-Werte:
- Alter: +0,10        
- Monatliches Einkommen: -0,05        
- Kreditsumme: +0,20        
- Beschäftigungsdauer: -0,03        
- Schufa-Score: -0,15        
    
##### Interpretation:    
- Ein positiver SHAP-Wert (z.B. Kreditsumme mit +0,20) zeigt an, dass dieses Merkmal den Ausfallwahrscheinlichkeitswert in Richtung eines höheren Risikos verschiebt.        
- Ein negativer SHAP-Wert (z.B. Schufa-Score mit -0,15) zeigt, dass dieses Merkmal den Wert in Richtung eines geringeren Risikos verschiebt.
        
##### Zusammenspiel der Werte:  
Wenn man alle SHAP-Werte addiert, ergibt sich die endgültige Modellvorhersage. In unserem Beispiel würden die Merkmale "Kreditsumme" und "Alter" den Risikowert erhöhen, während "monatliches Einkommen", "Beschäftigungsdauer" und insbesondere der "Schufa-Score" diesen senken.
    
##### Nutzen der Analyse:    
- **Priorisierung:** Der mittlere absolute SHAP-Wert über viele Kunden hinweg zeigt, dass z.B. die Kreditsumme oft der wichtigste Einflussfaktor ist.
- **Feature-Optimierung:** Erkennt man, dass einige Merkmale wie "Beschäftigungsdauer" nur einen geringen Einfluss haben, kann man diese in zukünftigen Modellen eventuell entfernen oder weniger gewichten.        
- **Interpretierbarkeit:** Für den einzelnen Kunden hilft die Aufschlüsselung der SHAP-Werte zu verstehen, welche Faktoren das Risiko erhöht oder verringert haben – wichtig für Transparenz und eventuelle Anpassungen im Kreditprozess.

### Sourcecode "SHAP Feature Importance"
| RefID | Verweis                              |
| ----- | ------------------------------------ |
| 27    | QM-29_SHAP Feature Importance_python |




### Referenzen
| RefID | Verweis                                                                             | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 81    |  The Shapley Value in Machine Learning                                              | In diesem Paper werden die grundlegenden Konzepte der kooperativen Spieltheorie und die axiomatischen Eigenschaften des Shapley-Werts diskutiert sowie dessen Anwendungen in der maschinellen Lernpraxis, einschließlich Merkmalsauswahl, Erklärbarkeit und Multi-Agenten-Verstärkungslernen, sowie die wichtigsten Einschränkungen und zukünftige Forschungsrichtungen aufgezeigt.                                                                                                       |
| 108   |  An introduction to explainable AI with Shapley values — SHAP latest documentation  | Die Webseite führt in erklärbare KI unter Verwendung von Shapley-Werten ein, welche die Interpretation von maschinellen Lernmodellen unterstützen, indem sie die Bedeutung einzelner Merkmale in Vorhersagen zuordnen. Es werden Beispiele mit dem SHAP-Paket von Python für verschiedene Modellarten vorgestellt.                                                                                                                                                                        |
| 228   |  Functional relevance based on the continuous Shapley value                         | Die Studie untersucht die Interpretierbarkeit von Modellen mit funktionalen Daten, die unendlich dimensionale Merkmale verwenden. Sie schlägt eine Methode basierend auf dem Shapley-Wert für kontinuierliche Spiele vor, um die Bedeutung der Prädiktoren fair zu verteilen. Im Fokus steht Scalar-on-Function-Regression. Experimente mit simulierten und realen Datensätzen zeigen die Anwendbarkeit der Methode. Zudem wird die Open-Source-Python-Bibliothek ShapleyFDA vorgestellt. |


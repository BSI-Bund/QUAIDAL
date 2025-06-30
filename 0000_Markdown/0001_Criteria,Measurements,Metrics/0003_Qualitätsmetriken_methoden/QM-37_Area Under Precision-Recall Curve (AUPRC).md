---
Name: QM-37_Area Under Precision-Recall Curve (AUPRC)
Title: QM-37 Area Under Precision-Recall Curve (AUPRC)
TitleGer: QM-37 Area Under Precision-Recall Curve (AUPRC)
shortdesc: Misst Gesamtleistung bei Präzision und Recall zusammen.
tags:
  - Qualitätsmetrik
ID:
  - QM-37
ListMetricID: 
ListMeasureID:
  - "'MA-10'"
MID: "46"
type:
  - method
lcstep: post
CodeEx: true
share: true
---
## QM-37 Area-Under-Precision-Recall Curve (AUPRC)

### Beschreibung

Die Area Under the Precision-Recall Curve (AUPRC) ist eine wichtige Metrik in der Maschinenlern- und Datenanalyse, besonders nützlich bei Klassifizierungsproblemen mit einem starken Ungleichgewicht in den Klassenverteilungen. Die Precision-Recall Curve zeigt die Beziehung zwischen Precision (Präzision) und Recall (Sensitivität) für verschiedene Schwellenwerte der Entscheidungsgrenze eines Klassifikators. 

Die AUPRC wird häufig verwendet, um die Leistung eines Modells zu messen, wenn die positiven Fälle viel seltener sind als die negativen. 

AUC-ROC grenzt sich gegen AUPRC durch die Wahl der betrachteten grundlegenden Konzepte des Modells. 
### Methoden:

####  1. Numerische Integration

Ähnlich wie bei der ROC-Kurve kann die Fläche unter der Precision-Recall Kurve numerisch berechnet werden, indem man die Fläche jedes Segments der Kurve aufsummiert. Dies kann durch Methoden wie die Trapezregel erfolgen, bei der die Kurve in eine Reihe von kleinen Trapezen oder Rechtecken aufgeteilt wird.

####  2. Nutzung von Bibliotheken in Programmiersprachen

In vielen modernen maschinellen Lernbibliotheken gibt es bereits eingebaute Funktionen zur Berechnung der AUPRC. Ein Beispiele für solche Funktion in Python (mit der Bibliothek Scikit-learn)

#### Interpretation: 

- **Precision und Recall**: Precision misst die Genauigkeit der positiven Vorhersagen des Modells, während Recall misst, wie gut das Modell alle tatsächlichen positiven Fälle erfasst. In Situationen, in denen falsch positive Werte hohe Kosten verursachen oder sehr nachteilig sind, kann die AUPRC eine wertvolle Metrik sein.
- **Datenungleichgewicht**: Die AUPRC ist besonders in Szenarien nützlich, wo es eine signifikante Unausgewogenheit zwischen den Klassen gibt (z.B. bei der Erkennung von Betrug, wo echte Betrugsfälle selten sind).
- **Leistung des Klasifikators**: Ein höherer Wert der AUPRC deutet auf eine bessere Leistung des Modells hin. Ein perfekter Klassifikator hätte eine AUPRC von 1, während ein Klassifikator, der keine nützliche Unterscheidung zwischen den Klassen trifft, eine AUPRC nahe 0 haben würde.


### Sourcecode "Area Under Precision-Recall Curve (AUPRC)"

| RefID | Verweis                                                |
| ----- | ------------------------------------------------------ |
| 30    | QM-37_Area Under Precision-Recall Curve (AUPRC)_python |



### Referenzen

| RefID | Verweis                                                                                                                               | Kurzbeschr.                                                                                                  |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance  | Information technology — Artificial intelligence — Assessment of machine learning classification performance |


---
Name: QM-07 Spezifität
Title: QM-07 Spezifität
TitleGer: QM-07 Spezifizität
shortdesc: Misst die Fähigkeit echte Positivwerte zu erkennen
tags:
  - Qualitätsmetrik
ID:
  - QM-07
ListMetricID: 
ListMeasureID:
  - "'MA-27'"
MID: "7"
type:
  - metric
CodeEx: true
share: true
lcstep: post
---
## QM-07 Spezifität

### Beschreibung

In ML-Modellen, speziell bei Klassifikationsaufgaben, ist die Specificity (Spezifität) eine Metrik, die die Fähigkeit eines Modells misst, tatsächlich negative Fälle korrekt als negativ zu identifizieren. Sie ergänzt den Recall, der sich auf die Identifikation von positiven Fällen konzentriert, indem sie bewertet, wie gut das Modell Nicht-Ereignisse erkennt und korrekt klassifiziert.

Die Specificity ist besonders wichtig in Situationen, in denen falsch positive Ergebnisse zu unnötigen oder schädlichen Folgemaßnahmen führen könnten, wie beispielsweise in der medizinischen Diagnostik, wo eine hohe Specificity die Wahrscheinlichkeit unnötiger Behandlungen verringert. In vielen Anwendungen wird ein Gleichgewicht zwischen Recall und Specificity angestrebt, um sicherzustellen, dass das Modell sowohl effektiv relevante Fälle identifiziert als auch nicht relevante Fälle korrekt ausschließt.

### Formel

- **Klassifikationsergebnisse sammeln**: Zunächst müssen alle Testergebnisse des Modells vorliegen. In diesem Zusammenhang gibt es vier mögliche Resultate:
    - **True Positives (TP)**: Das Modell sagt korrekt voraus, dass etwas positiv ist.
    - **False Positives (FP)**: Das Modell sagt fälschlicherweise voraus, dass etwas positiv ist, obwohl es negativ ist.
    - **True Negatives (TN)**: Das Modell sagt korrekt voraus, dass etwas negativ ist.
    - **False Negatives (FN)**: Das Modell sagt fälschlicherweise voraus, dass etwas negativ ist, obwohl es positiv ist.
- **Betrachte nur die negativen Fälle**: Um die Specificity zu berechnen, konzentrieren wir uns auf die negativen Fälle. Das heißt, wir schauen nur darauf, wie gut das Modell die tatsächlichen negativen Fälle behandelt.
- **Richtige negative Vorhersagen zählen**: Nun zählen wir die **True Negatives** (TN), also die Fälle, in denen das Modell korrekt erkannt hat, dass etwas negativ ist.
- **Alle tatsächlichen negativen Fälle identifizieren**: Jetzt addieren wir alle tatsächlichen negativen Fälle, das heißt, sowohl die True Negatives (TN) als auch die False Positives (FP). Das sind alle Fälle, bei denen das tatsächliche Ergebnis negativ ist, unabhängig davon, ob das Modell richtig oder falsch lag.
- **Verhältnis berechnen**: Specificity ist dann das Verhältnis zwischen den True Negatives (richtige negative Vorhersagen) und der Summe aller tatsächlichen negativen Fälle (True Negatives + False Positives).

#### Interpretation 

- **Hohe Spezifizität (nahe 1)**: Das Modell macht wenige **False Positive**-Fehler. Das bedeutet, dass das Modell selten Fälle fälschlicherweise als positiv klassifiziert, wenn sie tatsächlich negativ sind. In einem medizinischen Kontext bedeutet dies, dass gesunde Personen selten fälschlicherweise als krank eingestuft werden.
- **Niedrige Spezifizität (nahe 0)**: Das Modell macht viele **False Positive**-Fehler, d.h., es klassifiziert viele negative Fälle fälschlicherweise als positiv. Ein Beispiel wäre ein medizinischer Test, der gesunde Personen oft als krank diagnostiziert.

### Python Code für "Specificity"

| RefID | Verweis                  |
| ----- | ------------------------ |
| 7     | QM-07_Specificity_python |



### Referenzen

| RefID | Verweis                                                                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 122   |  Sensitivity and specificity                                                                                                          | Die Sensitivität misst die Fähigkeit eines Tests, richtig positive Ergebnisse korrekt zu identifizieren, während die Spezifität seine Fähigkeit misst, richtig negative Ergebnisse korrekt zu identifizieren. Es gibt oft einen Kompromiss zwischen den beiden, wobei die Erhöhung des einen den anderen verringern kann. Sensibilität ist von entscheidender Bedeutung, wenn das Übersehen einer Erkrankung riskant ist, und Spezifität ist wichtig, um unnötige Konsequenzen für Personen ohne diese Erkrankung zu vermeiden. |
| 126   |  Statista - das Statistik-Portal: Statistiken, Marktdaten & Studien                                                                   | Statista ist eine Datenplattform, die Statistiken und Berichte aus verschiedenen Branchen und Märkten bereitstellt. Sie bietet Umfragen, Prognosen und Analysen zu Themen wie Wirtschaft, Gesellschaft und Technologie für Unternehmen, Forscher und Medien.                                                                                                                                                                                                                                                                    |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance  | Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                                                                                                                                                                                                                                                                                                                                                                                    |

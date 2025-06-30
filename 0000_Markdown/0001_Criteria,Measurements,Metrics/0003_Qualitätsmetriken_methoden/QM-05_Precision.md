---
Name: QM-05_Precision
Title: QM-05 Precision
TitleGer: QM-05 Präzision
shortdesc: Verhältnis korrekter positiver Vorhersagen zu allen Positiven.
tags:
  - Qualitätsmetrik
ID:
  - QM-05
ListMetricID: 
ListMeasureID:
  - MA-8
  - "'MA-08'"
MID: "5"
type:
  - metric
CodeEx: true
share: true
lcstep: post
---
## QM-05 Präzision

### Beschreibung

Die Präzision bezeichnet eine Leistungsmetrik, die insbesondere bei Klassifikationsproblemen verwendet wird. Die Präzision gibt an, wie viele der als positiv klassifizierten Fälle tatsächlich positiv sind. Sie ist besonders nützlich in Szenarien, in denen die Kosten für falsch positive Ergebnisse hoch sind.

Formal wird die Präzision berechnet als das Verhältnis von wahren positiven Vorhersagen (d.h. die Anzahl der korrekt identifizierten positiven Fälle) zur Gesamtzahl der als positiv klassifizierten Fälle (d.h. die Summe aus wahren positiven und falsch positiven Vorhersagen)

Die Präzision ist nicht zu verwechseln mit der Genauigkeit (engl. Accuracy).

### Methode

- Positive Vorhersagen prüfen: Zuerst schaust du dir alle Fälle an, bei denen das Modell vorhersagt, dass sie zu einer bestimmten Kategorie gehören (z.B. alle Fälle, bei denen das Modell "Ja" oder "Positiv" gesagt hat).
- Richtige Vorhersagen ermitteln: Von diesen positiven Vorhersagen schaust du, wie viele davon tatsächlich korrekt sind, also wie viele dieser Vorhersagen in der Realität auch wirklich positiv sind (d.h. es wurde „Ja“ vorhergesagt und tatsächlich ist es „Ja“).
- Präzision bestimmen: Die Präzision zeigt dir dann den Anteil der korrekt vorhergesagten positiven Fälle an allen Fällen, die das Modell als positiv markiert hat. Sie beantwortet die Frage: "Wie viele der als positiv vorhergesagten Fälle sind wirklich positiv?".


### Python Code für "Precision"
| RefID | Verweis                |
| ----- | ---------------------- |
| 5     | QM-05_Precision_python |



### Referenzen
| RefID | Verweis                                                                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                  |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 126   |  Statista - das Statistik-Portal: Statistiken, Marktdaten & Studien                                                                   | Statista ist eine Datenplattform, die Statistiken und Berichte aus verschiedenen Branchen und Märkten bereitstellt. Sie bietet Umfragen, Prognosen und Analysen zu Themen wie Wirtschaft, Gesellschaft und Technologie für Unternehmen, Forscher und Medien. |
| 276   |  ISO/IEC TS 4213:2022 - Information technology — Artificial intelligence — Assessment of machine learning classification performance  | Information technology — Artificial intelligence — Assessment of machine learning classification performance                                                                                                                                                 |

---
Name: QM-71 Polynomiale Features
Title: QM-71 Polynomiale Features
TitleGer: ""
shortdesc: Die polynomiale Feature-Erweiterung ist eine Technik zur Darstellung nicht-linearer Zusammenhänge in Daten durch Bildung höherer Potenzen und Kreuzterme aus ursprünglichen Merkmalen, um linearen Modellen komplexere Strukturen zugänglich zu machen.
tags:
  - Qualitätsmetrik
ID:
  - QM-71
ListMetricID: 
ListMeasureID:
  - "'MA-24'"
MID: 
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-71-1 Polynomiale Features

### Beschreibung

Feature Creation mit Polynomialen Features ist eine Technik der Feature-Erweiterung in maschinellen Lernverfahren, bei der aus den ursprünglichen Merkmalen höhergradige Terme gebildet werden $(z. B. x^2, x^3)$ oder Produkte $(x_i x_j​)$. Ziel ist es, nicht-lineare Zusammenhänge in den Daten für lineare Modelle erfassbar zu machen.

Synonyme für polynomiale Feature-Erweiterung sind **Polynomial Expansion**, **Basis-Expansion** und **Polynomial Transformation**. In der Statistik spricht man teils auch von **Moment Features**, wenn explizit Potenzen einzelner Variablen betrachtet werden.

Abzugrenzen ist diese Methode von ähnlichen Techniken wie **Interaktionsfeatures** (nur Produkte ohne höhere Potenzen) und **Fourier-Features** (Sinus-/Kosinus-Basis). Während polynomiale Features Potenzen und Kreuzterme hoher Ordnung generieren, modellieren Interaktionsfeatures allein Wechselwirkungen erster Ordnung, und Fourier-Features legen den Schwerpunkt auf periodische Basisfunktionen.

### Sourcecode "Polynomiale Features"
| RefID | Verweis                           |
| ----- | --------------------------------- |
| 94    | QM-71 Polynomiale Features_python |



### Referenzen
| RefID | Verweis                                                                        | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 180   |  The elements of statistical learning: data mining, inference, and prediction  | Dieses Buch bietet einen umfassenden Überblick über Schlüsselkonzepte des Data Mining in Bereichen wie Medizin und Finanzen und konzentriert sich dabei auf überwachtes und unüberwachtes Lernen. Es behandelt Themen wie neuronale Netze, Boosting und fügt neue Inhalte zu Random Forests, Ensemble-Methoden und dem Umgang mit „großen“ Daten hinzu. Es ist nützlich für Statistiker und diejenigen, die in der Wissenschaft oder Industrie tätig sind. |

---
Name: QM-44-7 LLM-basierte Imputation
Title: QM-44-7 LLM-basierte Imputation
TitleGer: QM-44-7 LLM-basierte Imputation
shortdesc: LLM Modelle sagen fehlende Werte anhand der Umgebungsvariablen voraus
tags:
  - Qualitätsmetrik
  - ML-Data-Imp
ID:
  - QM-44-7
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: "61"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-44-7 LLM-basierte Imputation

### Beschreibung

Die Daten-Imputation durch die Verwendung von Large Language Models (LLMs) ist ein relativ neuer Ansatz, der darauf abzielt, die Fähigkeiten von LLMs zur Text- und Dateninterpretation zu nutzen, um fehlende oder unvollständige Informationen in Datensätzen zu ergänzen. 

#### Vorteile von LLM-basierter Imputation
- Flexibilität: Kann sowohl für textbasierte als auch für strukturierte Daten verwendet werden.
- Kontextbewusstsein: Nutzt umfassendes Wissen und Kontextverständnis zur Generierung plausibler Datenpunkte.
- Skalierbarkeit: Kann leicht auf große Datensätze angewendet werden.

#### Herausforderungen
- Bias und Varianz: LLMs können bestehende Vorurteile in Trainingsdaten widerspiegeln.
- Transparenz und Erklärbarkeit: Die von LLMs generierten Imputationen können schwer zu interpretieren sein, besonders wenn es um komplexe oder indirekte Zusammenhänge geht.

LLM-basierte Daten-Imputation ist ein vielversprechender Ansatz, der jedoch sorgfältig eingesetzt und validiert werden sollte, um die besten Ergebnisse zu erzielen.


### Methode

- Daten-Initialisierung
Laden des unvollständigen Datensatzes. 

- Laden des Modells und Tokenizers
Ein vortrainiertes Sprachmodell (Language Model) wird aus einer Bibliothek wie Hugging Face geladen. Parallel dazu wird ein Tokenizer initialisiert, der den Text in eine Form bringt, die vom Modell verarbeitet werden kann.

- Erstellen einer Imputationfunktion
Eine Funktion wird definiert, die überprüft, ob Werte fehlen. Falls ein Wert fehlt, wird ein Eingabe-Prompt erstellt, der das Modell dazu auffordert, auf Basis des vorhandenen Kontexts (wie anderer Felder im Datensatz) den fehlenden Wert zu generieren. Das Modell wandelt den Prompt in eine Textvorhersage um, die als Imputation für den fehlenden Wert verwendet wird.

- Anwendung der Imputation
Die Imputationsfunktion wird auf den gesamten Datensatz angewendet. Für jede Zeile wird überprüft, ob Werte fehlen, und falls dies der Fall ist, wird die Funktion aufgerufen, um den fehlenden Wert zu ergänzen.

- Zusammenfassung und Prüfung der Ergebnisse
Der vervollständigte Datensatz wird ausgegeben, wobei die zuvor fehlenden Werte durch vom Modell generierte Werte ersetzt wurden. 


### Sourcecode "LLM-Based Imputation"
| RefID | Verweis                             |
| ----- | ----------------------------------- |
| 43    | QM-44-7_LLM-Based Imputation_python |


### Referenzen
| RefID | Verweis                                                                | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                  |
| ----- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 76    |  Quantitative knowledge retrieval from large language models           | In diesem Paper wird die Machbarkeit von großen Sprachmodellen (LLMs) als Mechanismus für die quantitative Wissensabfrage untersucht, um bei Datenanalyseaufgaben wie der Erhebung von Priorverteilungen für bayesianische Modelle und der Imputation fehlender Daten zu unterstützen, wobei ein Framework für Prompt-Engineering und Herausforderungen der Nutzung von LLMs als Experten diskutiert werden. |
| 156   |  6.4. Imputation of missing values — scikit-learn 1.5.2 documentation  | Die Seite erklärt, wie fehlende Daten in scikit-learn durch verschiedene Imputationstechniken wie den SimpleImputer, IterativeImputer und KNNImputer basierend auf vorhandenen Daten geschätzt und ersetzt werden können.                                                                                                                                                                                    |

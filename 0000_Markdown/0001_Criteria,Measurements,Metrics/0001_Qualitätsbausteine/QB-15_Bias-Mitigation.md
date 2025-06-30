---
Name: QB-15_Bias-Mitigation
Title: QB-15 Bias-Mitigation
TitleGer: QB-15 Bias-Mitigation
shortdesc: Der Baustein beschreibt technische Verfahren zur Reduzierung von Verzerrungen in KI-Modellen, die idealerweise bereits bei der Datenerhebung ansetzen und sich je nach Zeitpunkt ihres Einsatzes im Entwicklungszyklus in Präprozessierungs-, Inprozessierungs- und Postprozessierungsmethoden gliedern, wie anhand eines Bewerbungs-Beispiels veranschaulicht wird.
tags:
  - Qualitätsbaustein
ID:
  - QB-15
ListMeasureID:
  - "'QKB-01'"
ListCritID:
  - "'QKB-01'"
lcstep: 
share: true
---
## QB-15_Bias-Mitigation

### Beschreibung 

Der Baustein Bias-Mitigation erläutert technische Verfahren zur Reduzierung oder Verhinderung von Verzerrungen (Bias) in KI-Modellen. Bias-Mitigation-Maßnahmen lassen sich je nach Zeitpunkt ihres Einsatzes im Entwicklungszyklus in drei Klassen einteilen:

- **Präprozessierungsmethoden**: Veränderungen an den Trainingsdaten vor dem Modelltraining, um Ungleichgewichte auszugleichen (z. B. Label-Massaging, Upsampling/Downsampling, SMOTE).
- **Inprozessierungsmethoden**: Anpassung des Lernverfahrens selbst, etwa durch Regularisierung oder adversariales Training, um Bias während des Trainings direkt zu minimieren. 
- **Postprozessierungsmethoden**: Nachträgliche Anpassung der Modellausgaben, zum Beispiel durch Calibrations oder Fairness-Constraints auf Score-Ebene.

Idealerweise beginnt Bias-Mitigation bereits bei der Datenerhebung durch sorgfältiges Studiendesign und geeignete Frage- und Aufnahmesysteme. Wo das nicht vollständig möglich ist, gleichen die vorgestellten Verfahren verbleibende Verzerrungen aus.

Im vorliegenden Kapitel veranschaulichen wir die Methoden anhand eines Bewerbungs-Beispiels: KI-Modelle bewerten quantifizierbare Merkmale von Bewerbenden (z. B. Bildungsabschluss, Berufserfahrung, Sprachkenntnisse) und sagen binär voraus, ob eine Person eingestellt wird. Bias kann auch dann entstehen, wenn sensitive Merkmale wie Geschlechtsidentität nur implizit in den Daten abgebildet sind („Fairness through Unawareness“ verhindert Bias nicht).

**Synonyme für Bias-Mitigation** sind unter anderem „Verzerrungsreduktion“, „Bias-Reduktion“, „Fairness-Enhancement“ oder „Bias Correction“. Allen Begriffen gemeinsam ist das Ziel, erkannte oder latente Benachteiligungen aktiv zu verringern.
   
### Beispiele

#### Beispiel 1: Präprozessierung mit SMOTE

Im Bewerbungs-Szenario zeigt sich, dass deutlich weniger Bewerbungen von Frauen vorliegen. Mithilfe von **SMOTE** (QM-57 Synthetic Minority Over-sampling Technique) werden synthetische Datenpunkte für die unterrepräsentierte Gruppe erzeugt, sodass das Trainingsset ausgeglichener wird. Dadurch lernt das Modell Muster, die auch für die Minderheit repräsentativ sind, und erzielt eine faire Vorhersageleistung über alle Subpopulationen hinweg.

#### Beispiel 2: Inprozessierung mit Learning Fair Representations

Bei der Inprozessierung nutzen wir den Algorithmus **Learning Fair Representations (LFR)**. Hierbei werden Prototypen als latente Repräsentationen gelernt, die einerseits die Informationskraft für die Einstellungsentscheidung maximieren und andererseits sicherstellen, dass Bewerbende verschiedener Gruppen gleich häufig auf die Prototypen projiziert werden (statistische Parität). Ergänzend kann adversariales Training eingesetzt werden, um ein Detektor-Netzwerk zu verhindern, das Gruppenunterschiede aus den Repräsentationen extrahiert.

### Maßnahmen

| Maßnahme       | Kurzbeschr.                                                                                                                                                                                                                         |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MA-30_Fairness | Fairness im Machine Learning bezeichnet Techniken (z. B. SMOTE, LFR), die systematische Verzerrungen in Daten und Modellen korrigieren, um gerechte, gleichbehandelte Vorhersagen für alle demografischen Gruppen zu gewährleisten. |


### Referenzen

| RefID | Verweis                                                                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                    |
| ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 131   |  Security of AI-Systems: Fundamentals - Adversarial Deep Learning                                                                                          | Im Projekt 464, Teilprojekt 1 Sicherheit von KI-Systemen: Adversariales Deep Learning, untersuchte das BSI die Sicherheit von Verbindungssystemen in neuronalen Netzwerken und präsentierte Best-Practice-Richtlinien für die Zertifizierung und Verifizierung von neuronalen Netzwerken sowie Verteidigungstechniken gegen Angriffe wie Evasion, Poisoning, Backdoor und Datenschutzangriffe. |
| 230   |  ISO/IEC TS 12791 - Information technology — Artificial intelligence — Treatment of unwanted bias in classification and regression machine learning tasks  | Information Technology – Artificial Intelligence – Behandlung unerwünschter Verzerrungen bei Klassifizierungs- und Regressionsaufgaben des maschinellen Lernens                                                                                                                                                                                                                                |
| 296   |  Bias in der künstlichen Intelligenz                                                                                                                       | Das Dokument Bias in der künstlichen Intelligenz befasst sich mit den Grundlagen und zeigt Detektion und Mitigationsmechanismen auf um Bias in den eigenen Datensätzen auf die Spur zu kommen.                                                                                                                                                                                                 |



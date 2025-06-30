---
Name: QM-31 Prozessanalysemetriken
Title: QM-31 Prozessanalysemetriken
TitleGer: QM-31 Prozessanalysemetriken
shortdesc: Prozessbewertung bzgl. verschiedener Themen
tags:
  - Qualitätsmetrik
ID:
  - QM-31
ListMetricID: 
ListMeasureID:
  - "'MA-20'"
MID: "40"
type:
  - method
CodeEx: true
share: true
lcstep: pre
---
## QM-31 Prozess Analyse Ansätze

### Beschreibung
  
Die Bewertung der Wirksamkeit eines Prozesses im AI-Lifecycle eines KI-Modells kann durch verschiedene Metriken erfolgen. Relevant sind verschiedene spezifische Aspekte wie Effizienz, Qualität, Kosten, Flexibilität, Zuverlässigkeit, Compliance und Zielerreichung. Messbare Metriken werden häufig für einzelne Elemente usecase-spezifisch hergeleitet. 

### Methode

#### Effizienz
- Durchlaufzeit: Misst die Zeit vom Beginn bis zum Abschluss einer bestimmten Phase im AI-Lifecycle, um Engpässe zu identifizieren. Bspw. Zeitserienanalyse über mehrere Iterationen. 
- Ressourcenauslastung: Beurteilt, wie effektiv die verfügbaren Ressourcen (z.B. Rechenkapazitäten, Speicher) genutzt werden. Bsp.: Konfiguration des AI Lifecycle auf optimale Ausnutzung beobachten und dahingehend optimieren. 

#### Qualität
- Modellgenauigkeit: Anteil korrekt vorhergesagter Werte im Verhältnis zu den tatsächlichen Werten.
- Fehlerrate: Anteil der inkorrekten Vorhersagen oder Aktionen des Modells.
- Validierungs- und Testergebnisse: Ergebnisse aus Validierungs- und Testphasen, die Aufschluss über die Modellleistung geben.

#### Kosten
- Gesamtkosten: Summe aller Kosten, die mit dem Prozess verbunden sind, einschließlich direkter und indirekter Kosten. 
- Kosten pro Einheit: Durchschnittliche Kosten, um eine Einheit der Produktion oder Dienstleistung zu erzeugen.

#### Flexibilität
- Anpassungsfähigkeit: Wie schnell und effizient kann das Modell an neue Anforderungen oder Daten angepasst werden?
- Skalierbarkeit: Die Fähigkeit des Prozesses, mit einer zunehmenden Menge von Daten oder Anforderungen effektiv umzugehen.

#### Zuverlässigkeit
- Verfügbarkeit: Prozentsatz der Zeit, in der das System verfügbar und funktionsfähig ist.
- Wiederherstellbarkeit: Die Fähigkeit des Systems, nach einem Ausfall wieder in einen betriebsfähigen Zustand zurückzukehren.

#### Compliance
- Einhalten von Vorschriften und Standards: Erfüllung relevanter rechtlicher und industrieller Standards (z.B. GDPR für Datenschutz). 
- Dokumentation und Auditierbarkeit: Qualität und Vollständigkeit der Prozessdokumentation zur Unterstützung von Audits. Auch relevante Datenquellen die in die Modelle eingeflossen sind müssen dokumentiert werden.

#### Zielerreichung
- Zielerreichungsgrad: Das Ausmaß, in dem das KI-Modell die festgelegten geschäftlichen oder technischen Ziele erfüllt.
- ROI (Return on Investment): Das Verhältnis von Nutzen oder Gewinn, der aus der Implementierung des KI-Modells resultiert, im Vergleich zu den Investitionskosten.

Beispiele für diese Methoden und Metriken sind stark vom Use Case abhängig. 


### Referenzen
| RefID | Verweis                                                                                                                                                      | Kurzbeschr.                                                                                                                                                         |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 34    |  ISO/IEC 25030:2019 - Systems and software engineering — Systems and software quality requirements and evaluation (SQuaRE) — Quality requirements framework  | Das Dokument bietet einen Rahmen zur Erfassung und Steuerung von Qualitätsanforderungen für Systeme, Software und Daten anhand der Modelle ISO/IEC 25010 und 25012. |
| 39    |  ISO/IEC TR 5469:2024 - Artificial intelligence — Functional safety and AI systems                                                                           | Die Dokument definiert Methoden und Prozesse zur Risikominimierung beim Einsatz KI-gestützter sicherheitsrelevanter Funktionen.                                     |

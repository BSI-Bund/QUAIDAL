---
Name: QM-65_AI_or_S_Bom
Title: QM-65 AI or S-Bom
TitleGer: QM-65 AI or S-Bom
shortdesc: Eine SBOM (Software Bill of Materials) und ihr KI-Pendant, der AIBOM, bieten eine umfassende und transparente Dokumentation aller Komponenten, Abhängigkeiten und Prozessinformationen – inklusive Sicherheitslücken, Versions- und Lizenzdetails sowie ethischer und Compliance-Aspekte – um potenzielle Risiken in der Software- bzw. KI-Lieferkette frühzeitig zu erkennen und zu mindern.
tags:
  - Qualitätsmetrik
ID:
  - QM-65
ListMetricID: 
ListMeasureID:
  - "'MA-20'"
  - "'MA-18'"
  - "'MA-22'"
MID: 
type:
  - method
share: true
CodeEx: false
lcstep: pre
---
## QM-65 SBoM / AIBoM / AI-S-BoM

### Beschreibung SBoM (Software Bill of Materials)

Eine SBOM stellt eine umfassende und detaillierte Inventarliste der Software dar, die sämtliche verwendete Komponenten – von Bibliotheken und Paketen bis hin zu Abhängigkeiten – systematisch erfasst. Neben Versionsnummern und Lizenzinformationen werden auch bekannte Sicherheitslücken aufgeführt. Zu den zusätzlichen Aspekten, die in einer vollständigen SBOM Berücksichtigung finden sollten, zählen:

- **Revisions- und Änderungsverlauf:** Dokumentation der Historie von Updates und Sicherheits-Patches, um nachvollziehbar zu machen, wie und wann Änderungen vorgenommen wurden.
    
- **Abhängigkeiten und Integrationspunkte:** Eine detaillierte Aufschlüsselung, inwiefern einzelne Softwarekomponenten miteinander interagieren und welche Drittanbieter-Komponenten eingebunden sind.
    
- **Automatisierte Aktualisierungs- und Validierungsprozesse:** Einsatz von Tools zur regelmäßigen Überprüfung der Komponenten auf Sicherheitslücken und Lizenzkonformität.
    
- **Compliance- und Audit-Informationen:** Nachweis, dass gesetzliche und branchenspezifische Vorgaben eingehalten werden, was insbesondere in kritischen Infrastrukturen eine zentrale Rolle spielt.
    

Der wesentliche Nutzen der SBOM liegt in der erhöhten Transparenz innerhalb der Softwarelieferkette, wodurch potenzielle Risiken – etwa durch veraltete Komponenten oder Lizenzverstöße – frühzeitig identifiziert und mitigiert werden können.


### Beschreibung AI-BoM (AI Bill of Materials)

Das Konzept des AIBOM überträgt und erweitert die Prinzipien der SBOM auf den Bereich der Künstlichen Intelligenz. Neben der Erfassung klassischer Softwarekomponenten wird hier der gesamte Lebenszyklus eines KI-Systems abgebildet, der sowohl Daten, Algorithmen als auch die Infrastruktur umfasst. Neben den bereits bekannten Bestandteilen sollten in einem AIBOM folgende Punkte aufgeführt werden:

- **Trainingsdaten:**
    - Herkunft der Daten
    - Lizenzierungsbedingungen
    - Dokumentation möglicher Verzerrungen (Bias) und Maßnahmen zur Bias-Reduktion
    - Qualitätssicherung und Validierungsprozesse

- **Modelldetails:**
    - Name, Version und Architektur des Modells
    - Hyperparameter und Konfigurationseinstellungen
    - Validierungsergebnisse und performancerelevante Kennzahlen

- **Entwicklungsprozess und Protokollierung:**
    - Detaillierte Aufzeichnungen zu Prompt-Protokollen, generiertem Code und verwendeten Optimierungsmethoden
    - Dokumentation des Trainings- und Testprozesses inkl. Benchmarks und Testszenarien

- **Technische Abhängigkeiten:**
    - Eingebundene Frameworks (wie TensorFlow, PyTorch oder andere spezialisierte Bibliotheken)
    - Versionsmanagement der unterstützenden Softwarekomponenten und Tools

- **Ethische Richtlinien und Sicherheitsüberprüfungen:**
    - Implementierte ethische Standards und Richtlinien zur Vermeidung von Diskriminierung oder unfairen Entscheidungen
    - Maßnahmen zur Überwachung von Sicherheitslücken in den zugrundeliegenden Modellen, inklusive Tests gegen potenzielle Manipulationen oder Angriffe

- **Transparenz und Nachvollziehbarkeit der Entscheidungsprozesse:**
    - Aufschlüsselung, wie und warum bestimmte Entscheidungen getroffen wurden
    - Modellinterpretierbarkeit und Erklärbarkeit, um Fehlfunktionen oder unvorhergesehene Verhaltensweisen frühzeitig zu erkennen

- **Regulatorische und Compliance-Aspekte:**
    - Sicherstellung der Einhaltung gesetzlicher Vorgaben und branchenspezifischer Standards
    - Dokumentation von Audit-Ergebnissen und Risikomanagement-Prozessen
        

Durch die Kombination von technischen, prozessualen und ethischen Informationen adressiert der AIBOM nicht nur die Funktionsweise des KI-Systems, sondern auch seine Auswirkungen auf die Gesellschaft sowie mögliche Angriffsflächen. Dies ermöglicht es, KI-spezifische Schwachstellen – wie Datenverzerrungen, fehlerhafte Entscheidungsfindungen oder gezielte Angriffe auf das Modell – frühzeitig zu erkennen und zu beheben.



### Referenzen

| RefID | Verweis                 | Kurzbeschr.                                                                                |
| ----- | ----------------------- | ------------------------------------------------------------------------------------------ |
| 226   |  aai-institute/AI-SBOM  | JSON Spec for Transparency Obligations of the EU AI Act, including LLM / foundation models |

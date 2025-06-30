---
Name: MA-02 Format Prüfung
Title: MA-02 Format Prüfung
TitleGer: MA-02 Format Prüfung
shortdesc: Inhalte mittels Formatierungsprüfung auf Korrektheit prüfen
sciencetopic: 
tags:
  - Qualitätsmaßnahme
  - validation
ID:
  - MA-02
ListMetricID: 
ListMeasureID:
  - "'QB-12'"
  - "'QB-13'"
  - "'QB-01'"
  - "'QB-08'"
  - "'QB-06'"
share: true
---
## MA-02 Format Prüfung

### Beschreibung

Diese Maßnahme stellt sicher, dass die vorgesehenen Datentypen wie Datum, Zeichenketten (Strings) und andere Datentypen genau im spezifizierten Format vorliegen. Da Daten oft in verschiedenen Formaten und Typen vorliegen können, beugt eine solche Überprüfung und Standardisierung, Fehlern in der Datenverarbeitung und der Missinterpretation der Daten vor. 

Beispielsweise können sich Datumsformate - je nach Anwendungsregion - stark unterscheiden:
- ISO-Format: JJJJ-MM-TT
- Amerikanisches Format: MM/TT/JJJJ
- Europäisches Format: TT.MM.JJJJ


### Beispiele 
#### Beispiel 1 - Datum 
Nehmen wir das Beispiel von Datumsfeldern, die in diversen Formaten existieren können. Drei der gängigsten Formate sind:

- **ISO (International Organization for Standardization) Format**, das in der Form JJJJ-MM-TT (Jahr-Monat-Tag) dargestellt wird. Dieses Format ist international anerkannt und wird vor allem in technischen und internationalen Kontexten bevorzugt, da es Missverständnisse vermeidet und eine einheitliche, leicht zu sortierende Struktur aufweist.

- **USA Format**, welches die Struktur MM/TT/JJJJ (Monat/Tag/Jahr) verwendet. Dieses Format ist in den Vereinigten Staaten üblich und unterscheidet sich von den meisten anderen Ländern, die in der Regel den Tag vor dem Monat angeben. Die Verwendung dieses Formats in einem internationalen Umfeld kann zu Verwechslungen führen, wenn es nicht klar gekennzeichnet oder standardisiert ist.

- **EUR (Europäisches) Format,** dargestellt als TT.MM.JJJJ (Tag.Monat.Jahr). Dieses Format ist in vielen europäischen Ländern standard und ähnelt dem ISO-Format, verwendet jedoch Punkte anstelle von Bindestrichen als Trennzeichen. Es spiegelt die traditionelle Art wider, in vielen europäischen Ländern das Datum anzugeben


#### Beispiel 2 - E-Mail Adressen

- Prüfen, ob der Wert des Attributs "E-Mail" ein '@' enthält


#### Beispiel 3 - Komplexes Beispiel -  Formatprüfung bei Telefonnummern in internationalen Systemen

In einem globalen System, das Telefonnummern von Nutzern aus verschiedenen Ländern speichert und verarbeitet, ist die Standardisierung und Formatprüfung essenziell, um eine konsistente und zuverlässige Nutzung der Telefonnummern zu gewährleisten. Telefonnummern unterscheiden sich stark zwischen Ländern hinsichtlich der Ländervorwahlen, Anzahl der Ziffern und der Formatierung (Leerzeichen, Bindestriche, Klammern etc.).

##### Herausforderung:

- Telefonnummern können in vielen verschiedenen Formaten eingegeben werden:
    
    - **Deutschland**: +49 151 23456789
    - **USA**: +1 (555) 123-4567
    - **Großbritannien**: +44 (20) 7946 0958
    - **Frankreich**: +33 (1) 23 45 67 89
    
    Es gibt Unterschiede in der Anzahl der Ziffern, der Nutzung von Leerzeichen, Bindestrichen, und anderen Sonderzeichen sowie der Strukturierung von Vorwahl und Rufnummer. Zudem nutzen viele Länder verschiedene Vorwahlsysteme und Längen von Telefonnummern.
    

##### Anforderungen an die Formatprüfung:

- **Internationale Vorwahl**: Die Nummer muss mit einem '+' gefolgt von der Landesvorwahl beginnen. Eine gängige Fehlermeldung könnte hier sein, wenn die Nummer nicht mit einem '+' beginnt oder eine ungültige Ländervorwahl verwendet wird.
    
- **Anzahl der Ziffern**: Die Rufnummer selbst (ohne Vorwahl) sollte eine festgelegte Länge haben, die je nach Land variiert. Zum Beispiel:
    
    - Deutsche Mobilnummern haben typischerweise 10 bis 11 Ziffern nach der Landesvorwahl.
    - In den USA haben Telefonnummern insgesamt 10 Ziffern (ohne Vorwahl), oft strukturiert als (NPA) NXX-XXXX. Eine Prüfung könnte sicherstellen, dass die Anzahl der Ziffern korrekt ist, je nachdem, welches Land durch die Vorwahl identifiziert wird.
- **Formatierung von Sonderzeichen**: Sonderzeichen wie Klammern, Leerzeichen, Bindestriche sind häufig optional und werden oft zur besseren Lesbarkeit verwendet. Das System sollte diese Zeichen entweder standardisieren (z. B. alle Leerzeichen entfernen) oder ihre Nutzung flexibel handhaben, ohne die Integrität der Nummer zu beeinflussen. Dennoch sollten unübliche oder fehlerhafte Zeichen, die zu Problemen bei der Validierung oder Verarbeitung führen könnten, erkannt und gemeldet werden (z. B. Buchstaben oder unübliche Sonderzeichen wie „%“, „&“).
- **Länderspezifische Besonderheiten**: Einige Länder haben besondere Regeln für Telefonnummern. In Indien müssen Mobilnummern zum Beispiel mit einer Ziffer zwischen 7 und 9 beginnen. In Frankreich mit einer 6 oder 7. In Großbritannien variiert die Anzahl der Ziffern in der Festnetznummer je nach Stadt.

### Metriken & Methoden

| ID                              | Kurzbeschr.                                                                               |
| ------------------------------- | ----------------------------------------------------------------------------------------- |
| QM-32 Reguläre Ausdrücke        |  Technik zur Mustererkennung und Textmanipulation                                         |
| QM-34 Validierung der Feldgröße | Textfelder und Variablen auf erwartete Länge überprüfen. Automatisiert/expertengesteuert. |
| QM-43 Kreuzabgleich             | Ergebnisprüfung durch Kreuzabgleich verschiedener Quellen.                                |



### Referenzen

| RefID | Verweis                                                                                                    | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----- | ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 31    |  ISO/IEC 24029-2:2023 - Robustness of neural networks – Part 2: Methodology for the use of formal methods  | Dieses Dokument beschreibt eine Methodik zur Auswahl, Anwendung und Verwaltung formaler Methoden zur Bewertung und zum Nachweis der Robustheitseigenschaften von neuronalen Netzen.                                                                                                                                                                                                                                         |
| 74    |  Imbalanced learning: foundations, algorithms, and applications                                            | Dieses Werk bietet die erste umfassende Übersicht über das Lernen mit unausgewogenen Datensätzen, ein zentrales Thema in Bereichen wie Überwachung, Sicherheit, Finanzen und biomedizinischen Systemen. Es vermittelt Einblicke in modernste Techniken, Prinzipien und Anwendungen und unterstützt Wissenschaftler und Ingenieure dabei, Herausforderungen zu bewältigen und zukünftige Forschungsperspektiven zu erkunden. |
| 173   |  OWASP - Development-time threats – AI Exchange                                                            | Die OWASP-Seite beschreibt Risiken während der Entwicklung von KI-Systemen, wie Datenvergiftung, geistigen Diebstahl und Supply-Chain-Angriffe. Sie empfiehlt Schutzmaßnahmen wie Verschlüsselung, Datenisolation und Integritätsprüfungen, um Modelle und Daten zu sichern.                                                                                                                                                |
| 229   |  Identifying Mislabeled Training Data                                                                      | Das Papier stellt einen Ansatz vor, der mithilfe von Lernalgorithmen falsch beschriftete Trainingsdaten identifiziert und entfernt, um die Klassifikationsgenauigkeit zu verbessern. Die Ergebnisse zeigen, dass Konsensfilter bei knappen Daten konservativ arbeiten, während Mehrheitsfilter bei großen Datenmengen effektiver schlechte Daten aussortieren.                                                              |


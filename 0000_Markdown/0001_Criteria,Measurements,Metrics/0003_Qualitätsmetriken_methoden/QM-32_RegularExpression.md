---
Name: QM-32 Reguläre Ausdrücke
Title: QM-32 Reguläre Ausdrücke
TitleGer: QM-32 Reguläre Ausdrücke
shortdesc: " Technik zur Mustererkennung und Textmanipulation"
tags:
  - Qualitätsmetrik
ID:
  - QM-32
ListMetricID: 
ListMeasureID:
  - "'MA-2'"
  - "'MA-1'"
  - "'MA-02'"
  - "'MA-01'"
MID: "41"
type:
  - method
lcstep: pre
CodeEx: true
share: true
---
## QM-32 Reguläre Ausdrücke

### Beschreibung

Reguläre Ausdrücke (RegEx) sind eine Technik zur Mustererkennung und Textmanipulation. Sie ermöglichen es mittels entsprechender Formatvorgaben nach Mustern in Texten zu suchen und bieten eine flexible Methode zur Erkennung, Validierung und Transformation von Daten.


### Beispiele 

#### Beispiel 1 - Ausdruck einfacher Komplexität

Suche nach einem spezifischen Wort: 
   - `RegEx`: `\bWort\b`
   - Beschreibung: Findet das exakte Wort „Wort“ als ganzes Wort im Text.

Ziffern finden:
   - `RegEx`: `\d`
   - Beschreibung: Findet jede einzelne Ziffer (0-9) im Text.


#### Beispiel 2 - Ausdruck mittlerer Komplexität

E-Mail-Adresse validieren (einfache Version):
   - `RegEx`: `[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}`
   - Beschreibung: Prüft, ob eine Zeichenfolge dem Format einer E-Mail-Adresse entspricht. Diese Version berücksichtigt Buchstaben, Ziffern, Punkte, Unterstriche, Prozentzeichen, Plus- und Minuszeichen vor dem @-Symbol; Domänennamen können Buchstaben und Ziffern enthalten.

Datum im Format DD/MM/YYYY validieren:
   - `RegEx`: `\b(0?[1-9]|[12][0-9]|3[01])[-/.](0?[1-9]|1[012])[-/.](19|20)?\d\d\b`
   - Beschreibung: Überprüft, ob eine Zeichenfolge einem Datum im Format DD/MM/YYYY, DD-MM-YYYY oder DD.MM.YYYY entspricht. Berücksichtigt Tage von 01 bis 31 und Monate von 01 bis 12. Jahre können vierstellig oder zweistellig sein und optional mit 19 oder 20 beginnen.

#### Beispiel 3 - Ausdruck hoher Komplexität

URL validieren:
- `RegEx`: `^(https?://)?(www\.)?[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}(/.*)?$`
- Beschreibung: Überprüft, ob eine Zeichenfolge dem Format einer URL entspricht. Akzeptiert optional „http://“ oder „https://“ und „www.“ am Anfang. Unterstützt Domänennamen mit Buchstaben, Ziffern, Punkten und Bindestrichen. Akzeptiert jegliche Art von Pfaden am Ende der URL.

Passwortvalidierung (stark):
- `RegEx`: `^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$`
- Beschreibung: Stellt sicher, dass das Passwort mindestens acht Zeichen lang ist und mindestens eine Kleinbuchstabe, eine Großbuchstabe, eine Ziffer und ein Sonderzeichen enthält. Diese Anforderungen machen es zu einem starken Passwort.

Komplexe E-Mail-Adresse validieren:
- `RegEx`: `^(?![_.-])(?!.*[_.-]{2})[a-zA-Z0-9._+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$`
- Beschreibung: Eine erweiterte Validierung für E-Mail-Adressen, die zusätzliche Bedingungen wie das Verbot aufeinanderfolgender Sonderzeichen und das Verbot von Sonderzeichen am Anfang implementiert.


### Pythoncode "RegularExpression"

| RefID | Verweis                        |
| ----- | ------------------------------ |
| 28    | QM-32_RegularExpression_python |


### Referenzen

| RefID | Verweis              | Kurzbeschr.                                                                                                                                                                                                                                                                                                 |
| ----- | -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 253   |  Regular expression  | Ein regulärer Ausdruck (regex) ist eine Folge von Zeichen, die ein Textvergleichsmuster definieren, das häufig bei der Suche, Textverarbeitung und Eingabevalidierung verwendet wird, seinen Ursprung in der formalen Sprachtheorie hat und durch Unix-Tools und Programmiersprachen populär gemacht wurde. |

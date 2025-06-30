---
Name: QM-58-3 Lokale differentielle Privatsphäre
Title: QM-58-3 Lokale differentielle Privatsphäre
TitleGer: QM-58-3 Lokale differentielle Privatsphäre
shortdesc: Methoden der differentiellen Privatsphäre, umgesetzt bereits beim Nutzer
tags:
  - Qualitätsmetrik
  - DifferentialPrivacy
ID:
  - QM-58-3
ListMetricID: 
ListMeasureID:
  - "'MA-25'"
MID: "101"
type:
  - method
lcstep: post
CodeEx: true
share: true
---
## QM-58-3 Lokale differentielle Privatsphäre

### Beschreibung
  
Die lokale differentielle Privatsphäre (Local Differential Privacy, LDP) ist eine Variante der differentiellen Privatsphäre, die den Datenschutz auf der Ebene des einzelnen Benutzers stärkt. Während differentielle Privatsphäre typischerweise in einer zentralisierten Umgebung angewendet wird, wo ein vertrauenswürdiger Server Daten sammelt und analysiert, bietet die lokale differentielle Privatsphäre einen Ansatz, bei dem die Daten schon auf dem Gerät des Benutzers anonymisiert werden, bevor sie überhaupt an einen Server weitergeleitet werden. 

### Methode

- Benutzerkontrolle: Bei LDP kontrolliert der Benutzer die Anonymisierung seiner Daten. Das bedeutet, dass die Daten bereits in einer anonymisierten Form gesammelt werden, was das Risiko von Datenschutzverletzungen durch den Datensammler oder durch einen Angriff auf den zentralen Server minimiert.
- Rauschen hinzufügen: Wie bei der herkömmlichen differentiellen Privatsphäre wird auch bei LDP Rauschen zu den Daten hinzugefügt, um zu verhindern, dass Rückschlüsse auf einzelne Personen gezogen werden können. Dies geschieht jedoch lokal auf dem Gerät des Benutzers.
- Analyse und Genauigkeit: Obwohl LDP einen stärkeren Schutz der Privatsphäre bietet, kann das Hinzufügen von Rauschen auf lokaler Ebene die Genauigkeit der aggregierten Daten beeinträchtigen. Die Herausforderung besteht darin, ein Gleichgewicht zwischen Datenschutz und Datenqualität zu finden.
- Anwendungsbereiche: Lokale differentielle Privatsphäre wird häufig in Umgebungen eingesetzt, in denen das Vertrauen in den zentralen Server begrenzt ist oder die rechtlichen und regulatorischen Anforderungen einen starken Schutz der individuellen Privatsphäre erfordern. Beispiele hierfür sind Telemetrie-Daten in Betriebssystemen oder Nutzungsstatistiken in mobilen Apps.

Die zentralen Vorgaben (z. B. ε, Mechanismus, Randomisierungsparameter) werden vom Datenkurator bzw. dem zentralen Aggregator (also z. B. der Organisation oder Firma, die die Daten sammelt) definiert und an die Clients kommuniziert. Die Clients führen die Konfiguration lokal aus, sind in ihrer Implementierung also typischerweise nicht autonom.

### Sourcecode "Lokale Differentielle Privatsphäre"
| RefID | Verweis                                         |
| ----- | ----------------------------------------------- |
| 81    | QM-58-3_LokaleDifferentiellePrivatsphäre_python |



### Referenzen
| RefID | Verweis                                               | Kurzbeschr.                                                                                                                                                                                                                        |
| ----- | ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 77    |  A Survey on Differentially Private Machine Learning  | Diese Arbeit untersucht Differential Privacy im maschinellen Lernen, konzentriert sich auf Methoden zur Rauschzugabe zu Modellen und Zielfunktionen zum Schutz der Privatsphäre und hebt zukünftige Forschungsschwerpunkte hervor. |



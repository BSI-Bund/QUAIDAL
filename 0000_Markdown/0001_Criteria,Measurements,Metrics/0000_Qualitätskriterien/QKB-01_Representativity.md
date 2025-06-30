---
Name: QKB-01_Representativity
Title: QKB-01 Representativity
TitleGer: QKB-01 Repräsentativität
shortdesc: Repräsentativität bezieht sich darauf, wie gut der Datensatz die Gesamtpopulation widerspiegelt, aus der er stammt.
tags:
  - Qualitätskriterien
ID:
  - QKB-01
ListMeasureID: 
ListCritID: 
share: true
---

## QKB-01 Repräsentativität

### Beschreibung 

Repräsentativität bezieht sich darauf, wie gut der Datensatz die Gesamtpopulation widerspiegelt, aus der er stammt. Um Repräsentativität innerhalb von Trainingsdaten sicherzustellen ist es zielführend diverse Aspekte zu beachten. Vielfalt gewährleistet, dass die Daten eine breite Palette von Permutationen abdecken und zur Generalisierung der Modelle beitragen. Ausgewogenheit stellt sicher, dass mögliche Inhalte innerhalb des Datensatzes nicht über- oder unterrepräsentiert werden. Um repräsentativ zu sein, muss auch die Größe des Datensatzes entsprechend gewählt werden. Ansonsten können systematische Fehler in den Modellen später zu sogenanntem Bias (Verzerrung) der Ergebnisse führen. 

Häufig werden Synonyme für "Repräsentativität" genutzt. Sie sind vielfältig und helfen, den Begriff aus unterschiedlichen Blickwinkeln zu betrachten. Wir bilden diese Begriffe wie "Abbildbarkeit" und "Repräsentationsqualität" als Bausteine des Hauptkriteriums ab.  "Ausgewogenheit" und "Vielfalt" fokussieren sich darauf, dass eine breite Palette von Merkmalen und Kategorien im Datensatz vorhanden ist, um eine faire und umfassende Repräsentation zu gewährleisten. "Verallgemeinerungsfähigkeit" und "Stichprobenqualität" beziehen sich auf die Eignung des Datensatzes, zuverlässige und genaue Vorhersagen für die gesamte Zielpopulation zu ermöglichen. 

Eine Abgrenzung kann gegen das Merkmal der "Gültigkeit" gemacht werden. Gültigkeit bezieht sich darauf, wie gut ein Datensatz tatsächlich das misst, was er messen soll. Repräsentativität hingegen bezieht sich darauf, wie gut er die Gesamtpopulation widerspiegelt, aus der er stammt. Das bedeutet: ein Datensatz kann valide sein (d.h. er misst genau das, was er messen soll), aber dennoch nicht repräsentativ (d.h. er spiegelt nicht die Gesamtpopulation wider). Umgekehrt kann ein repräsentativer Datensatz vorliegen, der jedoch nicht valide ist, wenn die Messungen oder Daten fehlerhaft oder irrelevant sind.

### Beispiel

Es soll ein maschinelles Lernmodell trainiert werden, um die Kreditwürdigkeit von Personen vorherzusagen. Der Zielmarkt für dieses Modell sind Kreditnehmer mit unterschiedlicher Demographie, Einkommensverteilung, Beschäftigungsarten und Kreditgeschichte. Um die Repräsentativität zu gewährleisten, müssen die Trainingsdaten eine breite und faire Stichprobe der gesamten Bevölkerung enthalten. Das bedeutet, dass der Datensatz Kreditnehmer aus verschiedenen Altersgruppen, Einkommensschichten, geografischen Regionen, Bildungsniveaus und Geschlechtern umfassen sollte.


### Bausteine

| Baustein              | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                          |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| QB-03_Diversity       | Vielfalt deckt die Verschiedenartigkeit und das Variationspotential von Werten ab.                                                                                                                                                                                                                                                                                   |
| QB-04_Balance         | Ausgewogenheit sichert gleichmäßige Verteilung, Vielfalt maximiert Varianz.                                                                                                                                                                                                                                                                                          |
| QB-05_Size            | Größere Datensätze verbessern Modellgenauigkeit, Robustheit und reduzieren Overfitting.                                                                                                                                                                                                                                                                              |
| QB-06 Bias-Detektion  | Unausgewogene Verteilung führt zu systematischen Verzerrungen in Modellvorhersagen.                                                                                                                                                                                                                                                                                  |
| QB-15_Bias-Mitigation | Der Baustein beschreibt technische Verfahren zur Reduzierung von Verzerrungen in KI-Modellen, die idealerweise bereits bei der Datenerhebung ansetzen und sich je nach Zeitpunkt ihres Einsatzes im Entwicklungszyklus in Präprozessierungs-, Inprozessierungs- und Postprozessierungsmethoden gliedern, wie anhand eines Bewerbungs-Beispiels veranschaulicht wird. |



### Referenzen

| RefID | Verweis                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Kurzbeschr.                                                                                                                                                                                                                                                                            |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 296   |  Bias in der künstlichen Intelligenz                                                                                                                                                                                                                                                                                                                                                                                                                            | Das Dokument Bias in der künstlichen Intelligenz befasst sich mit den Grundlagen und zeigt Detektion und Mitigationsmechanismen auf um Bias in den eigenen Datensätzen auf die Spur zu kommen.                                                                                         |
| 260   |  AI-Act - Verordnung (EU) 2024/1689 des Europäischen Parlaments und des Rates vom 13. Juni 2024 zur Festlegung harmonisierter Vorschriften für künstliche Intelligenz und zur Änderung der Verordnungen (EG) Nr. 300/2008, (EU) Nr. 167/2013, (EU) Nr. 168/2013, (EU) 2018/858, (EU) 2018/1139 und (EU) 2019/2144 sowie der Richtlinien 2014/90/EU, (EU) 2016/797 und (EU) 2020/1828 (Verordnung über künstliche Intelligenz) (Text von Bedeutung für den EWR)  | Der AI Act reguliert KI-Systeme nach Risikostufen, fordert für hochriskante Anwendungen strenge Vorgaben und setzt auf Transparenz und Menschenrechtsschutz. Artikel 10 verlangt qualitativ hochwertige, dokumentierte Datensätze, um faire und vertrauenswürdige KI zu gewährleisten. |
| 33    |  ISO/IEC 25012:2008 - Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model                                                                                                                                                                                                                                                                                                                                 | Softwareentwicklung – Qualitätsanforderungen und Bewertung von Softwareprodukten (SQuaRE) – Datenqualitätsmodell                                                                                                                                                                       |

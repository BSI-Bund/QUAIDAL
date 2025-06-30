---
Name: QM-44-9_Diffusion Imputation/Augmentation
Title: QM-44-9 Diffusion Imputation/Augmentation
TitleGer: QM-44-9 Diffusion Imputation/Augmentation
shortdesc: Daten Imputation mittels stochastischer Rauschprozesse
tags:
  - Qualitätsmetrik
ID:
  - QM-44-9
ListMetricID: 
ListMeasureID:
  - "'MA-16'"
MID: 
type:
  - metrik
lcstep: pre
CodeEx: false
share: true
---
## QM-44-9 Diffusion-Imputation

### Beschreibung

Daten-Imputation mittels Diffusionsmethoden nutzt die Prinzipien von Diffusionsprozessen, um fehlende Daten in Datensätzen plausibel zu rekonstruieren oder zu ergänzen. Dabei wird ein stochastischer Rauschprozess modelliert, der den zugrundeliegenden Datenraum erfasst und schrittweise die fehlenden Werte ergänzt. Durch das Lernen der komplexen Datenverteilung können Diffusionsmodelle fehlende Informationen realistisch im Kontext der vorhandenen Daten ergänzen, was zu einer verbesserten Datenqualität und robusteren Vorhersagemodellen führt.


### Beispiele 

#### Beispiel 1 - Bildimputation (Inpainting)  

In der Bildverarbeitung werden Diffusionsmodelle genutzt, um fehlende oder beschädigte Bildbereiche zu rekonstruieren. Ein Diffusionsmodell lernt dabei die zugrundeliegende Verteilung vollständiger Bilder. Wird ein Bild mit fehlenden Regionen (z. B. durch Rauschen oder Beschädigung) vorgelegt, kann das Modell schrittweise plausible Inhalte generieren, die nahtlos in den vorhandenen Kontext passen. Dies findet Anwendung bei der Restaurierung alter Fotografien oder in kreativen Bildbearbeitungsprozessen.

#### Beispiel 2 - Imputation tabellarischer Daten

Tabellarische Datensätze enthalten häufig fehlende Werte in einzelnen Merkmalen, etwa in medizinischen oder finanziellen Daten. Ein Diffusionsmodell kann hier die gemeinsame Verteilung der Features lernen und dadurch fehlende Werte auf Basis der beobachteten Daten plausibel ergänzen. Beispielsweise kann in einem medizinischen Datensatz, in dem bestimmte Laborwerte fehlen, das Modell diese Lücken im Kontext anderer Gesundheitsdaten füllen und somit zu einer verbesserten Datenqualität und robusteren Vorhersagemodellen beitragen.

### Referenzen

| RefID | Verweis                                             | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----- | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 275   |  Effective Data Augmentation With Diffusion Models  | Anstatt nur einfache Transformationen wie Drehungen oder Spiegelungen zu verwenden – die keine semantische Vielfalt erzeugen – wird ein Verfahren vorgestellt, das vortrainierte Text-zu-Bild-Diffusionsmodelle nutzt. Damit lassen sich Bilder so bearbeiten, dass sich ihre inhaltlichen Eigenschaften (z.B. Tierarten) verändern. Das Verfahren generalisiert bereits mit wenigen gelabelten Beispielen und führt in Aufgaben wie Few-Shot-Bildklassifikation und in der Unkrauterkennung zu verbesserten Ergebnissen. |

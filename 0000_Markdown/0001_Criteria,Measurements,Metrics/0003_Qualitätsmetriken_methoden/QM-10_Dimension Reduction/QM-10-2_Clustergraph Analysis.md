---
Name: QM-10-2_Clustergraph Analysis
Title: QM-10-2_Clustergraph Analysis
TitleGer: QM-10-2_Clustergraph AnalysisQM-10-2 Clustergraph Analysis
shortdesc: Ein Verfahren zur Darstellung globaler Beziehungen zwischen Datenclustern
tags:
  - Qualitätsmetrik
  - "#ML-DimRed"
  - ML-DimRed
ID:
  - QM-10-2
ListMetricID: 
ListMeasureID:
  - "'MA-14'"
  - "'MA-16'"
  - "'MA-23'"
MID: 
type:
  - metrik
  - method
share: true
CodeEx: true
lcstep: pre
---
## QM-10-2 ClusterGraph Analysis

### Beschreibung

Das Paper "ClusterGraph: a new tool for visualization and compression of multidimensional data" stellt das Konzept des ClusterGraphen vor, eine Methode zur Visualisierung und Komprimierung hochdimensionaler Daten. Der ClusterGraph kombiniert Clustering-Techniken und Topologische Datenanalyse (TDA), um die globale Struktur und die relativen Abstände zwischen Clustern zu bewahren, was in konventionellen dimensionalen Reduktionsverfahren oft verloren geht.


### Beispiele 

#### Beispiel 1 - Handwritten Digits

Ein einfaches Beispiel für die Anwendung des ClusterGraph-Verfahrens stammt aus dem Bereich der optischen Zeichenerkennung. In einem solchen Szenario könnten handgeschriebene Ziffern analysiert werden, ähnlich wie es im Dokument mit dem Datensatz "Handwritten Digits" beschrieben wird​

**Daten**: Ein Datensatz von handgeschriebenen Ziffern, z. B. Bilder von 0 bis 9.


**ClusterGraph**: Aufbau eines ClusterGraphen, bei dem jeder Cluster ein Knoten ist und die Kanten die durchschnittlichen Abstände zwischen den Clustern darstellen.

**Visualisierung**: Durch das Entfernen redundanter Kanten (Pruning) kann eine übersichtliche Darstellung der Cluster-Beziehungen erstellt werden. Zum Beispiel könnte der Abstand zwischen Ziffern wie 1 und 7 kleiner sein als zwischen 1 und 8, was im Graph visualisiert wird.

Dieses Beispiel zeigt, wie ClusterGraph eingesetzt werden kann, um die globalen Beziehungen zwischen Clustern zu visualisieren, während lokale Details durch Clustering erhalten bleiben.

#### Beispiel 2 - Konzentrische Kreise

**Daten**: Ein Datensatz bestehend aus 500 Punkten, die aus zwei konzentrischen Kreisen im zweidimensionalen Raum entnommen sind.

**Clustering**: Die Punkte werden mithilfe des k-Means-Algorithmus in 20 Cluster aufgeteilt. Jeder Cluster repräsentiert eine Teilmenge der Punkte, die eng beieinander liegen.

**ClusterGraph-Konstruktion**:
    Auf Basis der Cluster wird ein ClusterGraph erstellt, bei dem jeder Cluster ein Knoten ist.
    Die Kanten des Graphen repräsentieren die mittleren Abstände zwischen den Clustern.
    
**Intrinsische Distanzen**:
    Ein 10-Nächste-Nachbarn-Graph wird konstruiert, um die intrinsischen Distanzen zwischen den Punkten zu schätzen. Diese Distanzen spiegeln die tatsächlichen Verhältnisse innerhalb der Kreise wider.
    
**Pruning des ClusterGraphen**:
    Mittels der _metric distortion_-basierten Pruning-Methode werden Kanten entfernt, die die globale Struktur des Datensatzes nicht korrekt repräsentieren.
    Das Ergebnis ist ein pruned ClusterGraph, der zwei klar getrennte Komponenten zeigt, die den beiden Kreisen entsprechen.
    
**Komponenten-Merging**:
    Da der ursprüngliche Datensatz aus zwei getrennten Kreisen besteht, führt das Pruning zu zwei separaten Komponenten.
    Um die Verbindung zwischen den Komponenten zu visualisieren, werden zusätzliche Kanten zwischen den nächstgelegenen Knoten der beiden Komponenten hinzugefügt.
    Danach werden diese Kanten mit einem konnektivitätsbasierten Ansatz weiter vereinfacht.


### Referenzen

| RefID | Verweis                                                                               | Kurzbeschr.                                                                                                                                                                                                                                                                                                                                                                                |
| ----- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 224   |  ClusterGraph: a new tool for visualization and compression of multidimensional data  | Herkömmliche Methoden zur Analyse hochdimensionaler Daten wie Dimensionsreduktion und Clustering bewahren zwar lokale Strukturen, erfassen jedoch oft nicht die globale Datenorganisation. Das Paper stellt den ClusterGraph vor, eine datenstrukturierte Ergänzung, die die globale Anordnung von Clustern bewahrt und eine qualitativ hochwertige Visualisierung und Analyse ermöglicht. |

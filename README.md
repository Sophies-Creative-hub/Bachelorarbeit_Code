# Bachelorarbeit_Code

## Inhaltsübersicht des Repositories

Dieses Repository dient als praktische Ergänzung zur Bachelorarbeit und demonstriert die Implementierung verschiedener Konzepte und Werkzeuge im Bereich neuromorpher Architekturen und Spiking Neural Networks (SNNs).

Die Codebasis ist hauptsächlich strukturiert nach den Experimenten, die in **Kapitel 4 ("Werkzeuge zur Simulation und Modellierung von Spiking Neural Networks")** der Arbeit durchgeführt wurden.

### Kerninhalte und Experimente:

2.  **Funktionsweise von SNNs mit Norse und PyTorch:**
    *   Implementierung eines neuronalen Modells zur Klassifizierung des **Fashion-MNIST Datensatzes**.
    *   Untersuchung verschiedener Eingabe-Encoder:
        *   `ConstantCurrentLIFEncoder`
        *   `PoissonEncoder`
        *   `SpikeLatencyLIFEncoder`
    *   Analyse der Trainingsdynamik, Genauigkeit und des Verlusts 

3.  **N-MNIST: Ein neuromorpher Datensatz für SNNs:**
    *   Verarbeitung und Klassifizierung des ereignisbasierten N-MNIST Datensatzes.
    *   Implementierungen mit:
        *   **Norse** 
        *   **Intel Lava** 
    *   Nutzung der `tonic` Bibliothek zur Handhabung des N-MNIST Datensatzes.


4.  **STDP praktisch implementiert:**
    *   Demonstration der Spike-Timing-Dependent Plasticity (STDP) in einem einfachen Neuronenmodell.
    *   Visualisierung der Gewichtsänderungen und des Lernfensters (siehe Abbildungen 4.19 bis 4.27).
    *   Implementierung mit grundlegenden Python-Bibliotheken und ggf. spezifischen Lava-Komponenten für Loihi-Lernregeln.


---

## Verwendete Technologien und Frameworks

*   **Norse:** Eine Deep-Learning-Bibliothek für SNNs, die auf PyTorch aufbaut.
*   **PyTorch:** Als Backend für Norse und für die Implementierung von Trainingsschleifen.
*   **Intel Lava:** Ein Open-Source-Software-Framework für neuromorphes Computing, insbesondere für Experimente, die auf Intel Loihi Hardware abzielen.
*   **Tonic:** Zur einfachen Handhabung und Transformation von neuromorphen Datensätzen.
*   Standardbibliotheken: NumPy, Matplotlib, h5py, etc.



## Bezug zur Bachelorarbeit

Der Code in diesem Repository dient der Veranschaulichung und Reproduzierbarkeit der im praktischen Teil der Bachelorarbeit durchgeführten Experimente. Er ermöglicht ein tiefergehendes Verständnis der diskutierten Konzepte, Herausforderungen und Implementierungsdetails von neuromorphen Systemen und SNNs.


# Tensor Field Dynamics (TFD)

## Über diese Organisation
In dieser Umgebung werden hochleistungsfähige, GPU-beschleunigte Pipelines für Computational Art und die Simulation dynamischer Systeme entwickelt. Der Fokus wird primär auf die Visualisierung komplexer topologischer Strukturen (wie Strange Attractors) und die numerische Integration deterministisch-chaotischer Differentialgleichungen gelegt.

## Architektur-Standards
Für sämtliche Projekte wird eine strikte Modularisierung zwischen mathematischer Berechnungsebene, Rendering-Pipeline und Benutzeroberfläche vorausgesetzt:

*   **Core Engine:** Die Integration der Vektorfelder wird nativ über vektorisierte PyTorch-Tensoren durchgeführt. Um den VRAM-Durchsatz zu maximieren, werden CPU-basierte Schleifenarchitekturen vollständig vermieden.
*   **Render Pipeline:** Für die visuelle Ausgabe wird auf fortgeschrittene Post-Processing-Techniken zurückgegriffen. Dies umfasst Volumetric Shading, SSAA (Supersampling Anti-Aliasing) sowie filmisches ACES-Tone-Mapping, um Renderings zu erzeugen, die professionellen Standards für hochauflösende Kunstdrucke genügen.
*   **Deployment:** Interaktive Schnittstellen zur Parametersteuerung und Echtzeit-Auswertung werden als modulare Streamlit-Applikationen implementiert.

## Technologie-Stack
*   PyTorch (CUDA-optimiert)
*   NumPy / Pandas
*   Streamlit
*   Python 3.13+

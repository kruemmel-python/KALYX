# KGENOME_REPORT v2 Kontrollprotokoll

Dieser Report verwendet nur vorhandene KGLIB/KGENOME-Artefakte und berechnet keine Sequenz neu.

## Aktive Diagnose

- Matrixweite Self-vs-Cross-Profile.
- Lift-/Accuracy-/Surprise-Verteilungen.
- Gerichtete Asymmetrieanalyse.
- Label-Sampling über vorhandene Matrixwerte.

## Wichtige Grenze

Label-Sampling ist kein echtes Sequenz-Nullmodell. Es prüft Report- und Matrixstruktur, aber nicht, ob die KDNA/KGRAM-Struktur durch Symbolreihenfolge entsteht.

## Noch zu berechnende echte Nullmodelle

- Symbol-Shuffle der KDNA-Ströme.
- Block-Shuffle.
- Train/Test-Rotation.
- k-Sweep, z. B. k=12/k=16/k=20.

# KGENOME Enterprise Report v2

Quelle: vorhandene KGLIB/KGENOME-Artefakte. Keine FASTA-, KMAP-, KGRAM- oder Matrix-Neuberechnung.

## Gesamtstatus

- Matrixzellen: 576
- Self-Zellen: 24
- Cross-Zellen: 552
- Durchschnitt Self-Lift: 0.991483175090255
- Durchschnitt Cross-Lift: 0.991332598414977
- Durchschnitt Self-Accuracy: 0.992731581855858
- Durchschnitt Cross-Accuracy: 0.99258100518058

## Wissenschaftliche Grenze

Dieser v2-Report ist eine Diagnose der vorhandenen Matrix. Die Label-Permutation ist kein echtes Sequenz-Nullmodell. Echte Nullmodelle erfordern Symbol-Shuffle, Block-Shuffle, Train/Test-Rotation oder k-Sweep mit neuen abgeleiteten Artefakten.

## Stärkste Kopplung

- chr4 -> chr2
- lift: 0.997719291154194
- accuracy: 0.998843580783331
- surprise: 0.001156419216669

## Schwächste Kopplung

- chr22 -> chrY
- lift: 0.95116123413596
- accuracy: 0.952798062806586
- surprise: 0.047201937193414

## Wichtigste Tabellen

- tables/global_metrics.csv
- tables/self_cross_profile.csv
- tables/grammar_carriers_v2.csv
- tables/chromosome_receivers_v2.csv
- tables/asymmetry_v2.csv
- controls/control_summary.csv
- controls/CONTROL_PROTOCOL.md

## Abbildungen

- figures/cross_lift_distribution.svg
- figures/self_lift_distribution.svg
- figures/asymmetry_distribution.svg
- figures/self_vs_cross_scatter.svg

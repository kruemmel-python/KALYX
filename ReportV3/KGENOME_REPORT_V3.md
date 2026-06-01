# KGENOME_REPORT v3 — echte Nullmodell-Berechnung

Dieser Report nutzt vorhandene KDNA-Streams und vorhandene KGRAM01-Grammatiken. FASTA, KMAP, KDNA und KGRAM werden nicht neu erzeugt.

## Aktive Nullmodelle

- **symbol_shuffle**: from/to werden unabhängig aus dem Testbereich des KDNA-Stroms gezogen. Lokale Reihenfolge wird zerstört, marginale Symbolverteilung bleibt erhalten.
- **rotation**: to wird mit festem Offset aus demselben Teststrom gelesen. Direkte Adjazenz wird zerstört, Feldverteilung bleibt erhalten.
- **block_boundary**: Übergänge werden aus künstlichen Blockgrenzen erzeugt. Lokale Blöcke bleiben als Reservoir erhalten, echte Nachbarschaftsgrenzen werden ersetzt.

## Nullmodell-Zusammenfassung

| mode | cells | avg observed acc | avg null acc | avg delta | max null acc | min delta |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| symbol_shuffle | 576 | 0.992587279209 | 0.000230373264 | 0.992356905945 | 0.00035 | 0.952543062807 |
| rotation | 576 | 0.992587279209 | 0.000263541667 | 0.992323737542 | 0.00058 | 0.952483062807 |
| block_boundary | 576 | 0.992587279209 | 0.000381710069 | 0.992205569139 | 0.000855 | 0.952218062807 |

## Interpretation

Wenn vg_delta_accuracy deutlich positiv bleibt, hängt die beobachtete KGRAM-Kopplung nicht nur an der marginalen Häufigkeit der KDNA-Symbole, sondern an der Übergangsordnung.

## Artefakte

- controls/null_summary.csv
- tables/null_joined.csv
- tables/top_observed_minus_null.csv
- tables/lowest_observed_minus_null.csv
- tables/top_null_accuracy.csv
- report_v3_manifest.json

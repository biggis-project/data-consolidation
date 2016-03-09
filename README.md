# data-consolidation
Consolidation of data sources based on semantic technologies

```
Kontakt
Hannes Müller
hannes.mueller@lubw.bwl.de
h.mueller.geo@gmail.com
```

## XML Files
- Messstationsnamen im Filenamen Codiert 
- Station 4444 Karlsruhe Nordwest (4444_mw1.xml) 
- Station 76447 Karsruhe Mitte Meteo (76447_mw1.xml)
- 10min Takt von der Messnetzzentrale auf den SFTP-Server geschickt. Dort wird die ältere Datei überschrieben

Short legend:
- T-Luft (Lufttemp [°C])
- P-Luft (Luftdruck [hPA])
- Nsch (Niederschlag [mm])
- WIV_1 (windgeschwindigkeit [m/s])
- WIR_1 (Windrichtung 0-360°)
- STRG_1 (Globalstrahlung W/m²)
- RLF_1 (rel. Feuchte [%], DP=Taupunkt)

## LUPO Database
- [REST Schnittstelle zur LUPO Datenbank](http://www.umwelt-bw.de/aktuelle-messwerte)
- Nur aktuelle Werte abrufbar (3 stunden Takt), d.h. keine Zeitreihe abrufbar.
- Im JASONP Format oder GME

Dokumentation see the following examples:
- [Example #1 query with GME output](https://1-dot-lupo-messwerte.appspot.com/lupo_luft_query?land=bw&limit=999&format=gme&callback=abc)
- [Example #2 query with JSON output](https://1-dot-lupo-messwerte.appspot.com/lupo_luft_query?land=bw&limit=999&format=jasonp)

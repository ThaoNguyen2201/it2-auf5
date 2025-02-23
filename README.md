# it2-auf5
Erstellen eines Dashboards und Verarbeitung von Server-Daten zum Tracking von Temperatur, Vibration und Akustik.

# Generelle Anforderungen
**Visualisierung** (s.a. VL1 S.40)
- Die **"Funktionalität"** muss für alle in der Aufgabenbeschreibung genannten Anforderungen gegeben sein (s.u. "**_Aufgabenbeschreibung_**")
- Die **"Ergonomie"** muss auf die Verwendung auf einem **_Tablet mit Touch-Funktionalität_** ausgerichtet sein
- Die **"Ästhetik / das Layout"** des Programms muss sich an der Corporate Identity des **_PID4CPS Ressourcen Cockpit_** (s.a.VL1 S.37) orientieren
  - Schriftart:
    - Roboto
  - Farbcodes:
    - Farbe Hintergrund: 717e87
    - Farbe Action bar: 314151
    - Farbe Timer: 217446
    - Farbe Eskalation: d24525
  - Icons:
    - <https://www.flaticon.com/authors/vectors-market>

## Thema: Aufgabe 5: Elektromotorenprüfstand 1: Condition Monitoring / Zuordnung von Fehlern

### (_AUFGABENBESCHREIBUNG_) Funktionalitäten des Programms:
**Tracking Schmiermittelverbrauch – Temperatur (Qualität/Leck)**
- Visualisierung der Temperatur und des Temperaturverlaufs der Wellenkupplung inklusive Toleranz- und Schadensgrenze
- Faktenbasierte, datengetriebene Ableitung von Qualitätsgegebenheiten und Fehlerzuständen

**Tracking Kugellagerlauf – Vibration und Akustik (Verschleiß/Bruch)**
- Visualisierung der Bewegung der Wellen und der von dieser ausgehenden Akustik sowie der Wertverläufe inklusive Toleranz- und Schadensgrenze
- Faktenbasierte, datengetriebene Ableitung von Verschleiß und Fehlerzuständen

**Tracking Anlageninnenleben – Vibration und Akustik (gelöste/vergessenen Teile)**
- Visualisierung der Bewegung der Welle und der von dieser ausgehenden Akustik sowie der Wertverläufe
- Faktenbasierte, datengetriebene Ableitung von Fehlerzuständen

## Nötige Entpunkte und relevante Daten
- <http://it2wi1.if-lab.de/rest/mpr_fall1> (Optimale Qualität)
- <http://it2wi1.if-lab.de/rest/mpr_fall2> (Mindere Qualität)
- <http://it2wi1.if-lab.de/rest/mpr_fall3> (Defekt)
- <http://it2wi1.if-lab.de/rest/mpr_fall4> (Lose Teile)
- Toleranzgrenze_temp: 75; Schadensgrenze_temp: 150
- Toleranzgrenze_laut: 80; Schadengrenze_laut: 117
- Toleranzgrenze_vibr: 0,15; Schadengrenze_vibr: 0,4
- Fall 4: Indiz für loses Teil (Abweichung letzte 5 Sec. >): Temp: 6, Vibr: 0,02

## Kontext der Aufgabenstellung
- Dashboard-Entwicklung:
  - Visualisierung von Live-Daten
  - Kontextualisierung (also in Bezug zu dem ganzen setzen)
  - Ableiten von Kausalitäten und Schlüssen (**ggf. Fehlermeldungen anzeigen oder direkt auf die Maschinen reagieren?**)

## Wichtig:
Bei diesen Funktionalitäten handelt es sich um die **Minimalanforderungen**. Sie sind dazu eingeladen, **_weitere Funktionen_**, basierend auf den zur Verfügung gestellten Daten, zu entwerfen und diese mit uns zu diskutieren. Auch können weitere Daten auf dem Server zur Verfügung gestellt werden, wenn Sie diese für bestimmte Funktionalitäten benötigen.

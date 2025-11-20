# 04 – Energie (Energy System)

Dieses Modul beschreibt das komplette Energiesystem von **Tina Village** –
einer Siedlung für ca. 2'000 Menschen.  
Das Ziel ist ein langlebiges, reparierbares und hoch effizientes System,
das durch lokale Ressourcen (Holz, Sonne) weitgehend selbst Versorgungsstärke
erreicht.

Das Energiesystem ist in fünf Hauptbereiche gegliedert:

1. Holz-KWK (Kraft-Wärme-Kopplung)
2. Photovoltaik & lokale Energieerzeugung
3. Batteriespeicher
4. Nahwärmenetz
5. Steuerung & Monitoring

---

# 🌲 1. Holz-KWK (Holz-Kraft-Wärme-Kopplung)

Das Kernstück der Energieversorgung ist das **Holz-KWK-Zentrum**.

### 1.1 Rohstoff
- Holz aus 9 km² Wald
- nachhaltige Forstwirtschaft
- Holzhackschnitzel (Chip-Qualität A1)

### 1.2 Funktion
Holz-KWK erzeugt gleichzeitig:

- **Elektrizität**  
- **Heizwärme** (für Gebäude, Kantinen, Schule, Industrie)

### 1.3 Vorteile
- hoher Gesamtwirkungsgrad (bis 85 %)
- nutzbare Abwärme für Warmwasser & Heizung
- regionaler Brennstoff, kein Abhängigkeit von externen Märkten
- Kostenstabilität über Jahrzehnte
- leicht reparierbare Technik

### 1.4 Leistung
(Platzhalter – genaue Berechnung später)

- elektrische Leistung: 300–600 kW  
- thermische Leistung: 1–2 MW  

### 1.5 Wartung
- tägliche visuelle Kontrolle  
- wöchentlicher Ascheentnahme  
- jährliche Inspektion  
- Ersatzteile lokal lagerbar

---

# ☀️ 2. Photovoltaik

PV-Anlagen befinden sich:

- auf Gemeinschaftsgebäuden  
- auf Industriehallen  
- optional auf Wohngebäuden (wenn sinnvoll)

### 2.1 Prinzipien
- nur gut zugängliche Module (leichte Wartung)
- Standard-Schnittstellen (MC4)
- Ersatzpaneele jederzeit ersetzbar
- keine proprietären Wechselrichter

### 2.2 Ziel
PV liefert am Tag:

- Strom für Häuser  
- Strom für Batterien  
- Überschuss für Eigenverbrauch

---

# 🔋 3. Batteriespeicher

Das Dorf verwendet mehrere **modulare Batterieschränke**, keine einzigen Großspeicher.

### 3.1 Gründe für modulare Speicher
- leicht austauschbar  
- geringere Brandlast  
- bessere Reparierbarkeit  
- Skalierbarkeit  
- keine Abhängigkeit von einem kritischen Teilpunkt  

### 3.2 Typen
- LFP (Lithium-Eisenphosphat), bevorzugt  
- optional Second-Life-Batterien

### 3.3 Funktion
- Tagesglättung (Peak Shaving)  
- Kurzzeitpuffer während Lastspitzen  
- Unterstützung der PV-Nutzung

---

# 🔥 4. Nahwärmenetz (Heating Grid)

Alle Gebäude sind an ein **Vorlauf/Rücklauf-Nahwärmenetz** angeschlossen.

### 4.1 Vorteile
- kein Einzelheizen  
- geringere Gesamtkosten  
- keine privaten Installationen notwendig  
- einfache Wartung  
- sehr hohe Effizienz

### 4.2 Aufbau
- Haupttrassen aus dem Energiezentrum
- Abzweige zu Wohnclustern
- isolierte Stahlrohre (PUR/PIR)
- Übergabestationen in jedem Gebäude

### 4.3 Gebäudeübergabe
- kompakter Wärmeübergabekasten  
- Warmwasser + Raumwärme  
- Temperatur- und Verbrauchssensoren

---

# 🧠 5. Steuerung & Monitoring

### 5.1 Zentrale Energie-Software
- optimiert Lasten  
- prognostiziert Verbrauch  
- steuert Speicher  
- priorisiert Wärme und Strom intelligent  
- zeigt in der Siedlungs-App den Verbrauch an

### 5.2 Sensoren
- Wärmefluss  
- Stromfluss  
- Holzverbrauch  
- Temperatur  
- Netzspannung  
- Druck im Heiznetz

### 5.3 Notfallkonzept
- Ersatzbrenner  
- Notstromgenerator  
- definierte Lastabwurfzonen  
- manueller Betrieb möglich

---

# 🔧 6. Reparierbarkeit & Ersatzteile

Ein Kernziel des Dorfes: **Reparieren statt Wegwerfen**.

### 6.1 Ersatzteilstrategie
- Standardisierte Pumpen
- genormte Rohre
- universelle Ventile
- gängige Wechselrichter
- lokale Produktion von Metall- und Holzkomponenten

### 6.2 Dokumentation
Jedes Modul erhält:
- Schaltpläne  
- Wartungsanleitungen  
- Ersatzteilnummern  
- Open-Source-Dokumentation  

---

# 🔄 7. Zusammenspiel mit anderen Modulen

Das Energiesystem interagiert direkt mit:

- `03_infrastructure` (Wärme- und Stromtrassen)  
- `05_water` (Wasserpumpen, Temperaturen, Energiebedarf)  
- `08_industry` (Energieintensive Werkstätten)  
- `10_it` (Monitoring, App, Steuerung)  
- `12_finance` (Investition & laufende Kosten)  

---

# 📥 8. Mitarbeit

Du hast Know-how zu:

- KWK  
- Solar  
- Batteriespeicher  
- Wärmeverteilung  
- Pumpensystemen  
- Energiemonitoring  
- thermischer Simulation  

Dann bist du explizit eingeladen, zu diesem Modul beizutragen.

Bitte lege ein Issue an oder mache einen Pull Request.

---

# 🎯 Ziel dieses Moduls

Ein voll dokumentiertes, vollständiges, replizierbares Energiesystem,
das:

- langlebig  
- reparierbar  
- stabil  
- regional versorgt  
- digital steuerbar  
- offen dokumentiert  

ist – und damit weltweit von anderen Gemeinschaften genutzt werden kann.


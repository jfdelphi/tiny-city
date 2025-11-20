# 02 – Gebäude (Buildings)

Dieses Kapitel beschreibt alle Gebäudearten des Open-Source-Dorfprojekts
**Tina Village**.  
Jeder Gebäudetyp ist modular, reparierbar, aus lokalem Holz baubar und
so konzipiert, dass möglichst viele Teile im Dorf selbst produziert
werden können.

Ziel dieses Moduls:
- klare Standardisierung
- einfache Reproduzierbarkeit
- minimale technische Komplexität
- maximale Langlebigkeit und Wartbarkeit
- offene Dokumentation (Open-Source-Baupläne)

---

## 📚 Verzeichnis der Gebäudetypen

### **Wohngebäude**
- [`tiny_house.md`](tiny_house.md)  
  Kleine Wohneinheit (35–55 m²), ideal für 1–2 Personen.  
  Minimalküche, effiziente Grundrisse, Holzbauweise.

- [`family_house.md`](family_house.md)  
  Größere Wohneinheit (70–100 m²) für Familien.  
  Fokus auf Reparierbarkeit, niedrige Betriebskosten.

---

### **Gemeinschaftsgebäude**
- [`canteens.md`](canteens.md)  
  Vier verschiedene Kantinen (A–D), jeweils mit eigener Funktion  
  (Schule, Industrie, Dorfzentrum, Spa & Naturzone).  
  Zentrales Ernährungskonzept des Dorfes.

- [`coworking_hub.md`](coworking_hub.md)  
  Arbeitsplätze für Remote-Worker, lokale Firmen, Lernende & Kurse.

- [`tiny_mall.md`](tiny_mall.md)  
  Mikro-Einkaufszentrum: Bäckerei, Gemüse, Bio, Mini-Shop, Konditorei,
  einfache Dienstleistungen.

- [`school.md`](school.md)  
  Schulgebäude für ~180 Kinder (9 Klassen), Räume für Werkstätten,
  Musik, Sport und Waldpädagogik.

- [`spa_center.md`](spa_center.md) (optional)  
  Gesundheits- und Erholungszentrum für Dorf & Besucher.

---

### **Technische & Produktionsgebäude**

- [`energy_center.md`](energy_center.md)  
  Holz-KWK, Speicher, Wärmenetz-Übergabepunkte, PV-Schnittstelle.

- [`sawmill.md`](../08_industry/sawmill.md)  
  Sägewerk: Verarbeitung des Holz aus dem 9 km² großen Dorfwald.

- [`metal_workshop.md`](../08_industry/metal_workshop.md)  
  Schlosserei: Metallteile für Häuser, Infrastruktur und Reparaturen.

- [`textile_workshop.md`](../08_industry/textile_workshop.md)  
  Näherei: Textilien, Reparaturen, langlebige Produkte.

Hinweis: Produktionsgebäude befinden sich im Ordner  
`/docs/08_industry/`, sind hier aber verlinkt, da sie Teil der
Gebäudestruktur sind.

---

## 🛠 Bauprinzipien für alle Gebäude

Alle Gebäude folgen denselben Grundsätzen:

### **1. Holzbauweise aus lokalem Wald**
- Tragwerk aus Brettschichtholz, KVH oder Rahmenbau  
- Material aus nachhaltigem Waldmanagement  
- lokale Wertschöpfung

### **2. Reparierbarkeit**
- Schraubverbindungen statt Klebeverbindungen  
- modulare Innenwände  
- Fenster/Türen genormt und ersetzbar  
- Elektroinstallation revisierbar

### **3. Standardisierte Module**
- Wandmodule  
- Dachmodule  
- Fußbodenmodule  
- Technikmodule (Wasser/IT/Strom)

-> erleichtert Serienproduktion und Wartung

### **4. Energieeffizienz**
- Anschluss an das Nahwärmenetz  
- kompakte Gebäudehülle  
- hochwertige Dämmung  
- Vorbereitung für PV, falls nötig

### **5. Gemeinschaft statt Überdimensionierung**
- kleine private Küchen  
- gemeinsame Kantinen  
- gemeinschaftliche Werkstätten  
- geteilte Infrastruktur (Coworking, Spa, Kultur)

---

## 🧩 Struktur jedes Gebäudedokuments

Jedes Gebäude hat eine eigene Datei mit:

1. **Zweck & Nutzung**
2. **Kapazität & Zielgruppe**
3. **Grundrissbeschreibungen**
4. **Materialkonzept**
5. **Energiekonzept**
6. **Wasser/Abwasser/IT**
7. **Bauhinweise**
8. **Stücklisten (BOM)**
9. **Wartungs- & Reparaturhinweise**
10. **Open-Source-Pläne (CAD, Bilder, Tabellen)**

---

## 📥 Mitarbeit

Du möchtest:
- Grundrisse ergänzen?
- CAD-Skizzen beitragen?
- Wand- oder Dachmodule definieren?
- neue Gebäudetypen vorschlagen?
- Energie- oder Installationsvarianten beschreiben?

Dann erstelle ein Issue oder einen Pull Request – wir freuen uns über jede Mitarbeit.

---

## 🏗 Ziel

Dieses Modul soll am Ende eine **vollständige Sammlung von Open-Source-
Gebäudeplänen** darstellen, die sofort reproduzierbar sind — für Tina
Village und für jede Gemeinschaft, die ein ähnliches Dorf bauen möchte.

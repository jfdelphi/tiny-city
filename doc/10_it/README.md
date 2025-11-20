# 10 – IT, Kommunikation & Steuerungssysteme (Information Technology)

Dieses Modul beschreibt die komplette digitale Infrastruktur von **Tina Village**.
Auch in einer nachhaltigen, weitgehend autarken Siedlung ist eine robuste,
gut wartbare und transparente IT-Struktur entscheidend:

- für Energie- und Wassersteuerung  
- für Monitoring aller Systeme  
- für interne Kommunikation  
- für Bildung & Arbeit  
- für Handel & Verwaltung  

Tina Village setzt auf **Open-Source, Transparenz, Reparierbarkeit und
Low-Tech-kompatible Wartung**.

---

# 🌐 1. Netzwerkarchitektur

### 1.1 Kernprinzipien
- Glasfaser-Backbone  
- modulare, austauschbare Komponenten  
- möglichst wenige proprietäre Systeme  
- Redundanz an den wichtigsten Punkten  
- klare Dokumentation aller Netze  

### 1.2 Netzwerk-Topologie
Die Siedlung nutzt eine **Ring-/Stern-Hybridstruktur**:

- Glasfaser-Ring durch das gesamte Dorf  
- Sternförmige Verteilung in Wohn- und Industriecluster  
- getrennte VLANs für:
  - Energie  
  - Wasser  
  - Monitoring  
  - Verwaltung  
  - Bewohner-Netz  
  - Gäste-Netz  

### 1.3 Anschlusspunkte
- zentrale Serverräume (2 redundant)  
- pro Gebäude ein IT-Verteilerkasten (klein, schraubbar, standardisiert)  
- RJ45 Cat6A oder SFP+ (je nach Gebäude)

### 1.4 WLAN
- Mesh-System  
- Indoor/Outdoor-APs  
- Gästevlan getrennt  
- zentral verwaltet, einfach ersetzbar  

---

# 🛰 2. Internet & Externe Anbindung

### 2.1 Primäre Anbindung
- Glasfaser zum regionalen Anbieter  
- mind. 1–10 Gbit Kapazität  

### 2.2 Backup-Anbindung
- Satellitenlink (z. B. Starlink, geclustert)  
- LTE/5G-Fallback (Industrie-Router)  
- automatische Umschaltung  

---

# 🖥 3. Server & Rechenzentrum

Tina Village betreibt **ein kleines, aber robustes Rechenzentrum**.

### 3.1 Servertypen
- 2× redundante Hauptserver (Proxmox, Kubernetes oder Docker)  
- 1× Backupserver im anderen Gebäudeteil  
- optional: kleiner Edge-Server pro Industriehalle  

### 3.2 Software
- Linux überall  
- Open-Source-Services  
- GitOps für Konfigurationsverwaltung  

### 3.3 Wichtige Anwendungen
- Energie-Monitoring  
- Wasser-Monitoring  
- Temperatur-/Feuchtesensorik  
- Siedlungs-App Backend  
- File-Storage  
- interne Wiki / Handbuch  
- Verwaltungssoftware  
- Backup-Skripte  

### 3.4 Redundanz & Backup
- RAID-ZFS oder RAID-10  
- tägliche Snapshots  
- Backup-Replikation ins Energiezentrum  
- optional externes Cloud-Backup (verschlüsselt)

---

# 📱 4. Siedlungs-App

Die App ist das digitale Rückgrat der Gemeinschaft.

### 4.1 Funktionen
- Energieverbrauch anzeigen  
- Wasserverbrauch anzeigen  
- Kantinenmenü  
- interne Kommunikation  
- Wartungsmeldungen  
- Events im Dorf  
- Dokumente & Baupläne  
- Meldung „Gerät kaputt“ → Reparaturzentrum  

### 4.2 Prinzipien
- Open-Source  
- datensparsam  
- offline-fähig  
- Web-App + optional mobile App  

### 4.3 Vernetzung
Sie liest Daten aus:
- Energie (04)  
- Wasser (05)  
- Waste (06)  
- Food (07)  
- Industrie (08)  
- Infrastruktur (03)  

Die App ist die **Benutzerschnittstelle zu allen Systemen**.

---

# 🔐 5. Cybersecurity

Da alle Systeme (Energie, Wasser, IT) digital gesteuert werden, ist
Cybersecurity zentral.

### 5.1 Grundprinzipien
- Zero-Trust  
- klare Rollen & Berechtigungen  
- verschlüsselte Kommunikation  
- getrennte Netze (kritisch vs. nicht kritisch)  
- keine Cloudabhängigkeit  

### 5.2 Maßnahmen
- Firewall (mehrstufig)  
- IDS/IPS  
- regelmäßige Audits  
- Offline-Backups  
- physischer Zugriffsschutz  

### 5.3 Personal
- mindestens 1 Cybersecurity-Spezialist  
- zusätzlich 1 IT-Admin für Wartung  

---

# 🎛 6. Gebäudeautomatisierung

### 6.1 Systeme
- Temperatur  
- Lüftung  
- Feuchtigkeit  
- Energieübergabestationen  
- Warmwasser  
- Sensoren in Wohn- & öffentlichen Gebäuden  
- einfache Schnittstellen (Modbus, MQTT)  

### 6.2 Ziel
- **keine proprietären Smart-Home-Ökosysteme**  
- stattdessen robuste, offene Industrie-Standards  
- einfache Wartung durch die Dorfwerkstatt  

---

# 🔌 7. IoT & Sensorik

### 7.1 Sensorarten
- Energiefluss, Wärme, Druck  
- Wasserqualität, Wasserstand  
- Luftqualität  
- Temperatur, Luftfeuchte  
- Tür-/Fenstersensoren  
- Bodenfeuchte (Landwirtschaft)  

### 7.2 Kommunikation
- Ethernet bevorzugt  
- MQTT/Modbus  
- LoRaWAN für Außenbereiche  
- klare Dokumentation der Protokolle  

---

# 🧰 8. Reparierbarkeit & Ersatzteile

### 8.1 Hardware
- Standardserver  
- austauschbare Router  
- OpenWRT-fähige Hardware  
- keine Hochpreis-Proprietärsysteme  

### 8.2 Software
- Konfiguration per Git (GitOps)  
- Automatisierte Installationen (Ansible)  
- Dokumentierte Adressen und Ports  
- Open-Source-Anwendungen  

---

# 🧩 9. Schnittstellen zu anderen Modulen

Die IT ist verbunden mit:

- `04_energy` (Monitoring & Steuerung)  
- `05_water` (Sensorik, Alarme)  
- `06_waste` (Füllstandsmeldungen)  
- `07_food` (Lager & Kantinen)  
- `08_industry` (Maschinen, Produktion)  
- `03_infrastructure` (Leitungen, Verteilkästen)  
- `11_governance` (interne Verwaltung)  

---

# 📥 10. Mitarbeit

Gesucht werden Beiträge zu:

- Netzwerkdesign  
- Cybersecurity-Konzepte  
- IoT-Sensoren  
- Open-Source-Smart-Home-Module  
- Monitoring-Systemen  
- DevOps & Automatisierung  
- Siedlungs-App (Frontend/Backend)  

Bitte ein Issue erstellen oder Pull Request einreichen.

---

# 🎯 Ziel dieses Moduls

Ein vollständig dokumentiertes, langlebiges, reparierbares
IT-System, das:

- unabhängig  
- sicher  
- energieeffizient  
- skalierbar  
- modular  
- Open-Source-freundlich  

ist und jede moderne ökologische Gemeinschaft dabei unterstützt,
effizient und stabil zu funktionieren.


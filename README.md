# CAMT & CSV Finanz-Dashboard 🇨🇭

Ein modernes, browserbasiertes Finanz-Dashboard zur Analyse von Schweizer Kontoauszügen (**CAMT.053 ISO-20022 XML**, **Bank-CSVs** und **JSON-Sicherungen**).

Alle Analysen und Berechnungen laufen zu 100 % lokal im Browser. Es werden keinerlei Finanzdaten auf externe Server hochgeladen.

---

## ✨ Hauptmerkmale

- 🔒 **100 % Lokal & Datenschutz-konform**: Keine Server-Uploads, Daten bleiben im Browser.
- 📂 **Multi-Format Import**:
  - **CAMT.053 XML** & **ZIP-Archive** direkt aus dem E-Banking (z. B. UBS, PostFinance, Raiffeisen, ZKB, Valiant, BEKB u.v.m.).
  - **CSV-Dateien** Schweizer Banken & Fintechs (Neon, Yuh, Revolut, Trade Republic etc.).
  - **JSON-Sicherungsdateien** zum 1:1 Wiederherstellen des vollständigen Zustands.
- 💡 **Automatische Kategorisierung & Regel-Editor**:
  - Vordefinierte Regeln für über 80 Schweizer Händler, Supermärkte, ÖV, Abos & Gastronomie.
  - **Eigene Regeln anlegen** mit Live-Regex-Vorschau und rückwirkender Anwendung auf bestehende Transaktionen.
- 📊 **Ausgaben vs. Kontobewegungen (PR #2)**:
  - Unterscheidung zwischen echtem Konsum, Bargeldbezügen, Umbuchungen und P2P-Transaktionen (z. B. TWINT mit Privatpersonen).
  - P2P-Zahlungen werden netto mit Rückzahlungen verrechnet.
- 📈 **Visualisierungen & Analytics**:
  - 8 interaktive Chart.js Visualisierungen (Donut-Charts, Monatsvergleich, Vermögensverlauf, Wochentags-Heatmap, Ausreisser-Scatterplot).
  - Ausreisser-Erkennung basierend auf Median & Interquartilsabstand (IQR) pro Kategorie.
- 💾 **Auto-Speichern & Export**:
  - Automatisches Speichern im Browser (`localStorage`).
  - Export als aktualisierte HTML-Einzeldatei, JSON-Backup oder UTF-8 CSV.
- 🌓 **Darkmode & Responsive Design**:
  - Veredeltes Design-System mit CSS-Tokens, SVG-Icons und flüssiger Anpassung für Smartphones (ab 390px), Tablets und Desktop.

---

## 🚀 Schnellstart

1. Lade die Datei `index.html` herunter oder klone dieses Repository:
   ```bash
   git clone https://github.com/Valsante/finance-dashboard.git
   ```
2. Öffne `index.html` einfach per Doppelklick in einem beliebigen modernen Browser (Chrome, Firefox, Safari, Edge).
3. Ziehe deine **CAMT.053 XML-** oder **CSV-Kontoauszüge** per Drag & Drop in das Import-Feld.
4. *(Optional)* Klicke auf **"Beispieldaten laden"**, um das Dashboard mit 18 Monaten Beispieldaten unverbindlich auszuprobieren.

---

## 🛠️ Technologien

- **HTML5 & Vanilla CSS**: Modernes Design-System mit CSS-Variablen, Glassmorphism & HSL-Farbpalette.
- **JavaScript (ES6+)**: Reine Front-End Logik ohne externe Frameworks oder Build-Steps.
- **Chart.js v4.4.1**: Datenvisualisierung.
- **JSZip v3.10.1**: Direktes Entpacken von ZIP-exportierten Kontoauszügen im Browser.

---

## 📄 Lizenz

MIT License.

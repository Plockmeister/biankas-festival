# Soul Awakening Festival 2026 — Projektstatus
*Zuletzt aktualisiert: 15. Juni 2026*

---

## 🎯 Projekt-Übersicht

**Festival:** Soul Awakening Festival 2026  
**Datum:** 21.–23. August 2026 (67 Tage)  
**Ort:** Hotel Lethehof, Friedrichstraße 74, 26203 Wardenburg  
**Veranstalterin:** Bianka Hugen  
**Webmaster:** Daniel Plock  

**Website:** https://soul-awakening-festival.com  
**GitHub:** https://github.com/Plockmeister/biankas-festival  
**Lokale Datei:** `C:\CLAUDE\CLAUDE CODE\Biankas Festival\index.html`  

---

## 🚀 Hosting & Deploy

| Was | Details |
|-----|---------|
| **Hosting** | GitHub Pages (kostenlos, unbegrenzt) |
| **Deploy** | `git add . && git commit -m "..." && git push` → live in ~1 Min |
| **DNS** | Hetzner → soul-awakening-festival.com |
| **SSL** | GitHub Let's Encrypt (automatisch) |
| **NETLIFY** | ❌ NICHT MEHR NUTZEN — 300 Credits verbraucht |
| **Formspree** | ✅ Aktiv — ID `xnjylzzd` → sendet an bianka.hugen@gmx.de |
| **Auto-Reply** | ❌ Nicht auf Free-Plan — Bianka antwortet manuell. Plan: EmailJS sobald Bianka Gmail hat |

---

## 📄 Website-Struktur

| Datei | Inhalt |
|-------|--------|
| `index.html` | Hauptseite (alle Sektionen) |
| `impressum.html` | Impressum |
| `datenschutz.html` | Datenschutzerklärung |
| `agb.html` | AGB |

### Sektionen in index.html (von oben nach unten):
1. **Hero** — Logo, Countdown, CTA-Button
2. **About** — Übersichtsbild (100% Breite), 3 Textblöcke, Stats, Features
3. **Speaker** — 12 Speaker-Karten (inkl. Riccardo Avola) + Moderatoren
4. **Workshops** — Karten mit Speaker-Fotos (object-position center 15%)
5. **Programm** — ⚠️ AUSGEBLENDET (`display:none`) — wartet auf Google Sheet
6. **Feuerlauf** — Highlight-Sektion
7. **Tickets** — Early Bird €249 / Standard €299 / VIP Early Bird €449 (regulär €499)
8. **Buchungsformular** — Formspree, Felder: Name, E-Mail, Adresse, Ticket, Feuerlauf, Nachricht
9. **Moderation** — Bianka + Thomas (160px Fotos, zentriert)
10. **Unterkunft** — Lethehof + Verpflegung
11. **FAQ**
12. **Footer**

---

## 👥 Speaker (Stand: 15.06.2026)

| Nr | Name | Foto | Vortrag | Workshop | Bio | Status |
|----|------|------|---------|----------|-----|--------|
| 1 | Thomas Schmelzer | ✅ | ✅ | ✅ | ✅ | fertig |
| 2 | Samu Vitatum | ✅ | ⚠️ | ⚠️ | ✅ | Klären: Workshop "Non Duality" rein oder nicht? |
| 3 | Dr. Marc Stollreiter | ✅ | ⚠️ | ⚠️ | ✅ | Vortrag + Workshop-Text fehlt |
| 4 | Susanne Hühn | ✅ | ⚠️ | ⚠️ | ✅ | Vortrag + Workshop-Text fehlt |
| 5 | Bettina Hallifax | ✅ | ⚠️ | ⚠️ | ✅ | Vortrag + Workshop-Text fehlt |
| 6 | Renate Dertinger | ✅ | ⚠️ | ⚠️ | ✅ | Vortrag + Workshop-Text fehlt |
| 7 | Bianka Hugen | ✅ | ⚠️ | ⚠️ | ✅ | Besseres Foto kommt; Workshop-Text fehlt |
| 8 | Verena Jaus | ✅ | ⚠️ | ⚠️ | ✅ | Neue Bio aus Mail ausstehend; Vortrag: "Warum Spiritualität allein nicht die Antwort ist" |
| 9 | Desiree Salomon | ✅ | ⚠️ | ⚠️ | ✅ | Vortrag + Workshop-Text fehlt |
| 10 | Pjotr & Charlene Elkunoviz | ✅ | ⚠️ | ⚠️ | ✅ | Schreibweise "Geistige Aufrichtung" prüfen |
| 11 | Andy Schwab | ❌ | ❌ | ❌ | ❌ | Wartet auf Zusage, Foto + Bio |
| 12 | Riccardo Avola | ✅ | —  | ✅ | ✅ | Fertig — kein Vortrag, singt Fr + Heilkreis Sa/So |
| -- | Manfred Mohr | -- | -- | -- | -- | ABGESAGT — gestrichen |

---

## 🖼 Medien-Ordner

```
Medien/
├── Festival/
│   ├── Speaker/          ← Speaker-Fotos inkl. Riccardo-Avola-2026-06-13.jpg
│   ├── Angebote/         ← Klangliege (113,114), Breathwork (111,115), Aroma-Massage
│   ├── Feuerlauf/        ← Siluette✅, Titelbild, WhatsApp, fire-2-120
│   ├── Handpan/          ← IMG-2174✅, IMG-8615, Hilla-Knipper-05
│   └── Programm/         ← diverse Speaker-Fotos + Opening-hellere-Version.png
└── Awakening Festival Logo.png
```

---

## 💰 Tickets & Preise (Stand: 15.06.2026)

| Ticket | Early Bird Preis | Regulär | Early Bird Frist |
|--------|-----------------|---------|------------------|
| Festival-Ticket | €249 | €299 | bis 29. Juli 2026 oder 50 Tickets |
| VIP-Ticket | €449 | €499 | bis 29. Juli 2026 oder 50 Tickets |

**Buchungsweg:** Formspree → E-Mail an Bianka → Bianka bestätigt nach Zahlungseingang  
**Bankdaten:** Bianka muss selbst im Formular/Bestätigungsseite eintragen (Claude darf keine IBAN eingeben)

---

## 🔴 Offene Aufgaben

### Sofort umsetzbar (Claude) — Nach Todo-Checkliste:
- [ ] Kacheltexte (Festival-Erlebnis): Heilung & Tiefe, Klang & Rhythmus, Breathwork, Feuerlaufen — Texte aus Word-Dok
- [ ] Speaker-Vortrag/Workshop-Texte: alle 6 haben noch "Details folgen" Platzhalter
- [ ] Verena Jaus: Positionierung "Die Sonnenfrau" + neue Bio einbauen
- [ ] Pjotr & Charlene: "Geistige Ausrichtung" → "Geistige Aufrichtung" prüfen
- [ ] FAQ: Storno entfernen, Parkplatz-Hinweis, Hotel-E-Mail (.de vs .com), Hunde-Hinweis, Aussteller-Infos
- [ ] Ticket-Leistungsübersicht per Checkliste aktualisieren
- [ ] About-Bereich: Textblöcke aus Word-Dok einbauen

### Wartet auf Bianka:
- [ ] Google Sheet mit Programm freigeben → Programm-Sektion einblenden
- [ ] Andy Schwab — Foto + Bio + Vortrag
- [ ] Besseres Foto von Bianka
- [ ] Taiko-Foto für "Klang & Rhythmus"-Kachel
- [ ] Workshop-Fotos: Symposium, Aromamassage (Querformat), Klangliege, Heilkreis, Musik, Handpan, Füße, Breathwork, Feuer, Taiko, Atemmeditation
- [ ] Samu Vitatum klären: Workshop "Non Duality" rein oder raus?
- [ ] Instagram + Facebook Links
- [ ] EmailJS-Setup → sobald Bianka Gmail-Adresse hat

### Technik:
- [ ] WebGL Hero-Animation — Canvas 300×150 Bug (kein Vollbild)
- [ ] Mobile-Check: Feuerlauf, Tickets, FAQ Sektionen

---

## 🎨 Design-Details

```css
--gold:      #C9A84C   /* Hauptgold */
--gold-dark: #8B6914   /* Dunkles Gold */
--rose:      #C4848C   /* Rosa */
--black:     #3D1F14   /* Hintergrund (warmes Dunkelbraun) */
--cream:     #F5EDE3   /* Cremefarbe */
```

**Schriften:** Cormorant Garamond (Überschriften), Inter (Text), Georgia (Fallback)

---

## 📝 Letzte Änderungen (15.06.2026)

- Programm-Sektion ausgeblendet (`display:none`) inkl. Nav-Links — wartet auf Programminhalt
- Workshop-Karten: Gruppen-Platzhalter-Bild ersetzt durch individuelle Speaker-Fotos
- Workshop-Bilder: `object-position: center 15%` — Gesichter nicht mehr abgeschnitten
- Bettina Halifax: korrektes Foto (großes H) in Workshop-Karte
- Riccardo Avola: Speaker-Karte + Modal hinzugefügt (kein Vortrag, Workshop: Heilkreis & Gesang)
- Speaker-Modal: Vortrag/Workshop-Felder getrennt angezeigt
- Formspree aktiviert: ID xnjylzzd → bianka.hugen@gmx.de
- Dankeseite vereinfacht (war identisch mit geplanter Bestätigungsmail)
- Übersichtsbild 100% Breite (außerhalb Container)
- VIP-Ticket Preisdarstellung korrigiert: "449 statt 499"-Bug behoben
  - VIP zeigt jetzt klar: Early Bird €449 (statt ~~€499~~), "Du sparst €50"
  - Early Bird Frist: 20. Juli → **29. Juli 2026** überall aktualisiert

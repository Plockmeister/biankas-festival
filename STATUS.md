# Soul Awakening Festival 2026 — Projektstatus
*Zuletzt aktualisiert: 17. Juni 2026*

---

## 🎯 Projekt-Übersicht

**Festival:** Soul Awakening Festival 2026  
**Datum:** 21.–23. August 2026 (65 Tage)  
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
| **Hosting** | GitHub Pages (kostenlos) |
| **Deploy** | `git add . && git commit -m "..." && git push` → live in ~1 Min |
| **DNS** | Hetzner → soul-awakening-festival.com |
| **SSL** | GitHub Let's Encrypt (automatisch) |
| **NETLIFY** | ❌ NICHT MEHR NUTZEN — 300 Credits verbraucht |
| **Formspree** | ✅ Aktiv — ID `xnjylzzd` → sendet an bianka.hugen@gmx.de |

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
2. **About** — Übersichtsbild, 3 Textblöcke, Stats, Features
3. **Speaker** — 12 Speaker-Karten + Moderatoren, alle mit „Mehr erfahren"-Button
4. **Festival-Erlebnis** — 4 Kacheln mit „Mehr erfahren"-Popups
5. **Workshops & Aktivitäten** — Karten inkl. Popups für Breathwork, Klangliege, Atemmeditation, Feuerlauf
6. **Programm** — 3-Tages-Tabs (Fr/Sa/So), zwei Tracks
7. **Feuerlauf** — Highlight-Sektion mit „Mehr erfahren"-Popup (Stefanie Greifzu / ONFIRE)
8. **Tickets** — Early Bird €249 / VIP Early Bird €449
9. **Buchungsformular** — Formspree, inkl. Cosmic Healer Option
10. **Moderation** — Bianka + Thomas (200px Fotos, zentriert)
11. **Unterkunft** — Lethehof + Vollverpflegung
12. **FAQ**
13. **Footer**

---

## 👥 Speaker (Stand: 17.06.2026)

| Nr | Name | Foto | Vortrag | Workshop | Bio | Status |
|----|------|------|---------|----------|-----|--------|
| 1 | Thomas Schmelzer | ✅ neu | ✅ | ✅ | ✅ | ✅ fertig |
| 2 | Samu Vitatum | ✅ | ✅ | — | ✅ | ✅ fertig |
| 3 | Dr. Marc Stollreiter | ✅ | ✅ | ✅ | ✅ | ✅ fertig |
| 4 | Susanne Hühn | ✅ | ✅ | ✅ | ✅ | ✅ fertig |
| 5 | Bettina Hallifax | ✅ | ✅ | ✅ | ✅ | ✅ fertig |
| 6 | Renate Dertinger | ✅ | ✅ | — | ✅ | ✅ fertig |
| 7 | Bianka Hugen | ✅ neu | ✅ | ✅ | ✅ neu | ✅ fertig |
| 8 | Verena Jaus | ✅ | ✅ | ✅ | ✅ neu | ✅ fertig |
| 9 | Desirée Salomon | ✅ | ✅ | ✅ | ✅ | ✅ fertig |
| 10 | Pjotr & Charlene Elkunoviz | ✅ | ✅ | ✅ | ✅ | ✅ fertig |
| 11 | Andy Schwab | ❌ | ❌ | ❌ | ❌ | ⏳ wartet auf Zusage |
| 12 | Riccardo Avola | ✅ | — | ✅ | ✅ | ✅ Gastauftritt |

---

## 🖼 Medien-Ordner (Stand: 17.06.2026)

```
Medien/
├── Festival/
│   ├── Speaker/          ← Thomas (neu), Bianka (neu), Verena, Riccardo, Moderation
│   ├── Breathwork/       ← Foto 1 (Kachel), Foto 2 (Workshop), Klangliege Foto Aktuell
│   ├── Angebote/         ← Aroma-Massage, Füßedrücken, Heilkreis, Roland-Hutner
│   ├── Feuerlauf/        ← Feuerlauf-neu.jpg
│   ├── Handpan/          ← IMG-2174, Hilla-Knipper-05
│   ├── Inspiration/      ← workshop_party-feiern.jpg
│   ├── Programm/         ← Steffen-Gross-Opening.JPG (Taiko)
│   ├── Unsortiert/       ← popup_breathwork-roland-aurelia.jpg
│   └── Workshops/        ← Symposium.jpg, Atemmeditation-neues-Foto-10.jpg
└── Awakening Festival Logo.png
```

---

## 💰 Tickets & Preise (Stand: 17.06.2026)

| Ticket | Early Bird | Regulär | Frist |
|--------|-----------|---------|-------|
| Festival-Ticket | €249 | €299 | bis 20. Juli 2026 oder 50 Tickets |
| VIP-Ticket | €449 | €499 | bis 20. Juli 2026 oder 50 Tickets |
| Cosmic Healer | persönlich mit Bianka | — | direkt melden |

---

## 🔴 Offene Aufgaben

| # | Was | Notiz |
|---|-----|-------|
| 1 | **Andy Schwab** | Foto + Bio + Vortrag/Workshop — wartet auf Zusage |
| 2 | **Gesang mit Riccardo** | Eigene Karte gewünscht? Foto fehlt |
| 3 | **Social Media Links** | Instagram + Facebook |
| 4 | **WebGL Hero-Animation** | Canvas-Bug (kein Vollbild) |

---

## 🎨 Design-Details

```css
--gold:      #C9A84C   /* Hauptgold */
--gold-dark: #8B6914   /* Dunkles Gold */
--rose:      #C4848C   /* Rosa */
--black:     #3D1F14   /* Hintergrund (warmes Dunkelbraun) */
--cream:     #F5EDE3   /* Cremefarbe */
```

**Schriften:** Cormorant Garamond (Überschriften), Inter (Text)

---

## 📝 Letzte Änderungen (17.06.2026)

- Thomas Schmelzer: neues Foto eingebaut
- Breathwork: Foto 1 (Kachel) + Foto 2 (Workshop-Karte) + Popup Roland+Aurelia
- Klangliege: neues Foto (Kachel + Karte + Popup)
- Atemmeditation: Atemmeditation-neues-Foto-10.jpg
- Party & das Leben feiern: neue Workshop-Karte (kostenfrei)
- Symposium: an erste Stelle Speaker-Workshops, vollbreit, MYSTICA.TV Hinweis
- Desirée: Titel „Spiritueller Business Coach"
- Aroma Heil Massage: Text nach Biankas Vorgabe
- Klang & Rhythmus Kachel: Taiko-Foto statt Handpan
- Hotel: Vollinfos (Empfehlung EZ+Verpflegung, Anreise Do–Mo, Ausstattung)
- Feuerlauf, Breathwork, Klangliege, Atemmeditation: Mehr-erfahren-Popups
- Bianka Bio: neue Version
- Renate: Vortragstitel korrigiert
- Mobile Modal-Fix: Text nicht mehr über Bild

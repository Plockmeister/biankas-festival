# Soul Awakening Festival 2026 — Projektstatus
*Zuletzt aktualisiert: 14. Juni 2026*

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
| **Ticketsystem** | QRTicket (noch nicht eingerichtet) — Pretix aufgegeben (zu teuer) |

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
2. **Feature-Cards** — 3 Highlights (Taiko, Feuerlaufen, Verbundenheit)
3. **Speaker** — 10 Speaker-Karten + 1 Platzhalter (Andy Schwab)
4. **Festival-Erlebnis** — 4 Foto-Blöcke (Klangliege, Handpan, Breathwork, Feuerlauf)
5. **Programm** — Tab-basiert Fr/Sa/So (Platzhalter, ab 12:00 Fr)
6. **Workshops** — 9 Karten mit Preisen
7. **Feuerlauf** — Highlight-Sektion
8. **Tickets** — Early Bird €249 / Standard €299 / VIP €499
9. **Moderation** — Bianka + Thomas (160px Fotos)
10. **Unterkunft** — Lethehof + Verpflegung
11. **FAQ**
12. **Footer**

---

## 👥 Speaker (Stand: 14.06.2026)

| Nr | Name | Foto | Bio | Status |
|----|------|------|-----|--------|
| 1 | Thomas Schmelzer | ✅ | ✅ | fertig |
| 2 | Samu Vitatum | ✅ | ✅ | fertig |
| 3 | Dr. Marc Stollreiter | ✅ | ✅ | fertig |
| 4 | Susanne Hühn | ✅ | ✅ | fertig |
| 5 | Bettina Hallifax | ✅ | ✅ | fertig |
| 6 | Renate Dertinger | ✅ | ✅ | fertig |
| 7 | Bianka Hugen | ✅ | ✅ | fertig (besseres Foto kommt) |
| 8 | Verena Jaus | ✅ | ✅ | fertig |
| 9 | Desiree Salomon | ✅ | ✅ | fertig |
| 10 | Pjotr & Charlene Elkunoviz | ✅ | ✅ | fertig |
| 11 | Andy Schwab | ❌ | ❌ | wartet auf Zusage |
| -- | Manfred Mohr | -- | -- | ABGESAGT — gestrichen |

**Gewünschte neue Struktur** pro Speaker-Modal:
```
Vortrag: [Thema]
Workshop: [Thema]
Bio: [Text]
```
→ Bianka geht alle Texte durch

---

## 🖼 Medien-Ordner

```
Medien/
├── Speaker/              ← aktive Speaker-Fotos
├── Festival/
│   ├── Angebote/         ← Klangliege (113,114), Breathwork (111,115), Aroma-Massage
│   ├── Feuerlauf/        ← Siluette✅, Titelbild, WhatsApp, fire-2-120
│   ├── Handpan/          ← IMG-2174✅, IMG-8615, Hilla-Knipper-05
│   ├── Programm/         ← diverse Speaker-Fotos
│   └── Speaker/          ← weitere Speaker-Fotos
├── lethehof.jpg          ← Lethehof-Foto
└── Awakening Festival Logo.png
```

---

## 🔴 Offene Aufgaben

### Sofort umsetzbar (Claude):
- [ ] WebGL Hero-Animation reparieren (Canvas-Größe falsch: 300×150 statt Vollbild)
- [ ] Mobile-Check: Feuerlauf, Tickets, FAQ Sektionen
- [ ] STATUS.md aktuell halten

### Wartet auf Bianka:
- [ ] Besseres Foto von Bianka
- [ ] Party-Foto (erstellt mit Gemini)
- [ ] Breathwork-Foto nochmal tauschen
- [ ] Taiko-Foto für "Klang & Rhythmus"
- [ ] Workshop-Fotos: Symposium, Aromamassage, Klangliege, Heilkreis, Musik, Handpan, Füße, Breathwork, Feuer, Taiko, Atemmedi
- [ ] Speaker-Texte: Vortrag + Workshop + Bio pro Speaker
- [ ] Mehr Workshops — welche kommen noch?
- [ ] Andy Schwab — Foto + Bio
- [ ] Finales Programm Fr/Sa/So
- [ ] "Open Text / Open Foto" — unklar was gemeint ist
- [ ] QRTicket registrieren → Ticket-Links ersetzen
- [ ] Instagram + Facebook Links
- [ ] Hintergrundfarbe — endgültige Entscheidung

### Technik:
- [ ] SSL aktiv? (GitHub Zertifikat prüfen)
- [ ] QRTicket IBAN → Bianka muss selbst eintragen

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

**Hero-Animation:** WebGL2 Shader (Matthias Hurrle / @atzedent) — fließende Wolken/Wind
- Canvas: `#hero-canvas`, opacity 0.85, blur 4px, brightness 1.3
- Problem: Canvas wird mit 300×150 statt Vollbild gerendert → in Reparatur

---

## 💰 Tickets & Preise

| Ticket | Preis | Early Bird Plätze |
|--------|-------|-------------------|
| Early Bird | €249 | 30 (27 noch verfügbar lt. Counter) |
| Standard | €299 | unbegrenzt |
| VIP | €499 | unbegrenzt |

**Ticketsystem:** QRTicket (0,90€/Ticket vom Käufer, kostenlos für Bianka)  
**Status:** Noch nicht eingerichtet — Bianka muss sich registrieren  
**Aktuell:** Links zeigen noch auf Pretix (muss geändert werden nach QRTicket-Setup)

---

## 📝 Letzte Änderungen (14.06.2026)

- Domain .de → .com überall korrigiert
- GitHub Pages aufgesetzt (ersetzt Netlify)
- Unterkunft: Mobile-Fix
- Moderation: Fotos 90px → 160px, zentriert
- Breathwork-Foto: Roland-Hutner-111.jpeg
- Unterkunft: "nur per E-Mail buchbar" hervorgehoben
- Programm: Hinweis-Banner + Fr ab 12:00 Uhr
- Festival-Erlebnis: Feuer-Silhouette-Foto zurück
- Speaker: "Unsere Speaker hautnah · 11 Speaker · 3 Tage"
- Feuerlauf: "kostenlos" ergänzt
- "Gemeinschaft" → "Verbundenheit & Austausch"

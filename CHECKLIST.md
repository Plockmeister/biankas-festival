# Soul Awakening Festival 2026 — Checkliste
*Zuletzt aktualisiert: 13. Juni 2026*

---

## ✅ Heute erledigt

- [x] GitHub Pages aufgesetzt → https://soul-awakening-festival.com
- [x] Domain .de → .com überall korrigiert (index, agb, datenschutz, impressum)
- [x] Unterkunft Mobile-Fix
- [x] Moderation-Fotos auf 160px vergrößert, zentriert
- [x] Breathwork-Foto → Roland-Hutner-111.jpeg (Kreis)
- [x] Unterkunft: "nur per E-Mail buchbar" hervorgehoben
- [x] Programm: Hinweis-Banner "wird laufend aktualisiert"
- [x] Hintergrundfarbe → #3D1F14 (warmes Dunkelbraun)
- [x] Riccardo-Avola Bildpfad korrigiert
- [x] "Gemeinschaft" → "Verbundenheit & Austausch"
- [x] Speaker-Überschrift → "Unsere Speaker hautnah · 11 Speaker · 3 Tage"
- [x] Feuerlauf-Text: "kostenlos" ergänzt
- [x] Programm Freitag: Start 12:00 Uhr (war 16:00)
- [x] Festival-Erlebnis item 04: Feuer-Foto zurück (Siluette), Titel "Feuerlaufen & Feier"

---

## 🔴 Warte auf Bianka — kommt noch

| # | Was | Notiz |
|---|-----|-------|
| 1 | **Hintergrundfarbe** | Bianka sucht noch was Besseres |
| 2 | **WebGL Wind-Animation** im Hero | War da, jetzt weg — prüfen ob Code noch drin |
| 3 | **Party-Foto** | Bianka erstellt mit Gemini |
| 4 | **"Open Text"** | Format: Logo, Überschrift, Foto, Text — Bianka schickt |
| 5 | **Breathwork-Foto** | Bianka wechselt nochmal |
| 6 | **Speaker-Texte** | Bianka geht durch: Vortrag + Workshop + Bio pro Speaker |
| 7 | **Mehr Workshops** | Bianka schickt Liste + Fotos |
| 8 | **Workshop-Fotos** | Symposium, Aromamassage, Klangliege, Heilkreis, Musik, Handpan, Füße, Breathwork, Feuer, Taiko, Atemmedi |
| 9 | **Taiko-Foto** | Für "Klang & Rhythmus" in Festival-Erlebnis |
| 10 | **Andy Schwab** | Foto + Bio (wartet auf Zusage) |
| 11 | **Bianka-Foto** | Besseres Foto von sich |
| 12 | **Programm-Zeiten** | Finales Programm Fr/Sa/So |
| 13 | **QRTicket** | Bianka registriert sich → dann Ticket-Links ersetzen |
| 14 | **Social Media** | Instagram + Facebook Links |

---

## 🔴 Technisch noch offen

- [ ] **SSL** — GitHub Zertifikat abwarten (~30 Min nach DNS)
- [ ] **1. GitHub Pages IP** `185.199.108.153` — wurde die in Hetzner eingetragen?
- [ ] **Ticket-Links** — von Pretix auf QRTicket wechseln (nach QRTicket-Setup)

---

## 📋 Speaker-Karten Struktur (laut Bianka)

Neue gewünschte Struktur pro Speaker-Modal:
```
[Name]
[Titel]

Vortrag: [Thema]
Workshop: [Thema]

[Bio]
```
→ Bianka geht alle Speaker-Texte nochmal durch und schickt die Infos

---

## 🌐 Deploy-Workflow

```bash
git add .
git commit -m "Beschreibung"
git push
```
→ ~1 Minute später live auf soul-awakening-festival.com

**NETLIFY NICHT MEHR NUTZEN** — Credits verbraucht!

---

## 🌐 DNS GitHub Pages (Hetzner)

| Typ | Name | Wert |
|-----|------|------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `plockmeister.github.io` |

GitHub Repo: https://github.com/Plockmeister/biankas-festival

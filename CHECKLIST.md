# Soul Awakening Festival 2026 — Checkliste
*Zuletzt aktualisiert: 13. Juni 2026*

---

## 🔴 Dringend — jetzt zu tun

- [ ] **GitHub Pages live prüfen** → https://plockmeister.github.io/biankas-festival/ (1-2 Min nach Push)
- [ ] **DNS umstellen** (sobald Bianka Hetzner-Code schickt) → neue GitHub Pages IPs eintragen (siehe unten)
- [ ] **QRTicket einrichten** → Bianka registriert sich auf https://qrticket.de/anmeldung.php
  - Dann: Ticket-Links in Website ersetzen (aktuell noch Pretix-Links!)
- [ ] **IBAN in QRTicket** → Bianka trägt Bankdaten selbst ein (Claude darf das nicht!)

---

## 🟡 Feedback von Bianka (13. Juni) — zu erledigen

- [ ] **Breathwork-Foto** — anderes Foto nehmen: Menschen die im Kreis liegen
  → Datei prüfen: `Medien/Festival/Angebote/Roland-Hutner-111.jpeg` oder `Roland-Hutner-112.jpeg`
- [ ] **Moderation-Fotos größer** — Bianka möchte sichtbarer sein im Moderation-Bereich
- [ ] **Unterkunft betonen** — "Nur per E-Mail buchbar" deutlicher hervorheben
- [ ] **Programm "Coming Soon"** — Andy Schwab hat noch nicht zugesagt; Programm-Sektion verstecken oder "Coming Soon" anzeigen um Verwirrung zu vermeiden
- [ ] **Mehr Workshops** — Bianka nennt noch weitere, konkrete Liste ausstehend
- [ ] **"Open Text fehlt noch"** — unklar was gemeint ist, bei Bianka nachfragen
- [ ] **"Open Foto fehlt noch"** — unklar was gemeint ist, bei Bianka nachfragen
- [ ] **Bianka-Foto** — sie schickt ein besseres Foto von sich

---

## 🟡 Inhalte ausstehend (von Bianka)

- [ ] **Andy Schwab** — Foto + Bio (wartet auf Zusage)
- [ ] **Programm-Zeiten** — Tagesablauf Fr/Sa/So noch Platzhalter
- [ ] **Social Media Links** — Instagram + Facebook aktuell auf `#`
- [ ] **AGB & Datenschutz** — Platzhalter bis Ticketsystem live ist

---

## ✅ Erledigt

- [x] Hero-Sektion (Logo, Countdown, CTA)
- [x] Speaker-Sektion — 10 echte Karten
- [x] Manfred Mohr — gestrichen (hat abgesagt)
- [x] Verena Jaus — Speaker-Karte mit Bio eingebaut
- [x] Bettina Hallifax — Foto eingebaut
- [x] Workshops & Aktivitäten (9 Karten mit Preisen)
- [x] Tickets (€249 / €299 / €499)
- [x] Moderation (Bianka + Thomas mit Fotos)
- [x] Unterkunft (Lethehof, info@hotel-lethehof.com — .com korrigiert!)
- [x] Feuerlauf-Sektion — Checkbox entfernt, Text "Für alle inklusive"
- [x] Festival-Erlebnis — echte Fotos (Klangliege, Handpan, Breathwork, Riccardo)
- [x] FAQ
- [x] Netlify Deploy (jetzt erschöpft — nicht mehr nutzen!)
- [x] **GitHub Pages aufgesetzt** → https://plockmeister.github.io/biankas-festival/
- [x] Pretix Ticketsystem eingerichtet (wird durch QRTicket ersetzt)

---

## 🌐 Deploy-Workflow (NEU — GitHub Pages)

```bash
cd "C:/CLAUDE/CLAUDE CODE/Biankas Festival"
git add .
git commit -m "Beschreibung der Änderung"
git push
```
→ Website ist nach ~1 Minute automatisch live.

**NETLIFY NICHT MEHR NUTZEN** — Credits verbraucht!

---

## 🌐 DNS-Einstellungen (GitHub Pages) bei Hetzner

**URL:** https://dns.hetzner.com → Zone `soul-awakening-festival.com`

Alte Einträge löschen, dann diese anlegen:

| Typ   | Name  | Wert                        | TTL  |
|-------|-------|-----------------------------|------|
| A     | `@`   | `185.199.108.153`           | 3600 |
| A     | `@`   | `185.199.109.153`           | 3600 |
| A     | `@`   | `185.199.110.153`           | 3600 |
| A     | `@`   | `185.199.111.153`           | 3600 |
| CNAME | `www` | `plockmeister.github.io`    | 3600 |

Danach: GitHub Repo → Settings → Pages → Custom Domain → "soul-awakening-festival.com" eintragen.

---

## 📋 Was Bianka selbst tun muss

1. **Hetzner DNS** — Code an Daniel schicken → DNS umstellen auf GitHub Pages
2. **QRTicket** — Account anlegen auf https://qrticket.de/anmeldung.php
3. **IBAN in QRTicket** — Bankdaten selbst eintragen
4. **Fotos** — besseres Foto von sich schicken
5. **Mehr Workshops** — Liste der weiteren Workshops schicken
6. **"Open Text" / "Open Foto"** — erklären was gemeint ist

---

## 📁 Wichtige Links

| Was | Link / Pfad |
|-----|-------------|
| Website (live) | https://plockmeister.github.io/biankas-festival/ |
| Website (Domain, nach DNS) | https://soul-awakening-festival.com |
| GitHub Repo | https://github.com/Plockmeister/biankas-festival |
| QRTicket Anmeldung | https://qrticket.de/anmeldung.php |
| index.html | `C:\CLAUDE\CLAUDE CODE\Biankas Festival\index.html` |
| Speaker-Fotos | `C:\CLAUDE\CLAUDE CODE\Biankas Festival\Medien\Speaker\` |

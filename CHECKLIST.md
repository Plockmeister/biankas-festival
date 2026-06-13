# Soul Awakening Festival 2026 — Checkliste
*Zuletzt aktualisiert: 12. Juni 2026*

---

## 🔴 Dringend — Inhalte fehlen noch

- [ ] **Andy Schwab** — Foto + Bio (du fragst ihn direkt)
- [ ] **Manfred Mohr** — Foto + Bio (du fragst ihn direkt)
- [ ] **Verena Jaus** — Speaker-Bio fehlt noch (Foto ist drin)

---

## 🟡 Inhalte ausstehend

- [ ] **Festival Erlebnis Sektion** — Inhalte noch unfertig, muss überarbeitet werden
- [ ] **Programm-Zeiten** — Tagesablauf Fr/Sa/So noch Platzhalter (wartet auf Bianka)
- [ ] **Social Media Links** — Instagram + Facebook aktuell auf `#` (Links eintragen wenn vorhanden)
- [ ] **AGB & Datenschutz** — Platzhalter bis Ticketsystem live ist

---

## 🔵 Technik — noch offen

- [ ] **Domain DNS** — Hetzner auf Netlify zeigen lassen (Bianka schickt dir morgen den Code)
  → Einstellungen siehe unten
- [ ] **Pretix — IBAN eintragen** — Bianka muss ihre Bankdaten selbst eintragen
  → URL: https://pretix.eu/control/event/soulawakeningfestival/saf2026/quickstart/
- [ ] **Pretix — Livemodus aktivieren** — nach IBAN-Eintrag unter „Einstellungen" → Livemodus
- [ ] **Pretix — Bianka als Team-Mitglied einladen** (optional, damit sie eigenen Zugang hat)
  → Pretix → Veranstalter → Teams → Neue Einladung

---

## ✅ Heute erledigt (12. Juni 2026)

- [x] Hero-Sektion (Logo, Countdown, CTA)
- [x] Speaker-Sektion (10 echte Karten + 2 Platzhalter Andy/Manfred)
- [x] Bettina Hallifax — Foto eingebaut
- [x] Workshops & Aktivitäten (9 Karten mit Preisen + Labels)
- [x] Tickets (€249 / €299 / €499, sauber ohne Add-ons)
- [x] Moderation & Führung (Bianka + Thomas mit Fotos)
- [x] Unterkunft (Nur Lethehof mit Foto + Link)
- [x] Feuerlauf-Sektion
- [x] FAQ
- [x] Netlify-Deploy live: https://beamish-centaur-0aa073.netlify.app
- [x] Custom Domain bei Netlify eingetragen: soul-awakening-festival.de
- [x] Pretix Ticketsystem eingerichtet (Testmodus)
  - Early Bird €249 · Standard €299 · VIP €499 · unbegrenzte Kontingente
  - Shop-URL: https://pretix.eu/soulawakeningfestival/saf2026/
- [x] Ticket-Buttons auf Website mit Pretix verlinkt
- [x] CHECKLIST.md angelegt

---

## 🌐 DNS-Einstellungen bei Hetzner (sobald Code von Bianka da)

**URL:** https://dns.hetzner.com → Zone `soul-awakening-festival.de`

Alte A-Records löschen, dann diese anlegen:

| Typ   | Name  | Wert                                    | TTL  |
|-------|-------|-----------------------------------------|------|
| A     | `@`   | `75.2.60.5`                             | 3600 |
| A     | `@`   | `99.83.190.102`                         | 3600 |
| CNAME | `www` | `beamish-centaur-0aa073.netlify.app`    | 3600 |

> Nach der Änderung dauert es 1–24 Stunden bis die Domain aktiv ist.
> SSL-Zertifikat wird danach automatisch von Netlify ausgestellt.

---

## 📋 Was Bianka selbst tun muss

1. **IBAN eintragen** → https://pretix.eu/control/event/soulawakeningfestival/saf2026/quickstart/
2. **Livemodus aktivieren** in Pretix (nach IBAN-Eintrag)
3. **Hetzner DNS** — Code an Daniel schicken, dann DNS umstellen

---

## 📁 Wichtige Dateien & Links

| Was | Link / Pfad |
|-----|-------------|
| Website (live) | https://beamish-centaur-0aa073.netlify.app |
| Website (Domain, nach DNS) | https://soul-awakening-festival.de |
| Pretix Shop | https://pretix.eu/soulawakeningfestival/saf2026/ |
| Pretix Admin | https://pretix.eu/control/event/soulawakeningfestival/saf2026/ |
| index.html | `C:\CLAUDE\CLAUDE CODE\Biankas Festival\index.html` |
| Speaker-Fotos | `C:\CLAUDE\CLAUDE CODE\Biankas Festival\Medien\Speaker\` |

**Netlify Site-ID:** `52b17895-179f-4fab-b6cf-538a67307ebb`  
**Deploy-Befehl:**
```
cd "C:/CLAUDE/CLAUDE CODE/Biankas Festival" && netlify deploy --prod --dir . --site 52b17895-179f-4fab-b6cf-538a67307ebb
```

# Soul Awakening Festival 2026 — Session-Übergabe

## Projekt-Übersicht
Landingpage für das **Soul Awakening Festival 2026** von Bianka Hugen.
Statische HTML-Website (kein Framework, kein CMS), bereit zum Upload auf Netlify.

**Festival-Daten:**
- Datum: 21.–23. August 2026 (Freitag–Sonntag)
- Ort: Lethehof, Friedrichstraße 74, 26203 Wardenburg (Oldenburg)
- Max. 200 Teilnehmer
- Veranstalterin: Bianka Hugen, Eichenstraße 6, 26340 Zetel
- Kontakt: kontakt@soul-awakening-festival.de

---

## Dateistruktur

```
Biankas Festival/
├── index.html          ← Haupt-Landingpage (alle CSS + JS inline)
├── impressum.html      ← Vollständiges Impressum (Biankas echte Daten)
├── datenschutz.html    ← DSGVO-Datenschutzerklärung (angepasst auf diese Site)
├── agb.html            ← AGB (2 Platzhalter für Pretix-Daten)
├── Medien/
│   └── Awakening Festival Logo.png  ← Logo (PNG, transparent)
└── .claude/
    └── launch.json     ← Lokaler Dev-Server: py -m http.server 3456
```

---

## Design-System

| Element | Wert |
|---|---|
| Primärfarbe Gold | `#C9A84C` / `#E8C96D` |
| Hintergrund dunkel | `#0A0A0A` / `#141414` |
| Hintergrund hell | `#F5F0E8` / `#FEFCF7` |
| Display-Font | Cormorant Garamond (Google Fonts) |
| Body-Font | Inter (Google Fonts) |
| Fonts werden erst nach Cookie-Zustimmung geladen (DSGVO) |

---

## Was bereits fertig ist ✅

### Landingpage (index.html)
- [x] Sticky Navigation mit Hamburger-Menü (Mobile)
- [x] Hero mit WebGL-Shader-Background (animiertes goldenes Feuer)
- [x] Live-Countdown bis 21.8.2026
- [x] Über-das-Festival-Sektion mit Features & Stats
- [x] 3 Headliner-Speaker (Platzhalter-Bilder, Namen fehlen noch)
- [x] 6 weitere Speaker (Platzhalter)
- [x] Festival-Erlebnis (4 Blöcke: Transformation, Gemeinschaft, Inspiration, Feuerlauf)
- [x] Programm mit 3 Tabs (Fr/Sa/So)
- [x] Feuerlauf-Highlight mit Interesse-Counter (localStorage)
- [x] Ticket-Bereich (Early Bird / Standard / VIP) mit Preisrechner
- [x] Add-on-Selector (Feuerlauf, Verpflegung, Übernachtung)
- [x] Unterkunft & Verpflegung mit allen Preisen
- [x] 3 Platzhalter-Partnerhotels
- [x] FAQ-Akkordeon (6 Fragen)
- [x] Footer mit Social Links

### Rechtliche Seiten
- [x] impressum.html — mit Biankas echten Daten
- [x] datenschutz.html — DSGVO-konform für diese spezifische Website
- [x] agb.html — vollständig, 2 Platzhalter (Buchungslink + Zahlungsarten)

### Technisches
- [x] DSGVO Cookie-Banner (3 Kategorien: Notwendig / Google Fonts / Analyse)
- [x] Google Fonts nur nach Zustimmung geladen
- [x] Cookie-Einstellungen im Footer aufrufbar
- [x] Scroll-Reveal-Animationen (Intersection Observer)
- [x] Prefers-reduced-motion berücksichtigt
- [x] WebGL-Shader pausiert wenn Hero nicht sichtbar (Performance)
- [x] Konfigurations-Block (CONFIG) ganz oben in index.html für Bianka

---

## Konfigurations-Block (oben in index.html)

```javascript
const CONFIG = {
  earlyBirdPreis: 199,       // ← noch Platzhalter
  standardPreis: 249,        // ← noch Platzhalter
  vipPreis: 399,             // ← noch Platzhalter
  earlyBirdPlaetze: 50,
  earlyBirdVerkauft: 23,
  vipPlaetze: 20,
  feuerlaufPlaetze: 50,
  feuerlaufVerfuegbar: 34,
  verpflegungProTag: 55,     // ← aus Biankas Email, korrekt
  uebernachtungEinzel: 85,   // ← korrekt
  uebernachtungDoppel: 65,   // ← korrekt
  uebernachtungMehrbett: 35, // ← korrekt
  uebernachtungCamper: 5,    // ← korrekt
  buchungsLink: "#tickets",  // ← MUSS ersetzt werden sobald Pretix/Ticket Tailor eingerichtet
  kontaktEmail: "kontakt@soul-awakening-festival.de",
  festivalDatum: new Date("2026-08-21T09:00:00"),
};
```

---

## Nächste Schritte — Priorität 1: Ticketbuchungssystem

### Entscheidung noch offen: Welches System?

| System | Kosten | Aufwand | Empfehlung |
|---|---|---|---|
| **Ticket Tailor** | ~€30/Monat Flatrate + Stripe-Gebühren | Mittel | ⭐ Empfohlen |
| Pretix Hosted | 2,5% pro Ticket (gedeckelt €15) + Zahlungsanbieter | Mittel | Teuer bei 200 Tickets |
| Eventfrog | Kostenlos für Veranstalter | Gering | Eingeschränkte Add-ons |

**Benötigt für alle Systeme:**
- QR-Code-Tickets per Email
- Seriennummer pro Ticket
- Scanner-App (iOS/Android) für Einlass
- Verschiedene Ticket-Kategorien (Early Bird / Standard / VIP)
- Add-ons (Feuerlauf-Checkbox mit Zählung, Verpflegung, Übernachtung)

**Nach Systemwahl zu tun:**
1. Account einrichten
2. Ticket-Kategorien anlegen (mit Preisen aus CONFIG)
3. Add-ons/Extras konfigurieren (Feuerlauf max. 50 Plätze!)
4. Buchungslink in CONFIG.buchungsLink eintragen
5. In agb.html Platzhalter für Zahlungsarten + Buchungslink ergänzen
6. In datenschutz.html Pretix/Ticket Tailor als Auftragsverarbeiter eintragen
7. Alle "Jetzt buchen"-Buttons in index.html prüfen

---

## Nächste Schritte — Priorität 2: Texte anpassen

### Was noch Platzhalter ist (mit ✏️ im Code markierbar):

**Speaker (index.html — Sektionen #speaker und #more-speakers):**
- 3 Headliner-Speaker: Name, Titel, Biografie, Foto
- 6 weitere Speaker: Name, Titel, Biografie, Foto
- Unsplash-Platzhalter-Bilder durch echte Fotos ersetzen

**Programm (index.html — Sektion #programm):**
- Genaue Uhrzeiten und Sessiontitel noch offen
- Speaker-Namen in den Sessions eintragen

**Partnerhotels (index.html — Sektion #unterkunft):**
- 3 Hotel-Karten: Namen und Abstände eintragen
- Oder: Hotels komplett entfernen wenn nicht gewünscht

**Footer Social Media:**
- Instagram-Link und Facebook-Link eintragen (aktuell `href="#"`)

**AGB (agb.html):**
- § 5.3 Zahlungsarten: Platzhalter nach Systemwahl ausfüllen
- § 4.1 Buchungsvorgang: Pretix/Ticket Tailor Link eintragen

**Impressum (impressum.html):**
- Bereits vollständig mit Biankas echten Daten ✅

---

## Noch nicht begonnen

- [ ] Netlify-Deployment und Domain-Verknüpfung
- [ ] Ticketbuchungssystem (Entscheidung + Einrichtung)
- [ ] Echte Speaker-Fotos und Biografien
- [ ] Echte Partnerhotel-Daten
- [ ] Social Media Links
- [ ] Bianka-eigene Texte in "Über das Festival" (aktuell aus Email-Text)
- [ ] AGB: Anwaltliche Prüfung empfohlen (besonders Feuerlauf-Haftungsabschnitt)
- [ ] Netlify CMS (optional, falls Bianka Inhalte selbst pflegen möchte)

---

## Hosting-Plan

1. **Jetzt zum Testen:** netlify.com/drop → Ordner reinziehen → öffentliche URL
2. **Für Launch:** Domain `soul-awakening-festival.de` auf Netlify zeigen
   - Netlify-Account erstellen
   - Site deployen (Drag & Drop)
   - Custom Domain einrichten
   - HTTPS wird automatisch von Netlify aktiviert

---

## Lokale Vorschau starten

```bash
# In "Biankas Festival"-Ordner:
py -m http.server 3456
# → http://localhost:3456
```

---

## Wichtige Hinweise für nächste Session

1. **Bianka bearbeitet Preise** über den CONFIG-Block ganz oben in `index.html` (klar kommentiert)
2. **Speaker-Inhalte** stehen im HTML mit `<!-- SPEAKER X NAME -->` Kommentaren
3. **Cookie-Banner** ist DSGVO-konform — Google Fonts erst nach Zustimmung
4. **WebGL-Shader** im Hero ist ein animierter Feuer/Licht-Effekt — funktioniert in allen modernen Browsern mit WebGL2 (Fallback: dunkler Hintergrund)
5. **AGB vor Launch** bitte rechtlich prüfen lassen (e-recht24.de oder Anwalt)

# HANDOFF — Soul Awakening Festival Website
*Zuletzt aktualisiert: 13. Juni 2026*

## Projekt
- **Datei:** `C:\CLAUDE\CLAUDE CODE\Biankas Festival\index.html`
- **Live-Demo:** https://beamish-centaur-0aa073.netlify.app
- **Domain (nach DNS):** https://soul-awakening-festival.de
- **Netlify Site-ID:** `52b17895-179f-4fab-b6cf-538a67307ebb`
- **Deploy-Befehl:** `cd "C:/CLAUDE/CLAUDE CODE/Biankas Festival" && netlify deploy --prod --dir . --site 52b17895-179f-4fab-b6cf-538a67307ebb`

---

## Ticketsystem: QRTicket (beschlossen!)

Pretix war zu teuer (~2% pro Ticket). Entscheidung fiel auf QRTicket:
- **QRTicket** (qrticket.de) — 0,90 EUR pro Ticket, zahlt der Kaeufer => fuer Bianka kostenlos
- Noch einzurichten: https://qrticket.de/anmeldung.php
- Nach Einrichtung: Ticket-Links in Website ersetzen (aktuell noch Pretix-Links!)
- Pretix-Account kann ignoriert werden (kein IBAN, noch Testmodus)

**Pretix (alt, nicht mehr genutzt):**
- Admin: https://pretix.eu/control/event/soulawakeningfestival/saf2026/
- Shop: https://pretix.eu/soulawakeningfestival/saf2026/

---

## Speaker-Karten (12 Slots)

| Nr | Name | Bio | Foto | Dateiname |
|----|------|-----|------|-----------|
| 1 | Thomas Schmelzer | OK | OK | thomas-schmelzer.jpg |
| 2 | Samu Vitatum | OK | OK | samu-vitatum.jpg |
| 3 | Dr. Marc Stollreiter | OK | OK | marc-stollreiter.jpg |
| 4 | Susanne Huehn | OK | OK | susanne-huehn.jpg |
| 5 | Bettina Hallifax | OK | OK | bettina-Halifax.jpg |
| 6 | Renate Dertinger | OK | OK | renate-dertinger.jpg |
| 7 | Bianka Hugen | OK | OK | bianka-hugen.jpg |
| 8 | Verena Jaus | OK | OK | verena-jaus.jpg |
| 9 | Desiree Salomon | OK | OK | desiree-salomon.jpg |
| 10 | Pjotr & Charlene Elkunoviz | OK | OK | pjotr-charlene-elkunoviz.jpg |
| 11 | Andy Schwab | FEHLT | FEHLT (Platzhalter) | wartet auf Info |
| -- | Manfred Mohr | ABGESAGT | - | gestrichen |

Neue Fotos in Medien/Festival/Speaker/ vorhanden - noch nicht eingebaut:
Bettina-Hallifax.png, Riccardo-Avola.jpg, Moderation-Bianka-Hugen.jpg, Verena-Jaus.jpg,
mehrere Thomas-Schmelzer-Fotos (142, 80, 89-2, 99zwei)

---

## Foto-Ordner

Medien/Speaker/         - Aktive Fotos fuer Speaker-Karten
Medien/Festival/
  Angebote/             - Klangliege (113,114), Breathwork (115), Aroma-Massage, Roland-Hutner
  Feuerlauf/            - Siluette, Titelbild, WhatsApp, fire-2-120
  Handpan/              - IMG-2174, IMG-8615, Hilla-Knipper-05
  Programm/             - Viele Speaker-Fotos (Bettina, Charlene+Pjotr, Desiree, Renate, Riccardo usw.)
  Speaker/              - Weitere Speaker-Fotos mit evtl. besserer Qualitaet
Medien/lethehof.jpg
Medien/Awakening Festival Logo.png

---

## Sektionen der Website

| Sektion | Status | Hinweis |
|---------|--------|---------|
| Hero | fertig | Countdown, CTA |
| Speaker | fertig | 10 echt + 2 Platzhalter |
| Workshops | fertig | 9 Karten mit Preisen |
| Feuerlauf | fertig | |
| Festival-Erlebnis | verbessert | Echte Fotos (Klangliege, Handpan, Breathwork, Feuerlauf). Texte koennen noch persoenlicher werden. |
| Programm | Platzhalter | Echte Zeiten fehlen noch von Bianka |
| Tickets | Achtung | Links zeigen auf Pretix - muss auf QRTicket geaendert werden |
| Moderation | fertig | Bianka + Thomas |
| Unterkunft | fertig | Nur Lethehof, info@hotel-lethehof.com |
| FAQ | fertig | |

---

## Domain Setup (noch offen)

soul-awakening-festival.de liegt bei Hetzner DNS.
Bianka muss Hetzner-Code schicken, dann DNS umstellen.

DNS-Eintraege bei dns.hetzner.com:
  A     @    75.2.60.5                            TTL 3600
  A     @    99.83.190.102                        TTL 3600
  CNAME www  beamish-centaur-0aa073.netlify.app   TTL 3600

---

## CSS-Patterns

Farben: --gold: #C9A84C | --gold-dark: #8B6914 | --rose: #E8D5C4 | --cream-mid: #F5EDE3 | --black: #0A0705

Speaker-Bild aktiv:    class="speaker-img"             object-fit:cover; object-position:center 20%; grayscale(15%)
Speaker-Bild Platzh.:  class="speaker-img placeholder"  object-fit:contain; background:#2a2020; filter:none

Speaker-Karte HTML-Struktur:
  <article class="speaker-card reveal" onclick="openSpeakerModal(this)"
    data-name="NAME" data-title="TITEL" data-theme="THEMA" data-bio="BIO TEXT"
    data-img="Medien/Speaker/DATEI.jpg">
    <div class="speaker-img-wrap">
      <img src="Medien/Speaker/DATEI.jpg" alt="NAME" class="speaker-img" loading="lazy">
      <div class="speaker-glow"></div>
    </div>
    <div class="speaker-info">
      <div class="speaker-name">NAME</div>
      <div class="speaker-title">KURZTITEL</div>
      <div class="speaker-bio">INFO · INFO</div>
    </div>
  </article>

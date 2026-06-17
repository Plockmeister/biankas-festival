# Soul Awakening Festival 2026 — Checkliste
*Zuletzt aktualisiert: 17. Juni 2026*

---

## ✅ Erledigt (Stand: 17. Juni 2026)

### Technisches Setup
- [x] GitHub Pages → https://soul-awakening-festival.com
- [x] Formspree aktiv (ID xnjylzzd → bianka.hugen@gmx.de)
- [x] SSL / DNS (Hetzner → GitHub Pages)

### Design & Layout
- [x] Hintergrundfarbe #3D1F14 (warmes Dunkelbraun)
- [x] Ticket-Layout: 2 Karten (Early Bird + VIP Early Bird)
- [x] VIP-Preisbug behoben (€449 statt €499 statt €499)
- [x] Mobile: Speaker-Modal Fix (Text lag über Bild)
- [x] Moderation-Fotos zentriert

### Speaker
- [x] Thomas Schmelzer: neues Foto + MYSTICA.TV Erwähnung (Karte + Moderation)
- [x] Samu Vitatum: Vortragstitel aktualisiert
- [x] Dr. Marc Stollreiter: Workshop-Titel eingebaut
- [x] Susanne Hühn: „des Inneren Kindes" (war „deines")
- [x] Bettina Hallifax: Vortrag + Workshop-Texte
- [x] Renate Dertinger: Vortragstitel korrigiert (Demenz-Feld)
- [x] Bianka Hugen: neue Bio + neues Foto
- [x] Verena Jaus: neue Bio + Titel „Die Sonnenfrau"
- [x] Desirée Salomon: Workshop + Titel „Spiritueller Business Coach"
- [x] Pjotr & Charlene: „Geistige Aufrichtung®" (war „Ausrichtung")
- [x] Riccardo Avola: als Gastauftritt (kein Workshop)
- [x] Andy Schwab: Platzhalter (wartet auf Zusage)
- [x] Alle Speaker: „Mehr erfahren"-Button öffnet Modal

### Speaker-Workshop-Karten
- [x] Symposium: an erster Stelle + vollbreit + MYSTICA.TV Hinweis
- [x] Bianka: „Expedition ins SEIN" mit echtem Titel
- [x] Marc: „Der direkte Kontakt zum Göttlichen in Dir"
- [x] Bettina: „Unter der Oberfläche"
- [x] Susanne: „Die Heldenreise des Inneren Kindes"
- [x] Desirée: „Die Geldidentität der neuen Zeit"
- [x] Andy Schwab: Platzhalter €30

### Workshops & Aktivitäten
- [x] Breathwork: neues Foto Kachel (Outdoor-Gruppe), Workshop-Karte (Roland+Aurelia)
- [x] Breathwork: Popup mit Roland + Aurelia, Hinweis Kontraindikationen
- [x] Klangliege: neues Foto + Popup mit vollständigem Inhalt
- [x] Atemmeditation: neues Foto (Atemmeditation-neues-Foto-10)
- [x] Atemmeditation: Popup mit Inhalten
- [x] Aroma Heil Massage: Verenas Text eingebaut
- [x] Party & das Leben feiern: neue Karte (kostenfrei)
- [x] Heilkreis & Gesang (Riccardo): Karte vorhanden
- [x] Taiko Trommeln: Karte mit Steffen-Gross-Foto

### Festival-Erlebnis Kacheln
- [x] Klang & Rhythmus: Taiko-Foto (statt Handpan)
- [x] Breathwork-Kachel: Breathwork Experience Foto
- [x] Feuerlauf-Kachel: Popup mit Stefanie Greifzu / ONFIRE-Infos
- [x] Heilung & Tiefe: Mehr-erfahren → Klangliege-Popup
- [x] Breathwork: Mehr-erfahren → Breathwork-Popup
- [x] Feuerlaufen: Mehr-erfahren → Feuerlauf-Popup

### Programm
- [x] 3-Tages-Programm vollständig (Fr/Sa/So) aus PDF eingebaut
- [x] Zwei Tracks: Hauptbühne + Workshopraum parallel
- [x] Highlights (★) entfernt (waren Biankas interne Notizen)

### Tickets & Buchung
- [x] Early Bird: €249 (statt €299), Frist 20. Juli 2026
- [x] VIP Early Bird: €449 (statt €499), Frist 20. Juli 2026
- [x] Cosmic Healer: Dropdown-Option (kein Online-Bezahlen)
- [x] Aufzeichnungen der Vorträge als Leistung eingebaut
- [x] Buchungsformular: Name, E-Mail, Adresse, Ticket, Feuerlauf, Nachricht

### Unterkunft & Verpflegung
- [x] Lethehof: Empfehlung EZ €85 + Verpflegung €55 = €140/Tag
- [x] Anreise Do–Mo, Montagsfrühstück +€15
- [x] Ausstattungshinweise (WLAN, Zimmer, Camper)
- [x] Hotel-Email: info@hotel-lethehof.de (Website: hotel-lethehof.com)

### FAQ
- [x] Storno-Hinweis entfernt
- [x] Hotel-Email .de bestätigt

---

## 🔴 Noch offen

| # | Was | Notiz |
|---|-----|-------|
| 1 | **Andy Schwab** | Foto + Bio + Vortrag/Workshop — wartet auf Zusage |
| 2 | **Gesang mit Riccardo** | Eigene Karte? Foto fehlt noch |
| 3 | **Social Media** | Instagram + Facebook Links |
| 4 | **WebGL Hero-Animation** | Canvas-Bug (kein Vollbild) |
| 5 | **Neue Thomas-Fotos prüfen** | Er hat mehrere Optionen geschickt — stimmt das neue? |

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

# Design Tokens — Claude Design Onboarding

Dieses Verzeichnis enthält die Design-Token-Dateien, die Claude Design beim Onboarding liest, um Design-Systeme projekt- und kundenspezifisch anzuwenden.

## Dateien

| Datei | Zweck |
|-------|-------|
| `casa-vitale.json` | Casa-Vitale-Branding (Pflegedienst, Schwarzwald-Baar-Kreis) |

## Nutzung mit Claude Design

### Schritt 1 — Onboarding in Claude Design

1. Claude Design öffnen: https://claude.ai/design
2. Neues Design-System anlegen (pro Kunde/Projekt eines)
3. Beim Onboarding den Inhalt der entsprechenden JSON-Datei in den Chat einfügen oder als Datei hochladen
4. Claude Design extrahiert Farben, Typografie und Component-Specs automatisch

### Schritt 2 — Prototype generieren

**Beispiel-Prompt für Casa Vitale:**
```
Generiere eine Landingpage mit folgenden Sektionen:
- Hero: "Pflege mit Herz in Brigachtal"
- 3 Leistungs-Cards: Grundpflege, Behandlungspflege, Palliativversorgung
- Testimonial-Slider mit 3 Kundenstimmen
- FAQ mit 5 Fragen
- Kontaktformular mit Karten-Einbindung
- Footer mit Navigation und Newsletter

Nutze das Casa-Vitale-Design-System.
```

### Schritt 3 — Export

Nach Fertigstellung:
- **standalone HTML** herunterladen (für manuellen Wix-Studio-Nachbau)
- **Send to Claude Code** (ab API-Verfügbarkeit für VAB-Pipeline)

## Token-Schema

Das Schema folgt einer Konvention ähnlich [Design Tokens Community Group](https://www.designtokens.org/), aber angereichert um:

- `colorSchemes[]` — 5 vordefinierte Section-Background-Varianten (VAB-spezifisch)
- `sectionTypes[]` — Section-Templates mit Default-Layout und Scheme
- `voice` — Tonalität, Sprache, CTA-Beispiele für Content-Generierung
- `brand.personality[]` — Charakter-Adjektive für Content-Ton

## Neue Projekte hinzufügen

Für einen neuen Kunden:
1. Kopie von `casa-vitale.json` erstellen, z.B. `handwerk-mueller.json`
2. Farben, Typografie, Voice auf Kundenmarke anpassen
3. `sectionTypes[]` an vorhandene Sektionen im Kunden-Briefing anpassen
4. Hochladen in neues Claude-Design-Design-System

## Sync-Strategie

Wenn VAB Design-Tokens aktualisiert (in `lib/design/section-styles.ts`), muss diese JSON-Datei manuell synchronisiert werden. Perspektivisch: Build-Skript `npm run export:tokens` der aus Code die JSON generiert.

## Referenzen

- [Claude Design Help Center](https://support.claude.com/en/articles/14604416-get-started-with-claude-design)
- [Anthropic Labs Announcement](https://www.anthropic.com/news/claude-design-anthropic-labs)
- VAB CLAUDE.md (Section „Design System")

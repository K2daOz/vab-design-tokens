# Voice-Regeln — Casa Vitale

**Diese Regeln sind nicht verhandelbar.** Sie werden in jedem Prompt an Claude Design, Claude Code oder andere AI-Tools explizit mitgeliefert, weil JSON-Schema-Felder nicht zuverlässig durchgesetzt werden.

## Harte Regeln (immer einhalten)

1. **Sie-Form durchgehend** — niemals Du, niemals „Sie werden Sie'd" oder gemischt. Beispiel:
   - ✅ „Sie wünschen sich Unterstützung im Alltag?"
   - ❌ „Du wünschst dir Unterstützung im Alltag?"
   - ❌ „Wenn du dir Unterstützung wünschst, kontaktieren Sie uns"

2. **Deutsche Sprache** — keine Anglizismen wo deutsches Wort existiert:
   - ✅ „Kontakt" / „Pflegeleistungen" / „Beratung"
   - ❌ „Contact" / „Services" / „Consulting"
   - Ausnahme: etablierte Fachbegriffe („Hospice" nein, „Palliativversorgung" ja)

3. **Medizinisch-fachlich, aber warmherzig** — Fachbegriffe korrekt, aber in menschliche Sprache eingebettet:
   - ✅ „Palliativversorgung — damit Sie die letzte Lebensphase in Würde erleben können"
   - ❌ „Palliative Care Services"
   - ❌ „Wir terminal-pflegen Sie zu Hause"

4. **Keine generischen Marketing-Floskeln**:
   - ❌ „Ihr Partner für innovative Pflegelösungen"
   - ❌ „Wir sind die Nummer eins"
   - ❌ „Seit X Jahren setzen wir Maßstäbe"
   - ✅ „Wir kommen zu Ihnen nach Hause und kümmern uns um das, was zählt"

5. **Konkrete Orte nennen** — Casa Vitale bedient spezifische Gemeinden:
   - Brigachtal, Donaueschingen, Villingen-Schwenningen, Bad Dürrheim, Mönchweiler, Blumberg-Zollhaus
   - Diese Ortsnamen in Überschriften und Body-Text verwenden, nicht nur „Schwarzwald-Baar-Kreis"

## Ton-Beispiele (gut vs. schlecht)

### Hero-Headline

| Gut | Schlecht |
|-----|----------|
| „Ambulante Pflege mit Herz — zu Hause im Schwarzwald" | „Your Partner for Care Excellence" |
| „Wenn das Zuhause Pflege braucht" | „Premium Pflegeservices 24/7" |
| „Würdevoll leben in den eigenen vier Wänden" | „Innovative Healthcare Solutions" |

### CTA-Buttons

| Gut | Schlecht |
|-----|----------|
| „Beratung anfordern" | „Get started" |
| „Kontakt aufnehmen" | „Contact Us" |
| „Jetzt Termin vereinbaren" | „Book Now" |
| „Mehr erfahren" | „Learn more" |

### Testimonials

| Gut | Schlecht |
|-----|----------|
| „Die Schwestern von Casa Vitale sind für meine Mutter wie Familie geworden." | „Casa Vitale is the best care service ever!" |
| „Nach dem Krankenhausaufenthalt hatte ich große Sorge — Casa Vitale hat alles geregelt." | „5 stars. Highly recommend." |

## Harte Verbote

- Keine Gender-Sterne oder -Doppelpunkte (Casa Vitale ist ein traditioneller Pflegedienst, Kundenstamm mehrheitlich 65+)
- Keine Emoji in Haupttexten (nur in Social-Media-Posts erlaubt, nicht auf Website)
- Keine Superlative ohne Beleg („beste", „führend", „innovativ")
- Keine falschen Versprechen über medizinische Ergebnisse

## Prompt-Einbindung

Immer als Anhang oder expliziter Block in Claude Design Prompts:

```
WICHTIGE REGEL: Verwende IMMER die höfliche Sie-Form im gesamten Text.
NIEMALS Du-Form, auch nicht im Hero oder in CTAs. 
Bei Verstoß: komplett neu generieren.
```

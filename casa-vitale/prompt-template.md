# Casa Vitale — Claude Design Prompt Template

Kopiere den kompletten Prompt unten in Claude Design. Ergänze am Ende projektspezifische Details (z.B. welche Unterseite, besondere Anforderungen).

---

## 🚨 ZU ANFANG JEDES PROMPTS — Voice-Regel (nicht entfernen)

```
WICHTIGE SPRACHREGEL, die DURCHGEHEND eingehalten werden muss:
Verwende IMMER die höfliche Sie-Form im gesamten Text.
Niemals Du-Form, auch nicht im Hero, in CTAs oder in Fließtext.
Deutsche Sprache ohne Anglizismen (außer etablierte Fachbegriffe).
Bei Verstoß gegen diese Regel: komplett neu generieren.
```

---

## Basis-Briefing (immer gleich)

```
Brand: Casa Vitale — Ambulanter Pflegedienst
Region: Schwarzwald-Baar-Kreis (Brigachtal, Donaueschingen, Villingen-Schwenningen, Bad Dürrheim, Mönchweiler, Blumberg-Zollhaus)
Zielgruppe: Pflegebedürftige Menschen und deren Angehörige, mehrheitlich 60+ Jahre
Tonalität: Warmherzig, fachlich-medizinisch kompetent, respektvoll, Sie-Form
Kein Du, keine Anglizismen, keine Marketing-Floskeln

Design-System: Siehe design-tokens/casa-vitale.json
- Primary: Pacific Blue #0091CD
- Accent: Alizarin Crimson #E21C21 (nur für wichtige CTAs)
- Dunkle Sektionen: Astronaut Blue #002b3d
- Typografie: Poppins Medium für Headings, Regular für Body
- 5 Color Schemes für Section-Hintergründe
```

---

## Standard-Site-Struktur

```
Generiere die folgende Sitemap für casavitale.care:

1. Startseite
2. Pflegeleistungen (Übersicht)
   - Grundpflege
   - Behandlungspflege  
   - Verhinderungspflege
   - Hauswirtschaft
   - Pflege bei Demenz
   - Palliativversorgung
3. Pflegeberatung
   - Pflegegradrechner
   - Ambulanter Pflegedienst
   - Ambulante Wohngruppe
4. Wohnen
   - Betreutes Wohnen
   - Standort Mönchweiler
   - Standort Blumberg-Zollhaus
   - Standort Bad Dürrheim
5. Jobs
   - Aktuelle Stellen
   - Ausbildung
   - Initiativbewerbung
6. Über uns
   - Standort Donaueschingen
   - Standort Villingen-Schwenningen
   - Standort Brigachtal
7. FAQ
8. Kontakt
9. Rechtliches (Impressum, Cookies)
```

---

## Standard-Sektions-Bausteine

Für jede Seite folgende Sektion-Typen nutzen (aus `design-tokens/casa-vitale.json`, Abschnitt `sectionTypes`):

- **Navbar** (Color Scheme 5, dunkelblau, sticky, Logo links, CTA rechts)
- **Hero** (Color Scheme 4, dunkel, max. 600px Höhe, H1 max. 2 Zeilen, 1-2 CTAs)
- **Cards Grid** (Color Scheme 1, 3–4 Karten, jeweils Icon + H4 + Body)
- **Content + Bild** (Color Scheme 3, hellblau, 2-spaltig, Bild 50%)
- **Testimonials** (Color Scheme 1, 3 Karten, 5 Sterne, echte deutsche Namen)
- **FAQ** (Color Scheme 1, Accordion, max. 860px Breite zentriert)
- **Kontakt** (Color Scheme 3, Info links, Karte rechts)
- **CTA-Banner** (Color Scheme 4, einmal pro Seite, harte Handlungsaufforderung)
- **Footer** (Color Scheme 5, Newsletter + 4 Link-Spalten + Credits)

---

## Beispiel-Prompt für eine Landing-Page

Kopiere diesen Block in Claude Design und passe die **fett**-markierten Teile an:

```
WICHTIGE SPRACHREGEL, die DURCHGEHEND eingehalten werden muss:
Verwende IMMER die höfliche Sie-Form im gesamten Text.
Niemals Du-Form, auch nicht im Hero, in CTAs oder in Fließtext.
Deutsche Sprache ohne Anglizismen (außer etablierte Fachbegriffe).
Bei Verstoß gegen diese Regel: komplett neu generieren.

Brand: Casa Vitale — Ambulanter Pflegedienst im Schwarzwald-Baar-Kreis.
Zielgruppe: Pflegebedürftige und Angehörige, 60+.
Ton: warmherzig, fachlich, respektvoll, Sie-Form.

Design-System: aus design-tokens/casa-vitale.json (via GitHub).

Generiere die Startseite mit folgenden Sektionen:

1. Navbar (Scheme 5, sticky)
   - Logo links: "Casa Vitale" 
   - Links: Pflegeleistungen, Pflegeberatung, Wohnen, Über uns
   - CTA rechts: "Beratung anfordern" (primary button, E21C21)

2. Hero (Scheme 4, dunkelblau)
   - H1: "Ambulante Pflege mit Herz — zu Hause in Brigachtal"
   - Body: Kurze Einleitung, 2-3 Sätze, Sie-Form.
   - CTAs: "Beratung anfordern" (primary) und "Kontakt" (outline)
   - Optional: Stimmungsbild rechts (Pflegerin mit Seniorin)

3. Leistungen — Cards Grid (Scheme 1, weiß)
   - H2: "Unsere Pflegeleistungen"
   - Subheading: 1 Satz Einleitung
   - 4 Cards: Grundpflege / Behandlungspflege / Verhinderungspflege / Palliativversorgung
   - Jede Card: Icon + H4 + 2-Zeilen-Body + "Mehr erfahren →"-Link

4. Über uns — Content + Bild (Scheme 3, hellblau)
   - H2: "Mehr als Pflege — wir sind für Sie da"
   - Body: Text über Team, Werte, Region
   - Liste: 4 Punkte mit Häkchen (z.B. "24/7 erreichbar", "zertifizierte Fachkräfte")
   - Bild rechts: Team-Foto oder Stimmungsbild

5. Testimonials (Scheme 1, weiß)
   - H2: "Das sagen unsere Kunden"
   - 3 Testimonials mit 5 Sternen, echte deutsche Namen, Ort aus der Region
   - Beispiel: "Die Schwestern sind wie Familie geworden." — Maria Schmidt, Donaueschingen

6. FAQ (Scheme 1)
   - H2: "Häufige Fragen"
   - 5 Accordion-Items zu: Kosten/Pflegekasse / Erstgespräch / Verfügbarkeit / Vertrauenspersonen / Kündigung

7. CTA-Banner (Scheme 4, dunkel)
   - H2: "Jetzt Beratungstermin vereinbaren"
   - Body: 1 Satz
   - Großer CTA-Button: "Kostenlos beraten lassen" (E21C21 accent)

8. Footer (Scheme 5, sehr dunkel)
   - Newsletter-Anmeldung oben
   - 4 Spalten: Leistungen / Beratung / Standorte / Jobs
   - Unten: Impressum, Datenschutz, Copyright

Typografie-Check:
- H1: Poppins 500, 72px, letter-spacing -0.72px
- H2: Poppins 500, 48px
- Body: Poppins 400, 16px, line-height 1.5

Spacing-Check:
- Section-Padding: 80px oben und unten
- Container max-width: 1280px
- Mobile-Padding: 20px

Abschlussregel:
Gib den Output als standalone HTML mit eingebettetem CSS.
Keine externen CSS-Frameworks (außer Google Fonts für Poppins).
```

---

## Tipps für Nachjustierung (nach Claude Design Output)

Wenn das Ergebnis nicht passt, hier die häufigsten Fehler und ihre Fixes:

| Problem | Fix-Prompt |
|---------|-----------|
| Du-Form schleicht sich ein | „Schreibe alle Texte neu in der höflichen Sie-Form. KOMPLETT neu." |
| Englische Wörter | „Alle englischen Begriffe durch deutsche Entsprechungen ersetzen." |
| Farben zu bunt/verspielt | „Halte dich streng an die 5 Color Schemes, keine anderen Farben." |
| Cards zu überladen | „Cards: nur Icon + Überschrift + 2-Zeilen-Text + Link, nichts sonst." |
| Hero zu hoch | „Hero max. 600px Höhe, zentriert, nicht overflow." |

---

## Zukünftige Kunden

Für jeden Neukunden:
1. Kopie dieser Datei anlegen: `design-tokens/[kundenname]/prompt-template.md`
2. Branding/Ton-Regeln anpassen
3. Site-Struktur an Kundenbedürfnis anpassen
4. Voice-Rules entsprechend modifizieren (Sie/Du je nach Zielgruppe)

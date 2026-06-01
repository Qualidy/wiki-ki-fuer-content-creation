# Kapitel 12 – Bilder verfeinern

<div class="kurs-progress">
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step done"></div>
  <div class="step active"></div>
  <div class="step"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie du aus vier Vorschlägen **die beste Variante** aktiv auswählst und begründest
- **Vary Subtle und Vary Strong** gezielt und sparsam einsetzen
- Wann **Upscale und Zoom** sinnvoll sind
- Wie du einen Prompt **anpasst**, statt unkontrolliert Varianten zu stapeln
- Häufige **Bildprobleme erkennen** und lösen
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und arbeite mit einem Bild aus den vorherigen Kapiteln weiter – oder erzeuge ein neues Ausgangsbild.
2. Bearbeite die **Kurzübungen**.
3. Arbeite die **Workshop-Aufgabe** durch.

---

## 12.1 Die vier Vorschläge sichten

Jeder Prompt liefert **vier Bilder**. Das ist keine Auswahl nach Geschmack – es ist eine professionelle Entscheidung. Kurze Prüfroutine vor dem Verfeinern:

**Komposition:**
- Ist das Hauptmotiv klar erkennbar?
- Gibt es genug Freiraum für spätere Text-Overlays?
- Ist das Bild für den geplanten Kanal richtig ausgerichtet?

**Markentreue:**
- Passen Farben, Stimmung und Stil zur Marke?
- Wirkt das Bild zum Ton der zugehörigen Caption?

**Technische Qualität:**
- Gibt es verzerrte Hände, Gesichter oder Proportionen?
- Sind unerwünschte Schriftelemente sichtbar?
- Ist das Bild scharf und nicht pixelig?

**Entscheidungsregel:**  
Wenn keine der vier Varianten in mindestens zwei dieser Punkte überzeugt → **Prompt überarbeiten**, nicht Vary verwenden.

---

## 12.2 Vary: Subtle und Strong

Nach der Auswahl eines Bildes stehen zwei Varianten-Funktionen zur Verfügung:

| Funktion | Wirkung | Wann nutzen |
|---|---|---|
| **Vary Subtle** | Kleine Abwandlungen, Grundidee bleibt erhalten | Das Bild ist fast richtig – Feintuning bei Licht, Farbe, kleinen Details |
| **Vary Strong** | Deutlichere Variationen, neues Layout möglich | Die Richtung stimmt, aber Komposition oder Stimmung soll stärker variieren |

**Empfohlener Workflow:**

```
Beste Variante wählen → Vary Subtle (1–2×) → wenn nötig Vary Strong → Finalbild Upscale
```

!!! warning "Vary-Falle vermeiden"
    Zu viele Vary-Runden führen zu Kontrollverlust: Man verliert den Überblick, welche Version am stärksten war. Maximal 3–4 Vary-Schritte – dann Entscheidung treffen oder Prompt neu formulieren.

---

## 12.3 Upscale

**Upscale** erhöht die Auflösung des ausgewählten Bildes für den Export. Für Marketing-Bilder immer durchführen, bevor das Bild heruntergeladen wird.

Wann upscalen:
- Vor dem Download für Social Media, Website oder Präsentation
- Wenn das Bild in Canva oder PowerPoint eingebunden wird

Wann **nicht** sofort upscalen:
- Wenn das Bild noch stark überarbeitet werden soll (erst Prompt anpassen oder Vary, dann upscalen)

---

## 12.4 Zoom Out und Pan

Weitere Funktionen für besondere Situationen:

| Funktion | Wirkung | Typischer Einsatz |
|---|---|---|
| **Zoom Out** | Erweitert die Szene um das bestehende Bild herum | Wenn der Bildrahmen zu eng ist und mehr Kontext gewünscht wird |
| **Pan** | Verschiebt den Bildausschnitt in eine Richtung | Für Banner oder Panorama-Formate |

Für den Kurs reicht in den meisten Fällen: **Prompt mit richtigem `--ar` → Upscale → Export**. Zoom und Pan sind Zusatzfunktionen für spezifische Layoutanforderungen.

---

## 12.5 Prompt anpassen statt neu starten

Wenn eine Variante fast passt, lohnt es sich, den Prompt **gezielt zu verändern** – nicht alles löschen und von vorn beginnen.

**Vorher – zu unruhig im Hintergrund:**
```
Organic muesli in ceramic bowl on kitchen table, morning light, product photo --ar 1:1
```

**Nachher – Hintergrund beruhigt, Licht konkreter:**
```
Organic muesli in white ceramic bowl on clean light oak table, soft morning window light, minimalist product photography, uncluttered background --ar 1:1 --no text, logo, clutter, busy background
```

**Was hat sich geändert?**
- `clean light oak table` statt `kitchen table` (konkreter)
- `soft morning window light` statt `morning light` (präziser)
- `minimalist product photography` ergänzt (Look klar)
- `uncluttered background` + `--no clutter, busy background` (Problem behoben)

Das entspricht dem Prinzip der **Folgeprompts aus Woche 1** – nur für Bilder.

---

## 12.6 Häufige Bildprobleme und Lösungen

| Problem | Ursache | Lösung |
|---|---|---|
| **Text im Bild unleserlich** | Midjourney kann keine Schrift rendern | `--no text, letters, words` + Text in Canva ergänzen |
| **Hände verzerrt** | Anatomisch schwieriges KI-Thema | `--no distorted hands, extra fingers` oder Bildausschnitt ohne Hände wählen |
| **Hintergrund zu unruhig** | Szene nicht klar genug beschrieben | `clean background`, `blurred background`, `--no cluttered background` |
| **Farben passen nicht** | Keine Farbvorgabe im Prompt | Farbpalette direkt benennen: `sage green and cream palette, muted tones` |
| **Bild wirkt zu künstlich** | Midjourneys Standard-Glanz | `photorealistic, natural imperfections, shot on DSLR` oder `--style raw` |
| **Produkt nicht klar erkennbar** | Motiv zu weit hinten im Prompt | Hauptmotiv an den Anfang des Prompts stellen |
| **Kein Freiraum für Text** | Layout nicht geplant | `negative space at top` oder `centered product, empty background` |

---

## 12.7 Entscheidungshilfe – was tun wenn …

```
Ergebnis nicht gut?
│
├── Keines der 4 Bilder passt?
│   → Prompt überarbeiten (MSLK prüfen, Reihenfolge, --no ergänzen)
│
├── 1–2 Bilder fast passend?
│   → Vary Subtle 1–2×
│   → Wenn immer noch nicht gut: Vary Strong
│
├── Bild gut, aber kleines Detail stört?
│   → Vary Subtle (gezielt)
│
└── Bild gut, nur Auflösung zu gering?
    → Upscale → Download
```

---

## Kurzübungen

{{ task(file="tasks/tag12_01.yaml") }}

{{ task(file="tasks/tag12_02.yaml") }}

{{ task(file="tasks/tag12_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k12.yaml") }}

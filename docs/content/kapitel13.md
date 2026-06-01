# Kapitel 13 – Bilder für Social Media und Marketing

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
  <div class="step done"></div>
  <div class="step active"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Welche **Bildformate** zu welchen Kanälen passen – und warum
- Unterschied zwischen **Produktfoto** und **Lifestyle-Bild**
- Wie Personen im Bild sinnvoll eingesetzt werden – und wo Risiken liegen
- Wie ein **Bild-Briefing** vor dem Prompt die Qualität verbessert
- Wie Bild (Midjourney) und Text (Copilot) im Workflow zusammenkommen
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und erzeuge die Beispiel-Prompts in Midjourney.
2. Bearbeite die **Kurzübungen**.
3. Arbeite die **Workshop-Aufgabe** durch.

---

## 13.1 Formate nach Kanal

Das richtige Seitenverhältnis ist keine Ästhetik-Entscheidung – es ist eine **technische Voraussetzung**. Ein falsch formatiertes Bild wird auf dem Kanal abgeschnitten oder verzerrt dargestellt.

| Kanal | Typisches Format | Parameter |
|---|---|---|
| Instagram Feed (Quadrat) | 1:1 | `--ar 1:1` |
| Instagram Feed (Hochformat) | 4:5 | `--ar 4:5` |
| Instagram Story / Reels Cover | 9:16 | `--ar 9:16` |
| LinkedIn Post-Bild | 1:1 oder 4:3 | `--ar 1:1` oder `--ar 4:3` |
| LinkedIn Banner / Header | 4:1 | `--ar 4:1` |
| Website-Banner (breit) | 16:9 oder 3:1 | `--ar 16:9` |

**Freiraum für Text-Overlays:**  
Wenn später in Canva eine Headline oder Caption auf das Bild kommt, muss dieser Platz **im Prompt eingeplant** werden:

```
negative space at top           → Text oben im Layout
negative space on the left      → Text links (für Querformat-Banner)
centered product with empty background → Text unterhalb oder seitlich
```

---

## 13.2 Produkt vs. Lifestyle

Die beiden häufigsten Bildtypen im Marketing verfolgen unterschiedliche Ziele:

| Typ | Ziel | Prompt-Schwerpunkt | Beispiel |
|---|---|---|---|
| **Produktfoto** | Produkt klar erkennbar, Details sichtbar | `studio, sharp focus, clean background, centered` | Shop-Bild, Website |
| **Lifestyle** | Emotion, Alltagsszene, Marken-Feeling | `in context, natural light, candid, brand mood` | Instagram, Kampagne |

**Nordkorn (Müsli) – Produktfoto für Shop:**
```
Nordkorn organic granola bag front view on clean white studio background, sharp focus, centered composition, product photography --ar 1:1 --no text, logo, shadow, clutter
```

**Nordkorn – Lifestyle für Instagram:**
```
Healthy granola breakfast bowl on wooden kitchen table, blurred morning kitchen background, cozy lifestyle photography, warm early light --ar 4:5 --no text, logo
```

Beide Bilder zeigen dasselbe Produkt – der Kontext erzählt zwei verschiedene Geschichten.

---

## 13.3 Personen im Bild

Lifestyle-Bilder mit Menschen wirken oft authentischer als reine Produktfotos. Dabei gelten klare Regeln:

**Was funktioniert:**
- Generische, nicht erkennbare Personen (kein Gesicht, oder Gesicht im Hintergrund)
- Hände, die mit dem Produkt interagieren (z. B. Tasse halten, Buch aufschlagen)
- Silhouetten, Rückenansichten, angeschnittene Personen

**Was vermieden werden sollte:**
- Echte, erkennbare Personen ohne Einwilligung
- Prominente oder öffentliche Figuren
- Gesichter in sehr hoher Detailauflösung (können täuschend echt wirken)

**Technisch:**  
Hände und Gesichter sind fehleranfällig. Immer prüfen:

```
--no distorted hands, extra fingers, deformed face, unrealistic proportions
```

**Beispiel – GreenLoop Lifestyle mit Person:**
```
Young woman in sage green linen dress, urban street setting with greenery, natural light, editorial fashion photography, face not visible, candid walk --ar 4:5 --no text, logo, distorted hands, identifiable face
```

---

## 13.4 Text und Logo – die wichtigste Regel

**Midjourney erzeugt keinen verwendbaren Text.** Was wie Schrift aussieht, ist in der Regel unleserlicher Buchstabensalat. Das ist keine Schwäche, sondern eine Eigenschaft, die den Workflow definiert.

**Konsequenter Drei-Schritt-Workflow:**

1. **Midjourney** → Bild ohne jeglichen Text (`--no text, logo, watermark`)
2. **Copilot** → Caption, Headline, CTA formulieren
3. **Canva / Figma / PowerPoint** → Bild + Text zusammenführen

Das ist der **reale Workflow in Agenturen** – kein Tool macht alles. Wer das versteht, arbeitet effizienter als jemand, der Midjourney zur „Komplettlösung" machen will.

!!! tip "Markenlogo erst am Schluss"
    Das Logo kommt nie aus Midjourney – immer als eigene Ebene im Layout-Tool. Marke = Bild (Midjourney) + Text (Copilot) + Logo (eigene Datei).

---

## 13.5 Briefing vor dem Prompt

Ein kurzes Briefing vor dem Prompten verhindert ziellose Versuche. Auch ohne Berufserfahrung genügen wenige Stichpunkte:

| Briefing-Feld | Beispiel (Waldwerk) |
|---|---|
| Marke & Zielgruppe | Waldwerk, Outdoor-Ausrüster, 25–45, aktiv |
| Kanal & Format | Instagram Feed, 1:1 |
| Motiv / Botschaft | Neue Kollektion Herbst – Rucksäcke |
| Stimmung | Abenteuerlich, aber vertrauenswürdig, keine Extremsport-Ästhetik |
| Farbpalette | Forest green, slate grey, earthy tones |
| Bild-No-Gos | Kein Text im Bild, keine Logos, keine übertriebene Sättigung |

Aus diesem Briefing entsteht der Prompt:

```
Hiking backpack in forest green on autumn forest trail, earthy brown and grey tones, adventure lifestyle product photography, moody natural light, shallow depth of field --ar 1:1 --no text, logo, watermark, oversaturated
```

---

## 13.6 Bildwirkung: Was Kompositionsentscheidungen aussagen

Komposition ist keine rein ästhetische Entscheidung – sie kommuniziert.

| Komposition | Wirkung | Passend für |
|---|---|---|
| **Freie Mitte, viel Raum** | Ruhe, Klarheit, Luxus | LumaSkin, Premium-Produkte |
| **Viele Requisiten, volle Fläche** | Fülle, Wärme, Handwerk | BakeHaus, Lifestyle-Brands |
| **Person in Bewegung** | Energie, Dynamik | Waldwerk, Sport |
| **Nahaufnahme, kein Kontext** | Fokus, Qualität | Einzelprodukt-Feature |
| **Weite Szene, kleine Person** | Natur, Freiheit, Größe | Outdoor-Kampagne |

Wer den gewünschten **Effekt benennen** kann, kann ihn auch im Prompt formulieren.

---

## Kurzübungen

{{ task(file="tasks/tag13_01.yaml") }}

{{ task(file="tasks/tag13_02.yaml") }}

{{ task(file="tasks/tag13_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k13.yaml") }}

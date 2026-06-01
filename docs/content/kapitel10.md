# Kapitel 10 – Prompt-Aufbau für Bilder

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
  <div class="step active"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Das **MSLK-Modell** für strukturierte Bild-Prompts (Motiv, Szene, Look, Licht/Kamera)
- Wie **Negative Prompts** (`--no`) unerwünschte Elemente systematisch ausschließen
- Wie du aus einem schwachen Prompt Schritt für Schritt einen starken baust
- Welche Parameter den größten Einfluss auf das Ergebnis haben
- Wie derselbe Prompt für unterschiedliche Marken angepasst wird
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und teste die Beispiel-Prompts in Midjourney.
2. Bearbeite die **Kurzübungen** der Reihe nach.
3. Arbeite die **Workshop-Aufgabe** durch.

---

## 10.1 Das MSLK-Modell

Für Bild-Prompts eignet sich ein einfaches Raster – analog zum RCFT-Modell bei Texten aus Woche 1:

| Baustein | Bedeutung | Beispiel |
|---|---|---|
| **M – Motiv** | Was ist das Hauptobjekt? | fresh sourdough loaf, glass serum bottle, hiking backpack |
| **S – Szene** | Wo, welcher Kontext, was ist im Hintergrund? | rustic wooden bakery counter, clean marble bathroom shelf |
| **L – Look** | Stil, Medium, Ästhetik | editorial product photo, flat vector illustration, 3D render |
| **K – Kamera & Licht** | Perspektive, Lichtstimmung, Schärfentiefe | 45-degree angle, soft diffused daylight, shallow depth of field |

Nicht jeder Baustein muss in jedem Prompt enthalten sein. Aber: **Je konkreter die Beschreibung, desto weniger Zufall im Ergebnis.**

**Vollständiges Beispiel – BakeHaus (handwerkliche Bäckerei):**

```
Fresh artisan sourdough bread on rustic wooden board, cozy bakery interior blurred in background, warm editorial food photography, 45-degree angle, soft golden morning light, shallow depth of field --ar 4:5 --no text, logo, watermark
```

- **M:** Fresh artisan sourdough bread
- **S:** rustic wooden board, cozy bakery interior blurred in background
- **L:** warm editorial food photography
- **K:** 45-degree angle, soft golden morning light, shallow depth of field

---

## 10.2 MSLK für verschiedene Marken

Dasselbe Modell funktioniert für alle Marken – nur der Inhalt ändert sich:

**Nordkorn (Müsli) – Instagram 1:1:**
```
Organic granola in a white ceramic bowl on a light oak table, soft morning kitchen setting, minimalist food photography, overhead shot, gentle diffused natural light --ar 1:1 --no text, logo, clutter
```

**LumaSkin (Kosmetik) – Instagram 4:5:**
```
Matte white serum bottle on travertine stone slab, spa bathroom setting with soft towels in background, luxury beauty product photography, centered composition, soft diffused spa lighting --ar 4:5 --no text, logo, watermark
```

**Waldwerk (Outdoor) – LinkedIn 16:9:**
```
Hiking backpack and trail boots on weathered mountain rock, misty pine forest background, adventure lifestyle brand photography, wide shot with negative space left for text overlay, moody natural light --ar 16:9 --no text, logo, watermark
```

In allen drei Fällen: dieselbe MSLK-Struktur, andere Marken-Welt.

---

## 10.3 Negative Prompts (`--no`)

Mit `--no` werden Elemente **ausgeschlossen**, die Midjourney sonst gerne hinzufügt:

```
--no text, logo, watermark, blurry, distorted hands, extra fingers
```

**Standard-Set für Marketing-Bilder:**

```
--no text, logo, watermark
```

**Erweitert bei Produktfotos:**

```
--no text, logo, watermark, cluttered background, oversaturated, plastic look
```

**Bei Personenbildern:**

```
--no text, logo, distorted hands, extra fingers, deformed face, unrealistic proportions
```

!!! info "Wann `--no` ergänzen?"
    Nicht alle `--no`-Begriffe von Anfang an einbauen. Erst Ergebnis ansehen – dann gezielt ausschließen, was stört. So bleibt der Prompt lesbar und nachvollziehbar.

---

## 10.4 Schwacher vs. starker Prompt

| Version | Prompt |
|---|---|
| **Schwach** | `nice product photo of skincare` |
| **Besser** | `Skincare bottle on clean background, product photography` |
| **Stark** | `Minimalist product photo of a matte white skincare bottle on travertine stone, spa bathroom setting, soft diffused daylight, luxury beauty editorial style, centered composition --ar 4:5 --no text, logo, watermark` |

Der Unterschied liegt nicht in der Länge, sondern in der **Präzision**: konkrete Materialien, Licht, Komposition und Parameter – statt allgemeine Adjektive wie „schön" oder „professionell".

**Häufige Fehler bei schwachen Prompts:**

- Nur ein Adjektiv: `beautiful`, `nice`, `modern`
- Keine Szene: Midjourney erfindet einen beliebigen Kontext
- Kein Licht: Das Modell wählt oft dramatisches, unnatürliches Licht
- Kein `--no`: Text-Artefakte oder überfüllte Hintergründe

---

## 10.5 Die Reihenfolge im Prompt

Midjourney gewichtet **Begriffe am Anfang des Prompts stärker**. Die empfohlene Reihenfolge:

1. **Motiv** (Hauptobjekt zuerst)
2. **Szene / Kontext**
3. **Look / Stil**
4. **Licht / Kamera**
5. **Parameter** (immer am Ende: `--ar`, `--no`)

**Beispiel – falsche vs. richtige Reihenfolge:**

Ungünstig:
```
Soft morning light, minimalist photography, white bowl, granola --ar 1:1
```

Besser:
```
Organic granola in white ceramic bowl, soft morning light, minimalist food photography --ar 1:1 --no text
```

Das Motiv steht vorne – Midjourney fokussiert darauf.

---

## 10.6 Parameter im Überblick

| Parameter | Wirkung | Typischer Einsatz |
|---|---|---|
| `--ar 1:1` | Quadrat | Instagram-Feed |
| `--ar 4:5` | Hochformat | Instagram-Post |
| `--ar 9:16` | Story-Format | Instagram/TikTok Story |
| `--ar 16:9` | Querformat | LinkedIn-Banner, Website-Header |
| `--ar 3:1` | Sehr breit | Panorama-Banner |
| `--no …` | Ausschlüsse | Kein Text, kein Logo, keine Verzerrungen |

!!! tip "Immer `--ar` setzen"
    Ohne `--ar` liefert Midjourney ein Standardformat (meist quadratisch oder leicht querformat). Für Marketing-Bilder immer den Kanal vorher festlegen und den Parameter mitgeben.

---

## Kurzübungen

{{ task(file="tasks/tag10_01.yaml") }}

{{ task(file="tasks/tag10_02.yaml") }}

{{ task(file="tasks/tag10_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k10.yaml") }}

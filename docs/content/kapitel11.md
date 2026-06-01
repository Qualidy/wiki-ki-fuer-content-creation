# Kapitel 11 – Stile steuern

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
  <div class="step active"></div>
  <div class="step"></div>
  <div class="step"></div>
  <div class="step"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Unterschiede zwischen **Foto-, Illustrations- und 3D-Look** und wann welcher passt
- Wie du Stil, Stimmung und Ästhetik über konkrete Begriffe im Prompt steuerst
- Wie **Materialien und Texturen** das Markenbild prägen
- Wie **Kompositionsangaben** die Bildwirkung gezielt beeinflussen
- Wie **Stil-Referenzen** für einen konsistenten Marken-Look sorgen
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und erzeuge zu jedem Stilbeispiel mindestens eine Bildvariante in Midjourney.
2. Bearbeite die **Kurzübungen**.
3. Arbeite die **Workshop-Aufgabe** durch.

---

## 11.1 Stilkategorien – Überblick

Midjourney kann dasselbe Motiv in völlig unterschiedlichen visuellen Sprachen erzeugen. Die Wahl des Stils ist eine **strategische Entscheidung** – sie bestimmt, wie eine Marke wahrgenommen wird.

| Stilrichtung | Stichwörter im Prompt | Typischer Einsatz |
|---|---|---|
| **Realistisches Foto** | `product photography, photorealistic, shot on DSLR` | Shop, Website, LinkedIn |
| **Editorial / Lifestyle** | `editorial fashion photo, natural light, magazine style, candid` | Instagram, Kampagnen |
| **Flat Design / Illustration** | `flat vector illustration, bold colors, minimal shapes, clean lines` | Erklärposts, jüngere Zielgruppe |
| **3D-Render** | `3D render, octane render, soft shadows, clean background` | Tech, SaaS, Produkt-Mockups |
| **Aquarell / Kunstdruck** | `soft watercolor illustration, delicate brushstrokes, pastel tones` | Lifestyle, Handwerk, Gastronomie |

**Praxisregel:** Ein realistisches Produktfoto für den Online-Shop, ein Lifestyle-Bild für Instagram. Nicht beides mischen.

---

## 11.2 Stil über Wörter steuern

Midjourney reagiert stark auf **Stilbegriffe im Prompt**. Dieselbe Szene kann völlig unterschiedlich wirken – hier am Beispiel LumaSkin (Serum):

**Realistisches Produktfoto:**
```
Matte white skincare serum bottle on marble surface, soft spa lighting, luxury beauty product photography, sharp focus --ar 4:5 --no text, logo
```

**Flache Illustration:**
```
Flat vector illustration of a skincare serum bottle, pastel pink and cream palette, minimal geometric shapes, clean white background --ar 4:5 --no text, logo
```

**Aquarell:**
```
Soft watercolor illustration of a skincare serum bottle, delicate brushstrokes, blush pink tones, botanical elements, artisan beauty brand aesthetic --ar 4:5 --no text, logo
```

Das Motiv ist identisch – nur die Stilkategorie ändert sich. Für LumaSkin mit der Zielgruppe „vertrauenswürdig, sachlich" empfiehlt sich das reale Foto.

---

## 11.3 Realismus steuern

Midjourney hat einen eigenen ästhetischen Standard-Look – Bilder wirken oft makellos und etwas unwirklich. Für **vertrauenswürdige Marketing-Bilder** kann das kontraproduktiv sein.

**Realismus erhöhen:**
```
photorealistic, shot on Canon EOS R5, natural imperfections, authentic feel
```

**Weniger „KI-Glanz":**
```
--style raw
```
(reduziert Midjourneys automatische Verschönerung – Funktion je nach Interface-Version verfügbar)

**Bewusst künstlerischer Look** (für Kampagnen mit starker Bildsprache):
```
cinematic, dreamy, vibrant surreal, painterly
```

---

## 11.4 Materialien und Texturen

Konkrete Materialangaben verändern das Bild erheblich – und transportieren gleichzeitig **Markenwerte**:

| Material / Textur | Assoziationen | Markenbeispiel |
|---|---|---|
| `linen, natural cotton` | Nachhaltigkeit, Einfachheit | GreenLoop |
| `marble, travertine stone` | Luxus, Premium, Clean | LumaSkin |
| `rustic wood, terracotta` | Handwerk, Wärme, Tradition | BakeHaus |
| `weathered rock, pine wood` | Abenteuer, Natur, Outdoor | Waldwerk |
| `glass, brushed metal` | Tech, Modern, Professionell | FlowTask |

**Beispiel – GreenLoop:**
```
Organic cotton tote bag on natural linen tablecloth, dried eucalyptus sprig, soft daylight, sustainable fashion flat lay --ar 1:1 --no text, logo, plastic
```

Das Wort `plastic` im `--no`-Teil schließt billig wirkende Oberflächen aus – passend zur Nachhaltigkeits-Positionierung.

---

## 11.5 Kompositionsangaben

Komposition beeinflusst, **wo das Auge hingeht** und wie viel Freiraum für Text im Layout bleibt:

| Begriff | Wirkung |
|---|---|
| `centered composition` | Produkt mittig, ruhig, klar |
| `rule of thirds` | Motiv leicht versetzt, wirkt natürlicher |
| `flat lay` | Vogelperspektive, Produkt + Requisiten auf Fläche |
| `overhead shot` | Direkt von oben, Tabletop-Stil |
| `45-degree angle` | Leicht schräg, klassisch für Food und Produkt |
| `negative space at top` | Freiraum oben – Platz für Text-Overlay in Canva |
| `negative space on the left` | Freiraum links – für Querformat-Banner mit Text |

**Wann Freiraum planen?**  
Immer dann, wenn später in Canva oder PowerPoint **Text auf das Bild** kommt. Das ist der normale Workflow: Midjourney liefert das Bild ohne Text, das Layout-Tool fügt Headline und Caption hinzu.

```
Product centered with generous negative space at top and bottom, clean white background --ar 1:1
```

---

## 11.6 Farben und Stimmung

Farben gehören **direkt in den Prompt** – nicht nur als einzelne Farbnamen, sondern als Palette und Stimmungsbeschreibung:

**Zu schwach:**
```
green color, natural product photo
```

**Konkret und wirkungsvoll:**
```
sage green and warm cream color palette, muted earth tones, calm and unhurried mood, Scandinavian minimalism
```

**Farbpaletten der Kursmarken:**

| Marke | Palette im Prompt |
|---|---|
| **GreenLoop** | `sage green, cream, warm linen tones, muted earth palette` |
| **Nordkorn** | `oat beige, warm white, honey tones, morning light warmth` |
| **LumaSkin** | `soft rose, clean white, light grey, minimal and trustworthy` |
| **BakeHaus** | `golden brown, terracotta, warm amber, rustic warmth` |
| **Waldwerk** | `forest green, slate grey, dark navy, earthy and rugged` |
| **FlowTask** | `cool white, light blue-grey, clean and modern, professional` |

---

## 11.7 Stil-Referenz

Wenn ein Bild den gewünschten Marken-Look trifft, lässt sich dieser Look für **weitere Motive** wiederverwenden – über eine **Stil-Referenz**.

**Vorgehen im Web-Interface:**

1. Ein Referenzbild erzeugen, das Farben und Stimmung der Marke trifft
2. Das Bild im Interface als **Style Reference** auswählen (oder URL mit `--sref` hinterlegen)
3. Neue Prompts mit dieser Referenz ausführen
4. Vergleichen: Wirken die Bilder wie eine Serie?

!!! info "Marke GreenLoop – Referenz-Look"
    Gedämpfte Naturtöne, Leinen-Texturen, weiches Tageslicht, wenig Kontrast. Das Referenzbild entsteht einmal – danach können Flat Lays, Detail-Aufnahmen und Lifestyle-Bilder alle im gleichen Look produziert werden.

Die Stil-Referenz ist das Bild-Äquivalent zum **Persona-Block** aus Woche 1: einmal definiert, immer wieder anwendbar.

---

## Kurzübungen

{{ task(file="tasks/tag11_01.yaml") }}

{{ task(file="tasks/tag11_02.yaml") }}

{{ task(file="tasks/tag11_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k11.yaml") }}

# Kapitel 14 – Konsistenz und Bild-Workflow

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
  <div class="step done"></div>
  <div class="step active"></div>
</div>

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was Bildkonsistenz bedeutet und warum sie für Marken entscheidend ist
- Wie du eine **Bildserie** planst und mit Stil-Referenz umsetzt
- Wie Prompts **dokumentiert** werden, damit Motive nachproduziert werden können
- Wie der vollständige Workflow von Briefing bis Veröffentlichung aussieht
- Wie KI-Bildgenerierung in den **Berufsalltag** im Content-Marketing eingebettet ist
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und nutze die fiktive Marke **GreenLoop** als roten Faden.
2. Bearbeite die **Kurzübungen**.
3. Arbeite die **Workshop-Aufgabe** als Abschluss der Midjourney-Woche durch.

---

## 14.1 Was Bildkonsistenz bedeutet

Ein einzelnes starkes Bild reicht nicht – im Marketing zählt die **visuelle Kohärenz über alle Inhalte hinweg**. Bilder, die auf den ersten Blick zusammengehören, stärken die Markenwahrnehmung. Bilder, die stilistisch springen, wirken unprofessionell – selbst wenn jedes einzelne gut aussieht.

**Konsistenz entsteht durch:**

- Gleiche **Farbpalette** in allen Bildern
- Gleiches **Lichtverhältnis** (warm/kalt, hart/weich)
- Gleiche **Stilkategorie** (Foto, Illustration oder 3D – nicht gemischt)
- Gleiche **Kompositionslogik** (Flat Lay für alle, oder Editorial für alle)
- Gleicher **Freiraum** für Text-Overlays (immer oben, oder immer links)

Ohne Planung entsteht Konsistenz nur zufällig – mit einer **Stil-Referenz** und einem festen Prompt-Raster entsteht sie systematisch.

---

## 14.2 Bildreihen planen

Vor dem Prompten kommt die **inhaltliche Planung**. Für eine Mini-Kampagne reichen 3–5 Motive:

| Motiv-Typ | Funktion | Format |
|---|---|---|
| **Hero-Bild** | Hauptprodukt im Fokus, repräsentiert die Kampagne | 1:1 oder 4:5 |
| **Detail-Bild** | Material, Textur, Qualitätsmerkmal | 1:1 |
| **Lifestyle-Bild** | Produkt im Alltag, Emotion, Zielgruppe | 4:5 |
| **Saisonaler Kontext** | Frühling, Herbst, besonderer Anlass | 1:1 oder 4:5 |
| **Story-Format** | Vertikales Bild für Story oder Reels-Cover | 9:16 |

**Vorgehen:**

1. Motive in Stichpunkten planen (deutsch reicht)
2. Pro Motiv: MSLK notieren
3. Englische Prompts formulieren
4. Nacheinander in Midjourney erzeugen – nicht gleichzeitig
5. Nach jedem Bild: Konsistenz zur bisherigen Serie prüfen

---

## 14.3 Stil-Referenz als roter Faden

Ohne Stil-Referenz schwankt der Look zwischen den Motiven. Mit Stil-Referenz bleibt die visuelle Sprache stabil.

**Workflow:**

1. **Erstes Bild = Referenzbild** – muss Farbpalette, Licht und Stimmung der Marke treffen
2. **Upscalen** und als Referenz markieren (im Web-Interface oder URL für `--sref`)
3. Alle weiteren Bilder mit dieser Referenz prompten
4. Ergebnisse nebeneinander vergleichen

**Beispiel – GreenLoop:**

Referenzbild-Prompt:
```
Organic cotton sweater in sage green folded on natural linen, dried botanicals, soft window light, minimalist flat lay, Scandinavian sustainable fashion brand aesthetic --ar 1:1 --no text, logo
```

Zweites Motiv (Tote Bag) – gleiche Referenz:
```
Natural cotton tote bag on linen cloth, dried eucalyptus, same soft window light, minimalist flat lay, same Scandinavian aesthetic --ar 1:1 --no text, logo
```

Wenn die Stil-Referenz aktiv ist, übernimmt Midjourney die Farbtemperatur und Lichtstimmung automatisch – beide Bilder wirken wie aus einer Produktion.

---

## 14.4 Prompts dokumentieren

In der Praxis werden Bildkampagnen nicht einmalig erzeugt – Motive werden **nachproduziert**, wenn Produkte oder Formate wechseln. Ohne Dokumentation ist das Nachstellen Glückssache.

**Was pro finalem Bild festgehalten wird:**

| Feld | Inhalt |
|---|---|
| Datum / Version | z. B. „GreenLoop_SS26_Hero_v2" |
| Vollständiger Prompt | englisch, inkl. aller Parameter |
| Stil-Referenz | Ja/Nein – welches Bild |
| Variante | U1–U4 + Vary-Schritte |
| Kanal & Format | z. B. Instagram 1:1 |
| Dateiname | z. B. `greenloop-hero-sweater-1zu1.png` |

**Hilfreich:** Eine einfache Tabelle in Word oder Notion reicht. Das ist keine akademische Übung – es ist eine Gewohnheit, die professionelle Arbeit von improvisierten Ergebnissen unterscheidet.

---

## 14.5 Der vollständige Workflow

Zusammenfassung des Midjourney-Workflows von der Idee bis zur Veröffentlichung:

```
1. Briefing klären
   → Marke, Kanal, Motiv, Stimmung, No-Gos

2. MSLK notieren
   → Motiv, Szene, Look, Kamera/Licht (auf Deutsch)

3. Englischen Prompt formulieren
   → MSLK als Fließtext + Parameter (--ar, --no)

4. Midjourney ausführen
   → Vier Varianten sichten, beste auswählen

5. Verfeinern (wenn nötig)
   → Vary Subtle / Strong oder Prompt anpassen

6. Upscale + Export
   → Datei mit klarem Namen speichern

7. Text in Copilot
   → Caption, Headline, CTA passend zum Bild

8. Zusammenführen in Layout-Tool
   → Canva, Figma oder PowerPoint

9. Qualitätskontrolle
   → Text korrekt? Bild ohne Artefakte? Ton stimmig?
```

---

## 14.6 KI-Bilder im Berufsalltag

Midjourney ist kein Ersatz für professionelle Fotografie – aber es verändert, **wer ohne Fotostudio visuellen Content produzieren kann**.

**In Agenturen und Marketing-Teams wird KI-Bildgenerierung eingesetzt für:**

- Mood Boards und Konzeptvisualisierungen (bevor ein Fotoshooting genehmigt wird)
- Hintergrundbilder und Texturen für Layouts
- Social-Media-Bilder mit schnellem Turnaround
- Testbilder für A/B-Tests
- Content für kleine Budgets ohne Fotoproduktion

**Als Umschüler in einer Content-Rolle ist es wichtig zu verstehen:**

- Midjourney erzeugt Rohmaterial – die Bearbeitung (Layout, Text, Qualitätskontrolle) liegt weiter beim Menschen
- KI-generierte Bilder sind **nicht automatisch lizenzfrei** – Nutzungsrechte abhängig vom Abo-Modell prüfen
- In regulierten Branchen (Pharma, Finanzen, Lebensmittel) gelten besondere Regeln für Bildaussagen

---

## 14.7 Abschluss-Checkliste: Midjourney-Woche

Vor dem Abschluss prüfen:

- [ ] Ich kann einen vollständigen MSLK-Prompt auf Englisch formulieren
- [ ] Ich weiß, welches `--ar` für welchen Kanal sinnvoll ist
- [ ] Ich setze `--no text, logo, watermark` konsequent ein
- [ ] Ich kann aus vier Varianten eine begründet auswählen
- [ ] Ich verwende Vary sparsam und entscheide, wann ein neuer Prompt besser ist
- [ ] Ich habe mindestens einen Prompt vollständig dokumentiert
- [ ] Ich kenne den Drei-Schritt-Workflow: Midjourney → Copilot → Layout-Tool

---

## Kurzübungen

{{ task(file="tasks/tag14_01.yaml") }}

{{ task(file="tasks/tag14_02.yaml") }}

{{ task(file="tasks/tag14_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k14.yaml") }}

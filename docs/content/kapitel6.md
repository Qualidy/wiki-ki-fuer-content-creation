# Kapitel 6 – Prompts aufbauen und iterativ verbessern

<div class="kurs-progress">
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

- Prompts schrittweise aufbauen statt alles auf einmal zu formulieren
- Mit **Folgeprompts** ein Ergebnis gezielt weiterentwickeln
- Unerwünschte Inhalte durch explizite Verbote aus dem Ergebnis ausschließen
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und probiere die Beispiele in Copilot aus.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 6.1 Iteratives Prompten

Ein einzelner Prompt liefert selten ein fertiges Ergebnis – das ist strukturell bedingt und kein Zeichen für einen Fehler. Gute Texte entstehen durch Überarbeitung, und genauso entstehen gute KI-Texte durch mehrere aufeinander aufbauende Prompts.

Ein typischer iterativer Ablauf:

```
Groben Entwurf anfordern
      ↓
Einzelne Abschnitte vertiefen
      ↓
Ton und Länge anpassen
      ↓
Varianten vergleichen
```

Jeder Schritt erfordert wenig Aufwand. Das Gesamtergebnis ist deutlich präziser als bei einem einzigen umfassenden Auftrag.

---

## 6.2 Folgeprompts einsetzen

Copilot und ChatGPT merken sich alle Eingaben und Antworten innerhalb eines Gesprächs. Folgeprompts können daher direkt auf das vorherige Ergebnis Bezug nehmen, ohne den Ausgangstext erneut einzugeben.

**Typische Folgeprompts nach einem ersten Entwurf:**

| Ziel | Formulierung |
|---|---|
| Text kürzen | „Kürze den Text auf 80 Wörter. Die Kernaussage bleibt erhalten." |
| Ton ändern | „Formuliere sachlicher. Keine Ausrufezeichen, keine wertenden Adjektive." |
| Ergänzung einfügen | „Füge nach dem zweiten Absatz ein konkretes Beispiel aus dem Berufsalltag ein." |
| Alternative formulierungen | „Schlage drei alternative Formulierungen für den ersten Satz vor." |
| Kanal wechseln | „Überführe den Text in einen LinkedIn-Post. Maximal 900 Zeichen, Sie-Form." |

!!! tip "Ein Ziel pro Folgeprompt"
    Werden mehrere Überarbeitungsziele gleichzeitig formuliert, nimmt die Genauigkeit des Ergebnisses ab. Effektiver ist es, die Schritte nacheinander abzuarbeiten.

---

## 6.3 Negative Anweisungen

Eine häufig unterschätzte Technik: Das Modell kann explizit angewiesen werden, bestimmte Inhalte, Formulierungen oder Begriffe zu vermeiden.

Das Modell kennt weder den Stilguide einer Marke noch branchenspezifische Compliance-Anforderungen. Diese müssen im Prompt mitgeteilt werden:

- „Keine Superlative wie ‚beste', ‚einzigartig', ‚revolutionär'."
- „Keine erfundenen Studien oder Prozentangaben."
- „Keine Nennung von Mitbewerbern."
- „Kein Emoji."
- „Keine Gesundheitsversprechen."

Was in einem Redaktionsbriefing als No-Go vermerkt würde, gehört auch in den Prompt.

---

## 6.4 Praxisbeispiel: ein Blogartikel-Abschnitt in drei Prompts

**Prompt 1 – Gliederung:**
> Erstelle eine Gliederung für einen Blogartikel zum Thema „Nachhaltige Verpackungen im Online-Handel". Drei Abschnitte mit Überschriften, Zielgruppe: Shop-Betreibende, Du-Form. Kein Fazit.

**Prompt 2 – Abschnitt ausschreiben:**
> Schreib jetzt den zweiten Abschnitt aus der Gliederung. Ca. 200 Wörter, ein konkretes Beispiel aus dem Alltag eines Online-Shops.

**Prompt 3 – Überarbeitung:**
> Kürze den Abschnitt auf 150 Wörter. Entferne Füllwörter wie „natürlich" und „selbstverständlich". Ton beibehalten.

Das Ergebnis nach drei Prompts ist ein überarbeiteter, verwendbarer Textentwurf.

---

## 6.5 Stil durch Beispiele vorgeben

Wenn eine bestimmte Markenstimme schwer in Worte zu fassen ist, kann sie durch Beispiele vermittelt werden:

> Unser Content klingt normalerweise so: „Montag, und du hast schon drei Dinge erledigt? Respekt." und „Ideen kommen morgens um 3 Uhr. Gut, dass du sie irgendwo festhalten kannst." Schreib in diesem Stil einen Beitrag über unsere neue Notiz-App.

Diese Technik eignet sich besonders, wenn ein eigener Stil existiert, der durch abstrakte Beschreibungen nur unzureichend erfasst wird.

---

## Kurzübungen

{{ task(file="tasks/tag4_01.yaml") }}

{{ task(file="tasks/tag4_02.yaml") }}

{{ task(file="tasks/tag4_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k6.yaml") }}

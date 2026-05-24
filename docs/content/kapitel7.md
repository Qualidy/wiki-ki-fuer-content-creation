# Kapitel 7 – Prompts für Blog, Social Media und Newsletter

<div class="kurs-progress">
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

- Prompts kanalspezifisch ausrichten – was Blog, LinkedIn, Instagram und Newsletter unterscheidet
- Eine Zielgruppe im Prompt so beschreiben, dass das Ergebnis konkret wird
- Ton und Markenstimme steuern, damit KI-Texte zur jeweiligen Marke passen
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und probiere die Beispiele in Copilot aus.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 7.1 Kanalspezifische Anforderungen

KI-Modelle passen Stil und Format des Ergebnisses nicht automatisch an den Kanal an. Diese Informationen müssen im Prompt mitgegeben werden – sonst entsteht ein Text, der für keinen Kanal wirklich geeignet ist.

### Blog & Website

- Länge in Wörtern angeben
- Abschnittsstruktur mit Überschriften vorgeben oder anfordern
- Festlegen, ob ein Fazit gewünscht ist

**Beispiel-Prompt:**
> Du bist Redakteur für ein Fintech-Unternehmen. Schreib Abschnitt 2 eines Blogartikels über digitales Kontoführen. Ca. 250 Wörter, ein konkretes Alltagsbeispiel, Sie-Form. Keine Fachbegriffe ohne Erklärung.

---

### LinkedIn

- Zeichengrenze beachten: Die ersten ca. 150 Zeichen sind vor dem „Mehr lesen"-Abschnitt sichtbar.
- Einstieg (Hook) in der ersten Zeile
- Klarer Call-to-Action am Ende
- Maximal 3–5 Hashtags

**Beispiel-Prompt:**
> Schreib einen LinkedIn-Post über unsere neue Funktion zur Rechnungsautomatisierung. Zielgruppe: Buchhaltungsleiter in KMU. Die erste Zeile soll Interesse wecken – keine Floskel. Max. 900 Zeichen. CTA: „Mehr dazu in den Kommentaren." 3 Hashtags.

---

### Instagram

- Kürzer und emotionaler als LinkedIn
- Du-Form in den meisten Fällen passender als Sie
- Emojis nur wenn zum Markenstil passend
- Hashtags: bis zu 10, nur thematisch relevante

**Beispiel-Prompt:**
> Schreib eine Instagram-Caption für ein Produktfoto unseres neuen Snacks. Zielgruppe: Berufstätige 25–35 Jahre. Locker, Du-Form, ein Emoji am Ende. Max. 80 Wörter, 5 Hashtags.

---

### Newsletter

Betreffzeile, Preheader und Teaser sind drei eigenständige Textelemente, die im Posteingang gleichzeitig sichtbar sind:

| Element | Bedeutung | Empfohlene Länge |
|---|---|---|
| **Betreffzeile** | Entscheidet über die Öffnungsrate | Max. 50 Zeichen |
| **Preheader** | Vorschautext im E-Mail-Client | Max. 90 Zeichen |
| **Teaser** | Einstieg im Newsletter-Body | 2–4 Sätze |

**Beispiel-Prompt:**
> Für einen Newsletter über unsere Sommerkampagne werden benötigt: eine Betreffzeile (max. 50 Zeichen), ein Preheader (max. 90 Zeichen) und ein 3-Satz-Teaser. Ton: direkt und einladend.

---

## 7.2 Zielgruppe präzise beschreiben

„Zielgruppe: alle" ergibt im Prompt keine verwendbare Vorgabe. Ohne Konkretisierung schreibt das Modell für ein nicht definiertes Durchschnittspublikum.

Bereits ein präziser Satz verbessert das Ergebnis deutlich:

> Zielgruppe: Eltern mit Kindern unter 10 Jahren, geringer Zeitpuffer, suchen pragmatische Lösungen.

Oder ausführlicher:

> Zielgruppe: Marketingleiter in mittelständischen Unternehmen (50–200 Mitarbeitende). Berufserfahren, unter Zeitdruck, skeptisch gegenüber KI-Hype. Erwarten konkrete Anwendungsfälle statt Theorie.

Sinnvolle Angaben zur Zielgruppe umfassen: Rolle oder Beruf, Erwartungen und Bedürfnisse, typische Einwände oder Hindernisse, bevorzugte Ansprache (Du/Sie, Fachsprache ja/nein).

---

## 7.3 Ton und Markenstimme steuern

Copilot und ChatGPT kennen keine Markenstimme. Sie müssen durch explizite Angaben im Prompt informiert werden.

**Tonalität beschreiben:**
> Ton: kompetent, aber nicht arrogant. Kurze Sätze. Aktiv statt passiv. Keine Superlative.

**Verbotene Begriffe:**
> Vermeiden: „revolutionär", „einzigartig", „zukunftsweisend", „nahtlos".

**Stil durch Beispiel vermitteln:**
> Unser Stil klingt so: „Drei Stunden täglich verschwinden im Reporting – ohne erkennbares Ergebnis." Schreib in diesem Stil über unsere neue Rechnungsautomatisierung.

Wenn ein Stilguide vorhanden ist, lassen sich die drei bis fünf wichtigsten Regeln direkt in den Kontext-Teil des Prompts integrieren.

---

## 7.4 Multi-Format aus einer Kernbotschaft

Eine inhaltlich geprüfte Kernbotschaft lässt sich in einem Prompt für mehrere Kanäle gleichzeitig aufbereiten:

> Kernbotschaft: Unser Bestellprozess ist jetzt in drei Schritten abgeschlossen – ohne Account-Erstellung.
>
> Erstelle daraus:  
> 1) LinkedIn-Post (max. 800 Zeichen, Sie-Form, CTA: „Jetzt testen")  
> 2) Instagram-Caption (max. 80 Wörter, Du-Form, 1 Emoji, 3 Hashtags)  
> 3) Newsletter-Teaser (2 Sätze, einladend)  
>
> Gleiche Kernaussage in allen drei Formaten. Keine weiteren Zahlenangaben außer den drei Schritten.

---

## Kurzübungen

{{ task(file="tasks/tag4_04.yaml") }}

{{ task(file="tasks/tag4_05.yaml") }}

{{ task(file="tasks/tag5_01.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k7.yaml") }}

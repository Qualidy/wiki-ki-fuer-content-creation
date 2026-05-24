# Kapitel 5 – Was ist ein guter Prompt?

<div class="kurs-progress">
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

- Was einen guten von einem schwachen Prompt unterscheidet
- Das **RCFT-Modell** als strukturiertes Hilfsmittel für Content-Prompts
- Wie das Modell flexibel eingesetzt wird – situationsabhängig, nicht schematisch
</div>

---

## So gehst du vor

1. Lies die Kapitelinhalte und probiere die Beispiele in Copilot aus.
2. Bearbeite die **Kurzübungen** der Reihe nach – von Grundlagen bis Experte.
3. Arbeite die **Workshop-Aufgabe** durch. Sie vertieft das Gelernte an einem zusammenhängenden Szenario.

---

## 5.1 Was ist ein Prompt?

Als Prompt bezeichnet man die Eingabe, die an eine KI gerichtet wird. Jeder Text, der in Copilot oder ChatGPT eingegeben wird, ist ein Prompt – ob als Frage, Auftrag oder Stichpunkt.

Die Qualität des Prompts bestimmt maßgeblich die Qualität des Ergebnisses. Beide folgenden Anfragen haben dasselbe Ziel – liefern aber sehr unterschiedliche Ergebnisse:

❌ „Kannst du etwas zu unserem neuen Produkt schreiben?"

✅ „Schreib eine kurze Einleitung für unseren Newsletter. Thema: unser neues Treueprogramm. Zielgruppe: Stammkunden. Ton: freundlich und persönlich. Maximal 80 Wörter."

Der Unterschied liegt nicht im Aufwand, sondern in der Präzision der Anweisung.

---

## 5.2 Warum fehlende Vorgaben zu generischen Ergebnissen führen

Sprachmodelle füllen unspezifische Prompts mit statistisch wahrscheinlichem Material. Fehlt die Zielgruppe, wird für ein allgemeines Publikum geschrieben. Fehlt der Ton, wird ein neutraler Mittelweg gewählt. Fehlt das Format, erfindet das Modell eine Struktur.

Das Ergebnis ist formal korrekt, inhaltlich aber nichtssagend – weil keine konkreten Vorgaben vorhanden waren, auf die sich die KI stützen konnte.

---

## 5.3 Das RCFT-Modell

Das RCFT-Modell bietet eine strukturierte Orientierung beim Aufbau von Content-Prompts. Es besteht aus vier Elementen:

| Kürzel | Bedeutung | Leitfrage |
|:---:|---|---|
| **R** | Rolle | Welche Perspektive soll die KI einnehmen? |
| **C** | Kontext | Welche inhaltlichen Informationen braucht die KI? |
| **F** | Format | Wie soll das Ergebnis aussehen? |
| **T** | Task | Was soll die KI konkret tun? |

### Beispiel – alle vier Elemente

> **R:** Du bist Redakteur für ein nachhaltig orientiertes Modeunternehmen.  
> **C:** Es wird eine neue Linie aus recyceltem Material eingeführt. Zielgruppe: Frauen 25–40, kaufen lieber hochwertig als viel. Verboten: Begriffe wie „günstig" oder Preisangaben.  
> **T:** Schreib eine Instagram-Caption für den Produkt-Launch.  
> **F:** Maximal 120 Wörter. Du-Form. CTA am Ende: „Jetzt entdecken." Bis zu 5 Hashtags.

Ein solcher Prompt lässt sich schnell formulieren – das Ergebnis ist deutlich präziser als bei einer kurzen Anweisung ohne Kontext.

---

## 5.4 Flexible Anwendung

Das RCFT-Modell ist ein Hilfsmittel, kein Pflichtformular. Nicht jede Aufgabe erfordert alle vier Elemente. Manchmal reichen Zielgruppe und Format. Manchmal ist die Rolle offensichtlich und muss nicht formuliert werden.

Mit zunehmender Erfahrung entwickelt sich ein Gespür dafür, welche Bestandteile für welche Aufgabe tatsächlich relevant sind.

---

## Kurzübungen

{{ task(file="tasks/tag3_03.yaml") }}

{{ task(file="tasks/tag3_04.yaml") }}

{{ task(file="tasks/tag3_05.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k5.yaml") }}

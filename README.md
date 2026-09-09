# Psyche und Geist

Fachblog von **Christoph Lange** – Psychoonkologe (DKG), Krankenhausseelsorger.

Für Fachkolleginnen und -kollegen aus Psychoonkologie, Psychologie und Onkologie: aktuelle Forschung, Reflexionen aus dem klinischen Alltag und ein evidenznaher Blick auf Glaube und Spiritualität als Ressource der Krankheitsverarbeitung. Mit eigenem Bereich für Betroffene.

---

## Aufbau

| Datei | Inhalt |
|---|---|
| `index.html` | **Die komplette Website.** Eine einzige, in sich geschlossene Datei – HTML, CSS, Inhalte, Schriften, Logo und Porträtfoto sind eingebettet. Keine externen Abhängigkeiten, kein Build-Schritt. |
| `404.html` | Fehlerseite für nicht gefundene Adressen. |
| `.nojekyll` | Schaltet die Jekyll-Verarbeitung auf GitHub Pages ab; die Dateien werden unverändert ausgeliefert. |

## Lokal ansehen

`index.html` per Doppelklick im Browser öffnen. Mehr ist nicht nötig.

## Technische Eckdaten

- **Single-Page-Anwendung** ohne Framework: Alle Bereiche sind `<main class="page">`-Blöcke, die Funktion `go('seitenname')` blendet sie um.
- **Beiträge** liegen im JavaScript-Array `posts` (Felder: `id`, `rubrik`, `tag`, `tagClass`, `datum`, `lesezeit`, `titel`, `teaser`, `inhalt`). Neue Beiträge **am Anfang des Arrays** ergänzen – die Startseite zeigt `forschung[0]` als hervorgehobenen Beitrag, ein Anhängen am Ende würde ihn unter ältere Beiträge sortieren.
- **Rubriken:** `aktuelles` (wird als „Forschung“ angezeigt), `praxis`, `spiritual`.
- **Datenschutz:** keine Cookies, kein Tracking, keine externen Ressourcen, keine Netzwerkaufrufe. Schriften (Instrument Serif / Instrument Sans, SIL OFL 1.1) sind lokal als Base64-WOFF2 eingebettet.
- **Sicherheit:** Content-Security-Policy als Meta-Tag, alle externen Links mit `rel="noopener"`, ausschließlich HTTPS.
- **Responsiv** getestet für Desktop, Tablet und Smartphone.

## Wichtig bei Änderungen

Die Inhalte werden vollständig zur Laufzeit aus dem `posts`-Array aufgebaut. Ein Syntaxfehler im JavaScript führt deshalb nicht zu einem fehlerhaften Beitrag, sondern zu einer **leeren Seite**. Vor jedem Push gilt daher:

1. `index.html` lokal im Browser öffnen und prüfen, ob alle Rubriken Beiträge anzeigen.
2. Erst danach committen und pushen.

Für Besucher ohne aktiviertes JavaScript enthält die Seite einen `<noscript>`-Hinweis mit Kontakt- und Krisennummern.

## Redaktionelle Grundsätze

- Alle fachlichen Aussagen sind gegen Primärquellen belegt. Keine erfundenen Studien, Zahlen, Zitate oder Fallgeschichten.
- Deutschsprachige Quellen (S3-Leitlinien, AWMF, DKFZ, Deutsche Krebsgesellschaft) haben Vorrang, ergänzt um internationale Primärliteratur.
- Jeder Beitrag schließt mit einem Quellenblock (`div.quellen`).
- Klinische Rolle und Seelsorgerolle bleiben inhaltlich getrennt; Spiritual Care wird als Ressourcenperspektive dargestellt, nicht als Verkündigung.

## Hosting über GitHub Pages

Repository → **Settings** → **Pages** → unter *Source* den Branch `main` und den Ordner `/ (root)` wählen. Nach wenigen Minuten ist die Seite unter `https://pee111.github.io/psychoonkologie-und-glaube/` erreichbar. Eine eigene Domain lässt sich dort ebenfalls hinterlegen.

> Impressum und Datenschutzerklärung wurden nach bestem Wissen erstellt, sind jedoch keine Rechtsberatung. Eine anwaltliche Prüfung wird empfohlen.

---

© 2026 Christoph Lange. Inhalte urheberrechtlich geschützt. Schriftarten unter SIL Open Font License 1.1.

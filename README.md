# Psychoonkologie & Spiritual Care

Fachblog von **Christoph Lange** – Psychoonkologe (DKG), Krankenhausseelsorger.

Für Fachkolleginnen und -kollegen aus Psychoonkologie, Psychologie und Onkologie: aktuelle Forschung, Reflexionen aus dem klinischen Alltag und ein evidenznaher Blick auf Glaube und Spiritualität als Ressource der Krankheitsverarbeitung. Mit eigenem Bereich für Betroffene.

---

## Aufbau

| Datei | Inhalt |
|---|---|
| `index.html` | **Die komplette Website.** Eine einzige, in sich geschlossene Datei – HTML, CSS, Inhalte, Schriften, Logo und Porträtfoto sind eingebettet. Keine externen Abhängigkeiten, kein Build-Schritt. |
| `UEBERGABE-Projektstand.md` | Vollständiger Projektkontext: Entscheidungen, Struktur, Quellen, offene Punkte. |
| `START-HIER.md` | Startprompt für eine neue Cowork-Sitzung. |
| `assets/` | Originaldateien von Porträtfoto und Logo (in `index.html` bereits in Webgröße eingebettet). |

## Lokal ansehen

`index.html` per Doppelklick im Browser öffnen. Mehr ist nicht nötig.

## Technische Eckdaten

- **Single-Page-Anwendung** ohne Framework: Alle Bereiche sind `<main class="page">`-Blöcke, die Funktion `go('seitenname')` blendet sie um.
- **Beiträge** liegen im JavaScript-Array `posts` am Dateiende (Felder: `id`, `rubrik`, `tag`, `tagClass`, `datum`, `lesezeit`, `titel`, `teaser`, `inhalt`). Neue Beiträge als weiteres Objekt ergänzen – Übersichtslisten und Artikelansicht bauen sich automatisch auf.
- **Rubriken:** `aktuelles` (Forschung), `praxis`, `spiritual` (Spiritual Care).
- **Datenschutz:** keine Cookies, kein Tracking, keine externen Ressourcen. Schriften (Instrument Serif / Instrument Sans, SIL OFL 1.1) sind lokal als Base64-WOFF2 eingebettet.
- **Responsiv** getestet für Desktop, Tablet und Smartphone.

## Vor der Veröffentlichung

Drei Platzhalter sind noch zu füllen – in `index.html` gelb hervorgehoben (CSS-Klasse `.placeholder`):

1. Private Anschrift im Impressum
2. E-Mail-Adresse (zwei Stellen: Kontaktbox und Impressum)
3. Hosting-Anbieter in der Datenschutzerklärung

Details und Begründungen stehen in `UEBERGABE-Projektstand.md`.

> Impressum und Datenschutzerklärung wurden nach bestem Wissen erstellt, sind jedoch keine Rechtsberatung. Eine anwaltliche Prüfung vor dem Livegang wird empfohlen.

## Hosting über GitHub Pages (optional)

Repository → **Settings** → **Pages** → unter *Source* den Branch `main` und den Ordner `/ (root)` wählen. Nach wenigen Minuten ist die Seite unter `https://<benutzername>.github.io/<repository>/` erreichbar. Eine eigene Domain lässt sich dort ebenfalls hinterlegen.

---

© 2026 Christoph Lange. Inhalte urheberrechtlich geschützt. Schriftarten unter SIL Open Font License 1.1.

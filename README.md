# Craniosacral Praxis Johann von Arb

Website der Craniosacral-Praxis von Johann von Arb in Fulenbach, Solothurn.

**Live:** https://f5yct67kcv-source.github.io/webseite-johann-vonarb/

## Aufbau

Statisches HTML, kein Framework, keine Abhängigkeiten, kein Build-Schritt.

- `index.html` – die ganze Startseite, CSS liegt inline im Dokument
- `impressum.html`, `datenschutz.html` – Rechtsseiten, teilen sich `assets/seite.css`
- `assets/fonts/` – Marcellus und Schibsted Grotesk, lokal eingebunden
- `assets/img/og.jpg` – Vorschaubild fürs Teilen, aus der Seite selbst gesetzt

Keine Cookies, keine Analyse-Werkzeuge, keine Aufrufe an fremde Server.

## Lokal ansehen

```bash
python3 -m http.server 8741
```

Dann http://localhost:8741 öffnen.

## Deployment

GitHub Pages liefert direkt aus dem `main`-Branch aus. Jeder Push ist nach ein bis zwei Minuten live.

## Bei einem Domainwechsel

Die Adresse steht an drei Stellen und muss überall gleich lauten:

1. `index.html` – `canonical`, `og:url`, `og:image` und die beiden JSON-LD-Blöcke
2. `sitemap.xml`
3. `robots.txt`

Läuft die Seite künftig bei einem Schweizer Anbieter, gehört ausserdem der Abschnitt zu den Server-Protokollen in `datenschutz.html` angepasst. Die Passage zur Bekanntgabe in die USA entfällt dann.

## Offen

- Alle Bilder fehlen: gebraucht werden ein Porträt von Johann und Aufnahmen aus der Praxis. Bis dahin kommt die Seite bewusst ohne Fotos aus.
- Tarife stehen nirgends. Die Kostenfrage wird im Fragenteil beantwortet, ohne Zahl.
- Ausbildung, Berufsverband und Kassenzulassung fehlen, solange sie nicht bestätigt sind.
- Der Text «Über mich» ist allgemein formuliert und sollte in Johanns eigenen Worten kommen.
- Keine Zeitangaben auf der Seite, weil eine Sitzung unterschiedlich lang dauert. Bitte nicht nachträglich einsetzen.

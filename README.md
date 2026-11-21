# Imkerverein Luisenburg e.V. – neue Website

Neue Website des Imkervereins Luisenburg e.V. – im gleichen Designsystem wie rutoso.de und sonneborns.de,
in den Vereinsfarben Braun und Honig. Reines HTML/CSS: kein Baukasten, keine Datenbank, keine Cookies,
kein Google Analytics, keine Schriften von fremden Servern.

## Seiten

Alle bisherigen Dateinamen bleiben gleich, alte Links funktionieren also weiter.

| Datei | Inhalt |
|---|---|
| `index.html` | Start / Über den Verein |
| `aktuelles.html` | Aktuelles |
| `termine.html` | Termine |
| `pressestimmen.html` | Pressestimmen |
| `sperrgebiete.html` | Bienengesundheit |
| `imkerstand.html` | Bienenstand |
| `vereinsheim.html` | Vereinsheim und Verleih |
| `mitglied-werden.html` | Mitglied werden, Beitrag, Formulare |
| `satzung.html` | Satzung |
| `kontakt.html` | Kontakt |
| `ansprechpartner.html` | Ansprechpartner |
| `vorstand.html` | Vorstand |
| `an-und-verkauf.html` | An- und Verkauf |
| `impressum.html` | Impressum |
| `datenschutz.html` | Datenschutz (neu) |
| `privacy/` | Weiterleitung der alten, kaputten Datenschutz-Adresse |
| `media/` | Bilder und PDFs (gleiche Pfade wie bisher) |
| `assets/` | CSS, JavaScript, Schrift, Favicon |

## Einrichten

1. **Bilder und PDFs holen** (solange die alte Seite online ist):
   Windows: Doppelklick auf `tools\dateien-holen.bat` · macOS/Linux: `bash tools/dateien-holen.sh`
2. **Repo anlegen** und den Ordner hochladen (z. B. `rutoso/imkerverein-luisenburg`).
3. **GitHub Pages einschalten:** *Settings → Pages*, Branch `main`, Ordner `/ (root)`.
   Zum Vorzeigen erscheint die Seite unter `https://apps.rutoso.de/imkerverein-luisenburg/` – alle Pfade sind relativ.
4. **Später auf die eigene Domain umziehen:** wie bei sonneborns.de – Domain im GitHub-Konto verifizieren,
   DNS beim Domain-Anbieter auf GitHub zeigen lassen (A-Records 185.199.108–111.153, `www` als CNAME auf `rutoso.github.io`),
   dann im Repo unter *Custom domain* `www.imkerverein-luisenburg.de` eintragen und *Enforce HTTPS* aktivieren.
   E-Mail-Einträge (MX) beim Umstellen nicht ändern.

## Vor dem Livegang bitte prüfen

- **Impressum:** Vertretung durch den Vorstand ist auf den Stand 2025 aktualisiert (Lennart Schmidt, Markus Sonneborn).
  Bitte bestätigen. Die alte Seite nannte noch Hans Werner Wunderlich.
- **Verantwortlich nach § 18 MStV:** Juliane Berger mit Vereinsanschrift – ggf. eigene Anschrift eintragen.
- **Telefonnummern** im Vorstand/Impressum: Einverständnis der Personen einholen bzw. bestätigen.
- **Termine 2027** eintragen (`termine.html`), die alte Seite hatte nur Platzhalter.
- **Links zur Kreisverwaltung** (Veterinäramt/Tierseuchenkasse auf `sperrgebiete.html`) sind die alten Adressen –
  bitte prüfen, ob sie noch funktionieren.
- **Datenschutz** ist auf GitHub Pages zugeschnitten. Bei anderem Hoster Punkt 3 anpassen.
  Die Rechtstexte sind eine Vorlage und keine Rechtsberatung.

## Pflegen

- **Neue Meldung:** in `aktuelles.html` einen `<article class="meldung">`-Block oben einfügen
  (und auf der Startseite die zwei neuesten anpassen).
- **Neue Bilder:** nach `media/images/` legen, vorher auf ca. 1600 px Breite verkleinern.
- **Stand / Jahr** steht in der Fußzeile; das Jahr aktualisiert sich automatisch.
- Die E-Mail-Adressen sind gegen Spam-Bots geschützt (`class="mail" data-u="…" data-d="…"`).

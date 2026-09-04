# Monteurwohnungen Stralsund – Gutshof Groß Behnkenhagen

Statische Website für die Monteur- und Firmenunterkünfte auf dem Gutshof
Groß Behnkenhagen (Sundhagen bei Stralsund), betrieben von der
MV Immoservice GmbH.

Geplante Domain: `monteurwohnungen-stralsund.de` (Hoster: Strato)

## Struktur

```
index.html              Hauptseite (Firmen/Monteure, Distanzkarte, Feierabend-Block)
wohnung-wustrow.html    Beispielwohnung mit Grundrissen EG/OG
assets/                 Bilder (Hero, Detail, 2 Grundrisse)
```

Reines HTML/CSS, kein Build-Schritt, keine Abhängigkeiten.
Zum Ansehen genügt ein Doppelklick auf `index.html`.

## Offene Punkte

- [ ] Domain `monteurwohnungen-stralsund.de` bei Strato registrieren
- [ ] Telefonnummer ersetzen: aktuell `+49 3832 859810` (Placetel),
      soll die Nummer des ElevenLabs-Telefonagenten werden
- [ ] Impressum und Datenschutzerklärung für die Domain ergänzen
- [ ] Deployment: erst GitHub Pages zum Testen, später Strato

## Deployment über GitHub Pages

Repository → Settings → Pages → Source: `Deploy from a branch`,
Branch `main`, Ordner `/ (root)`. Die Seite erscheint danach unter
`https://<benutzername>.github.io/gutshof-website/`.

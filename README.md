# Monteurwohnungen Stralsund – Gutshof Groß Behnkenhagen

Statische Website für die Monteur- und Firmenunterkünfte auf dem Gutshof
Groß Behnkenhagen (Sundhagen bei Stralsund), betrieben von der
MV Immoservice GmbH.

Zieldomain: `monteurwohnungen-stralsund.de` (registriert, Hoster Strato).
Testbetrieb derzeit über GitHub Pages.

## Struktur

```
index.html              Hauptseite (Fakten, Ausstattung, Lage, FAQ, Kontakt)
wohnung-wustrow.html    Beispielwohnung mit Grundrissen EG/OG
impressum.html          Pflichtangaben nach § 5 DDG
datenschutz.html        Datenschutzerklärung
robots.txt              Suchmaschinen-Freigabe, Verweis auf die Sitemap
sitemap.xml             Seitenverzeichnis für Suchmaschinen
favicon.svg             Browser-Symbol
assets/                 Bilder (Hero, Detail, 2 Grundrisse)
```

Reines HTML/CSS, kein Build-Schritt, keine Abhängigkeiten, keine externen
Ressourcen. Zum Ansehen genügt ein Doppelklick auf `index.html`.

## Eckdaten (Stand September 2026)

- 18 Wohnungen in 3 Gebäuden, rund 60 Betten
- 25 bis 30 Euro netto pro Person und Nacht
- Telefon: 0383-16153005 (ElevenLabs-Telefonagent)

## Offene Punkte

- [ ] Domain auf das Hosting umstellen und Meta-Angaben live prüfen
- [ ] Datenschutzerklärung anwaltlich gegenlesen lassen
- [ ] Weitere Wohnungen als Detailseiten ergänzen
- [ ] Bilder komprimieren (Hero-Bild ist rund 380 KB)

## Deployment über GitHub Pages

Repository → Settings → Pages → Source: `Deploy from a branch`,
Branch `main`, Ordner `/ (root)`. Die Seite erscheint danach unter
`https://dnagelde.github.io/gutshof-website/`.

Achtung: Die `canonical`-Angaben zeigen bereits auf die Zieldomain.
Die GitHub-Pages-Version wird dadurch bewusst nicht in Suchmaschinen
aufgenommen – das vermeidet doppelte Inhalte.

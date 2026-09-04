# Monteurwohnungen Stralsund – Gutshof Groß Behnkenhagen

Statische Website für die Monteur- und Firmenunterkünfte auf dem Gutshof
Groß Behnkenhagen (Sundhagen bei Stralsund), betrieben von der
MV Immoservice GmbH. Dreisprachig: Deutsch, Englisch, Polnisch.

Zieldomain: `monteurwohnungen-stralsund.de` (registriert, Hoster Strato).
Testbetrieb derzeit über GitHub Pages.

## Struktur

```
index.html                      Hauptseite Deutsch
wohnung-wustrow.html            Beispielwohnung Deutsch
en/index.html                   Hauptseite Englisch
en/apartment-wustrow.html       Beispielwohnung Englisch
pl/index.html                   Hauptseite Polnisch
pl/mieszkanie-wustrow.html      Beispielwohnung Polnisch
impressum.html                  Pflichtangaben nach § 5 DDG (nur Deutsch)
datenschutz.html                Datenschutzerklärung (nur Deutsch)
robots.txt                      Suchmaschinen-Freigabe, Verweis auf die Sitemap
sitemap.xml                     Seitenverzeichnis inklusive hreflang-Verknüpfung
favicon.svg                     Browser-Symbol
assets/                         Bilder (Hero, Detail, 2 Grundrisse)
```

Reines HTML/CSS, kein Build-Schritt, keine Abhängigkeiten, keine externen
Ressourcen, kein JavaScript. Zum Ansehen genügt ein Doppelklick auf
`index.html`.

## Mehrsprachigkeit

Jede Sprache hat eigene URLs statt einer Umschaltung per JavaScript –
nur so werden die Fassungen von Suchmaschinen und KI-Systemen erfasst.
Die Sprachen sind über `hreflang` wechselseitig verknüpft; der Umschalter
oben rechts in der Kopfleiste verlinkt zwischen ihnen.

Impressum und Datenschutzerklärung bleiben deutsch. Das ist für eine
deutsche GmbH rechtlich korrekt; aus den fremdsprachigen Seiten wird
entsprechend gekennzeichnet darauf verlinkt.

**Beim Ändern von Inhalten:** Texte immer in allen drei Fassungen
nachziehen, sonst laufen die Sprachen auseinander.

## Eckdaten (Stand September 2026)

- 18 Wohnungen in 3 Gebäuden, rund 60 Betten
- 25 bis 30 Euro netto pro Person und Nacht
- Telefon: 0383-16153005 (ElevenLabs-Telefonagent)
- Entfernungen: Stralsund 18 km, Grimmen 20 km, Greifswald 30 km,
  Wolgast 60 km, Sassnitz 65 km

## Offene Punkte

- [ ] Domain auf das Hosting umstellen und Meta-Angaben live prüfen
- [ ] Datenschutzerklärung anwaltlich gegenlesen lassen
- [ ] Weitere Wohnungen als Detailseiten ergänzen
- [ ] Bilder komprimieren (Hero-Bild ist rund 380 KB)
- [ ] Übersetzungen von einem Muttersprachler gegenlesen lassen

## Deployment über GitHub Pages

Repository → Settings → Pages → Source: `Deploy from a branch`,
Branch `main`, Ordner `/ (root)`. Die Seite erscheint danach unter
`https://dnagelde.github.io/gutshof-website/`.

Achtung: Die `canonical`-Angaben zeigen bereits auf die Zieldomain.
Die GitHub-Pages-Version wird dadurch bewusst nicht in Suchmaschinen
aufgenommen – das vermeidet doppelte Inhalte.

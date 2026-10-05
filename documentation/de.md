<!-- ELUCENIA technical documentation · carga-tabagica · de · no clinical/professional/rights approval -->

# Rauchexposition (Packungsjahre)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/carga-tabagica)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Zigaretten pro Tag (Durchschnitt)

`cig`

Zigaretten · Bereich: 1–100

### Jahre des Rauchens

`anos`

Jahre · Bereich: 1–80

### Aktueller Status

`status`

- `0` — Raucht derzeit
- `1` — Ehemals rauchend

### Alter (für das Screening)

`idade`

Jahre · optional · Bereich: 18–110

### Jahre seit Rauchstopp (ehemals rauchend)

`parou`

Jahre · optional · Bereich: 0–80

## Fassung der Methode

Packungen mit 20 Zigaretten; Packungsjahre; USPSTF 2021: 50–80 Jahre, ≥20 Packungsjahre, Rauchstopp≤15 Jahre

## Dokumentierte Formel

Packungsjahre = (Zigaretten/Tag ÷ 20) × Rauchjahre. Eine Packung enthält 20 Zigaretten.

Screening (USPSTF 2021): Jährliches Niedrigdosis-Thorax-CT für Erwachsene von 50–80 Jahren mit ≥ 20 Packungsjahren, die rauchen oder seit ≤ 15 Jahren aufgehört haben.

## Grenzen und Population

Die USPSTF-Kriterien 2021 betreffen jährliches Screening mittels Niedrigdosis-CT bei Erwachsenen von 50–80 Jahren mit mindestens 20 Packungsjahren, die aktuell rauchen oder in den vergangenen 15 Jahren aufgehört haben. Die Empfehlung verlangt außerdem das Beenden des Screenings nach 15 rauchfreien Jahren oder wenn Gesundheitsprobleme Lebenserwartung oder Fähigkeit beziehungsweise Bereitschaft zu einer kurativen Lungenoperation wesentlich begrenzen. Die Packungsjahrberechnung bewertet diese klinischen Bedingungen nicht.

## Referenzen

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

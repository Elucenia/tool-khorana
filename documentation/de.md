<!-- ELUCENIA technical documentation · khorana · de · no clinical/professional/rights approval -->

# Khorana-Score

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/khorana)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Lokalisation des Primärtumors

`sitio`

- `0` — Andere Lokalisationen
- `1` — Hohes Risiko: Lungenkrebs, Lymphom, gynäkologischer Krebs, Blasen- oder Hodenkrebs
- `2` — Sehr hohes Risiko: Magen- oder Bauchspeicheldrüsenkrebs

### Thrombozyten vor Chemotherapie ≥ 350.000/µL

`plaq`

### Hämoglobin \< 10 g/dL oder Anwendung eines erythropoesestimulierenden Wirkstoffs

`hb`

### Leukozyten vor Chemotherapie \> 11.000/µL

`leuco`

### BMI ≥ 35 kg/m²

`imc`

## Fassung der Methode

Khorana 2008: Tumorort+Thrombozyten+Hb/EPO+Leukozyten+BMI, Gesamt 0–6

## Dokumentierte Formel

Magen oder Pankreas 2 · Lunge, Lymphom, gynäkologischer Krebs, Harnblase oder Hoden 1 · Thrombozyten ≥ 350.000/µL 1 · Hb \< 10 g/dL oder Erythropoese-stimulierendes Mittel 1 · Leukozyten \> 11.000/µL 1 · BMI ≥ 35 kg/m² 1. Maximum: 6.

## Grenzen und Population

Risikopunktzahl für venöse Thromboembolien bei Krebs und ambulanter systemischer Therapie anhand von Daten vor der Chemotherapie. Die Punktzahl misst kein Blutungsrisiko und begründet allein weder eine Antikoagulation noch die Wahl eines Arzneimittels oder einer Dosis. Die Einstufung muss durch die klinische Beurteilung und die Beurteilung des Blutungsrisikos ergänzt werden. Diese lokalen numerischen Tests belegen keine Anwendung bei Kindern, stationären Patienten oder im perioperativen Umfeld; dafür sind eigene Nachweise und spezifische Protokolle erforderlich.

## Referenzen

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

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

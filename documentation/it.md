<!-- ELUCENIA technical documentation · khorana · it · no clinical/professional/rights approval -->

# Punteggio di Khorana

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/khorana)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sede del tumore primario

`sitio`

- `0` — Altre sedi
- `1` — Rischio elevato: tumore polmonare, linfoma, tumore ginecologico, vescicale o testicolare
- `2` — Rischio molto elevato: tumore gastrico o pancreatico

### Piastrine prima della chemioterapia ≥ 350.000/µL

`plaq`

### Emoglobina \< 10 g/dL o uso di un agente stimolante l’eritropoiesi

`hb`

### Leucociti prima della chemioterapia \> 11.000/µL

`leuco`

### IMC ≥ 35 kg/m²

`imc`

## Edizione del metodo

Khorana 2008: sede tumorale+piastrine+Hb/EPO+leucociti+IMC, totale 0–6

## Formula documentata

Stomaco o pancreas 2 · polmone, linfoma, tumore ginecologico, vescica o testicolo 1 · piastrine ≥ 350.000/µL 1 · Hb \< 10 g/dL o agente stimolante l’eritropoiesi 1 · leucociti \> 11.000/µL 1 · IMC ≥ 35 kg/m² 1. Massimo: 6.

## Limiti e popolazione

Punteggio del rischio di tromboembolia venosa nel contesto del cancro e del trattamento sistemico ambulatoriale, usando dati precedenti alla chemioterapia. Il punteggio non misura il rischio emorragico e non indica, da solo, anticoagulazione, un farmaco o una dose. La classificazione deve essere integrata dalla valutazione clinica e del rischio emorragico. Questi test numerici locali non stabiliscono l’applicazione alla popolazione pediatrica, ai pazienti ricoverati o al contesto perioperatorio; tali usi richiedono evidenze e protocolli specifici.

## Riferimenti

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Rischio basso: TEV nell'0,8% (in circa 2,5 mesi)

La profilassi di routine non è indicata.


### 2

Rischio intermedio: TEV nell'1,8%

ASCO 2020: con 2 punti o più, si può offrire apixaban, rivaroxaban o EBPM, se non vi è un rischio elevato di sanguinamento.


### 3

Rischio elevato: TEV nel 7,1%

ASCO 2020: offrire tromboprofilassi (apixaban, rivaroxaban o EBPM) se non vi è un rischio elevato di sanguinamento né interazione.


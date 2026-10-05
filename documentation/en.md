<!-- ELUCENIA technical documentation · khorana · en · no clinical/professional/rights approval -->

# Khorana score

[conditions, sources and permissions](https://elucenia.org/en/tools/khorana)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Primary cancer site

`sitio`

- `0` — Other sites
- `1` — High risk: lung, lymphoma, gynecologic, bladder or testicular cancer
- `2` — Very high risk: stomach or pancreatic cancer

### Prechemotherapy platelet count ≥ 350,000/µL

`plaq`

### Hemoglobin \< 10 g/dL or use of an erythropoiesis-stimulating agent

`hb`

### Prechemotherapy leukocyte count \> 11,000/µL

`leuco`

### BMI ≥ 35 kg/m²

`imc`

## Method edition

Khorana 2008: tumor site+platelets+Hb/EPO+leukocytes+BMI, total 0–6

## Documented formula

Stomach or pancreas 2 · lung, lymphoma, gynecologic, bladder or testicular cancer 1 · platelets ≥ 350,000/µL 1 · Hb \< 10 g/dL or an erythropoiesis-stimulating agent 1 · leukocytes \> 11,000/µL 1 · BMI ≥ 35 kg/m² 1. Maximum: 6.

## Limits and population

VTE risk score in the context of cancer and outpatient systemic therapy, using prechemotherapy data. The score does not measure bleeding risk and does not, on its own, indicate anticoagulation, a drug or a dose. Classification must be complemented by clinical assessment and bleeding-risk assessment. These local numerical tests do not establish application to pediatric patients, hospital inpatients or the perioperative setting; those uses require specific evidence and protocols.

## References

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

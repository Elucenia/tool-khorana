<!-- ELUCENIA technical documentation · khorana · pt-BR · no clinical/professional/rights approval -->

# Escore de Khorana

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/khorana)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Local do tumor primário

`sitio`

- `0` — Outros
- `1` — Alto risco: pulmão, linfoma, ginecológico, bexiga ou testículo
- `2` — Muito alto risco: estômago ou pâncreas

### Plaquetas pré-quimioterapia ≥ 350.000/µL

`plaq`

### Hemoglobina \< 10 g/dL ou uso de estimulador da eritropoese

`hb`

### Leucócitos pré-quimioterapia \> 11.000/µL

`leuco`

### IMC ≥ 35 kg/m²

`imc`

## Edição do método

Khorana 2008:localtumor+plaquetas+Hb/EPO+leucócitos+IMC, total 0–6

## Fórmula documentada

Estômago ou pâncreas 2 · pulmão, linfoma, ginecológico, bexiga ou testículo 1 · plaquetas ≥ 350.000/µL 1 · Hb \< 10 g/dL ou estimulador da eritropoese 1 · leucócitos \> 11.000/µL 1 · IMC ≥ 35 kg/m² 1. Máximo: 6.

## Limites e população

Escore de risco de TEV no contexto de câncer e tratamento sistêmico ambulatorial, com dados pré-quimioterapia. O escore não mede risco de sangramento e não indica, sozinho, anticoagulação, fármaco ou dose. A classificação precisa ser complementada pela avaliação clínica e pelo risco de sangramento. A aplicação a população pediátrica, internação hospitalar ou contexto perioperatório não é estabelecida por estes testes numéricos locais e exige evidência e protocolo específicos.

## Referências

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

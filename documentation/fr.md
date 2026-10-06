<!-- ELUCENIA technical documentation · khorana · fr · no clinical/professional/rights approval -->

# Score de Khorana

[conditions, sources et autorisations](https://elucenia.org/fr/outils/khorana)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Localisation du cancer primitif

`sitio`

- `0` — Autres localisations
- `1` — Risque élevé : cancer du poumon, lymphome, cancer gynécologique, de la vessie ou du testicule
- `2` — Risque très élevé : cancer de l’estomac ou du pancréas

### Plaquettes avant chimiothérapie ≥ 350 000/µL

`plaq`

### Hémoglobine \< 10 g/dL ou utilisation d’un agent stimulant l’érythropoïèse

`hb`

### Leucocytes avant chimiothérapie \> 11 000/µL

`leuco`

### IMC ≥ 35 kg/m²

`imc`

## Édition de la méthode

Khorana 2008 : site tumoral+plaquettes+Hb/EPO+leucocytes+IMC, total 0–6

## Formule documentée

Estomac ou pancréas 2 · poumon, lymphome, cancer gynécologique, vessie ou testicule 1 · plaquettes ≥ 350 000/µL 1 · Hb \< 10 g/dL ou agent stimulant l’érythropoïèse 1 · leucocytes \> 11 000/µL 1 · IMC ≥ 35 kg/m² 1. Maximum : 6.

## Limites et population

Score de risque de maladie thromboembolique veineuse dans le contexte du cancer et d’un traitement systémique ambulatoire, à partir de données préchimiothérapie. Le score ne mesure pas le risque hémorragique et n’indique pas, à lui seul, une anticoagulation, un médicament ou une dose. La classification doit être complétée par l’évaluation clinique et du risque hémorragique. Ces tests numériques locaux n’établissent pas son application à la population pédiatrique, aux patients hospitalisés ou au contexte périopératoire ; ces usages nécessitent des preuves et des protocoles spécifiques.

## Références

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Faible risque : TVE à 0,8 % (environ 2,5 mois)

La prophylaxie de routine n’est pas indiquée.


### 2

Risque intermédiaire : TVE à 1,8 %

ASCO 2020 : à partir de 2 points, l’apixaban, le rivaroxaban ou l’HBPM peuvent être proposés, s’il n’existe pas de risque hémorragique élevé.


### 3

Risque élevé : TVE à 7,1 %

ASCO 2020 : proposer une thromboprophylaxie (apixaban, rivaroxaban ou HBPM) s’il n’existe pas de risque hémorragique élevé ni d’interaction.


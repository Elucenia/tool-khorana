<!-- ELUCENIA technical documentation · khorana · es · no clinical/professional/rights approval -->

# Puntuación de Khorana

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/khorana)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Localización del cáncer primario

`sitio`

- `0` — Otras localizaciones
- `1` — Riesgo alto: cáncer de pulmón, linfoma, cáncer ginecológico, de vejiga o testicular
- `2` — Riesgo muy alto: cáncer de estómago o de páncreas

### Recuento de plaquetas antes de la quimioterapia ≥ 350.000/µL

`plaq`

### Hemoglobina \< 10 g/dL o uso de un agente estimulante de la eritropoyesis

`hb`

### Recuento de leucocitos antes de la quimioterapia \> 11.000/µL

`leuco`

### IMC ≥ 35 kg/m²

`imc`

## Edición del método

Khorana 2008: localización tumoral+plaquetas+Hb/EPO+leucocitos+IMC, total 0–6

## Fórmula documentada

Estómago o páncreas 2 · pulmón, linfoma, cáncer ginecológico, vejiga o testículo 1 · plaquetas ≥ 350.000/µL 1 · Hb \< 10 g/dL o un agente estimulante de la eritropoyesis 1 · leucocitos \> 11.000/µL 1 · IMC ≥ 35 kg/m² 1. Máximo: 6.

## Límites y población

Puntuación de riesgo de tromboembolismo venoso en el contexto del cáncer y el tratamiento sistémico ambulatorio, con datos previos a la quimioterapia. La puntuación no mide el riesgo hemorrágico ni indica por sí sola anticoagulación, un fármaco o una dosis. La clasificación debe complementarse con la evaluación clínica y del riesgo hemorrágico. Estos ensayos numéricos locales no establecen su aplicación a la población pediátrica, a pacientes hospitalizados ni al contexto perioperatorio; esos usos requieren evidencia y protocolos específicos.

## Referencias

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Bajo riesgo: TEV en 0,8% (en cerca de 2,5 meses)

No está indicada la profilaxis de rutina.


### 2

Riesgo intermedio: TEV en 1,8%

ASCO 2020: con 2 puntos o más, se puede ofrecer apixabán, rivaroxabán o HBPM, si no hay alto riesgo de sangrado.


### 3

Alto riesgo: TEV en 7,1%

ASCO 2020: ofrecer tromboprofilaxis (apixabán, rivaroxabán o HBPM) si no hay alto riesgo de sangrado ni interacción.


<!-- ELUCENIA technical documentation · khorana · zh · no clinical/professional/rights approval -->

# Khorana 评分

[条件、来源与许可](https://elucenia.org/zh/tools/khorana)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 原发肿瘤部位

`sitio`

- `0` — 其他部位
- `1` — 高风险：肺癌、淋巴瘤、妇科癌、膀胱癌或睾丸癌
- `2` — 极高风险：胃癌或胰腺癌

### 化疗前血小板计数 ≥ 350000/µL

`plaq`

### 血红蛋白 \< 10 g/dL，或使用红细胞生成刺激剂

`hb`

### 化疗前白细胞计数 \> 11000/µL

`leuco`

### 体重指数（BMI） ≥ 35 kg/m²

`imc`

## 方法版本

Khorana 2008：肿瘤部位+血小板+Hb/EPO+白细胞+BMI，总分0–6

## 已记录的公式

胃或胰腺2 · 肺、淋巴瘤、妇科癌症、膀胱或睾丸1 · 血小板≥350000/µL 1 · Hb \< 10 g/dL或使用促红细胞生成药物1 · 白细胞\>11000/µL 1 · BMI≥35 kg/m² 1。最高：6。

## 限制与适用人群

这是用于癌症及门诊全身治疗情境的静脉血栓栓塞风险评分，采用化疗前的数据。该评分不评估出血风险，也不能单独决定抗凝治疗、药物或剂量。风险分类必须结合临床评估和出血风险评估。这些本地数值测试并不能确立其在儿童、住院或围手术期情境中的适用性；这些用途需要具体证据和专门方案。

## 参考文献

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

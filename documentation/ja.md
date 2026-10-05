<!-- ELUCENIA technical documentation · khorana · ja · no clinical/professional/rights approval -->

# Khoranaスコア

[条件・出典・許諾](https://elucenia.org/ja/tools/khorana)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 原発がんの部位

`sitio`

- `0` — その他の部位
- `1` — 高リスク：肺がん、リンパ腫、婦人科がん、膀胱がん、精巣がん
- `2` — 非常に高いリスク：胃がん、膵がん

### 化学療法前の血小板数 ≥ 350000/µL

`plaq`

### ヘモグロビン \< 10 g/dL、または赤血球造血刺激因子製剤の使用

`hb`

### 化学療法前の白血球数 \> 11000/µL

`leuco`

### 体格指数（BMI） ≥ 35 kg/m²

`imc`

## 方法の版

Khorana 2008：腫瘍部位+血小板+Hb/EPO+白血球+BMI、合計0–6

## 記載された計算式

胃または膵臓2 · 肺、リンパ腫、婦人科がん、膀胱または精巣1 · 血小板≥350000/µL 1 · Hb \< 10 g/dLまたは赤血球造血刺激因子製剤の使用1 · 白血球\>11000/µL 1 · BMI≥35 kg/m² 1。最高：6。

## 限界・対象集団

がんに対する外来全身療法の状況で、化学療法前のデータを用いて静脈血栓塞栓症のリスクを評価するスコアです。出血リスクを測定するものではなく、スコアだけで抗凝固療法の適応、薬剤、用量を決めることはできません。分類には、臨床評価と出血リスクの評価を組み合わせる必要があります。小児、入院中、周術期への適用は、この実装の数値テストでは確立されておらず、それぞれに固有の根拠とプロトコルが必要です。

## 参考文献

- [Khorana AA et al. Development and validation of a predictive model for chemotherapy-associated thrombosis. Blood, 2008.](https://doi.org/10.1182/blood-2007-10-116327)

- [Key NS et al. Venous thromboembolism prophylaxis and treatment in patients with cancer: ASCO clinical practice guideline update. J Clin Oncol, 2020.](https://doi.org/10.1200/JCO.19.01461)

- [ASH official VTE pocket guide, October2023, based on ASH2021 guideline](https://www.hematology.org/-/media/hematology/files/clinicians/guidelines/vte/vte-update-03_24/19894_vte-prophylaxis-pocket-guide-8-panel___0001_high_res_proof-(2).pdf)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

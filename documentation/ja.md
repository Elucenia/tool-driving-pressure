<!-- ELUCENIA technical documentation · driving-pressure · ja · no clinical/professional/rights approval -->

# 駆動圧・静的コンプライアンス

[条件・出典・許諾](https://elucenia.org/ja/tools/driving-pressure)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 一回換気量

`vt`

mL · 範囲: 100–1500

### プラトー圧（吸気ポーズ）

`pplat`

cmH₂O · 範囲: 5–60

### 総PEEP

`peep`

cmH₂O · 範囲: 0–30

### 予測体重

`pbw`

kg · 任意 · 範囲: 20–120

## 方法の版

ΔP=Pplat−PEEP；Cstat=VT/ΔP；Amato 2015受動換気の文脈

## 記載された計算式

駆動圧 (ΔP) = プラトー圧 − PEEP.

静的コンプライアンス = 一回換気量 ÷ ΔP (mL/cmH₂O).

## 限界・対象集団

Amato 2015の解析は、過去の九つの試験から得た3562人の急性呼吸窮迫症候群（ARDS）患者を、能動的な呼吸がない人工呼吸の条件で研究しました。駆動圧（driving pressure）はVT/CRSとして、また生存に関連する変数として解析されました。この関連だけでは普遍的な閾値や、計算値に基づく治療介入は確立されません。測定手技と換気条件を確認する必要があります。

## 参考文献

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

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

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

ドライビングプレッシャーは15 cmH₂Oまで

| 結果の詳細 | |
| --- | --- |
| 静的コンプライアンス | 28.0 mL/cmH₂O |


### 2

15 cmH₂O を超える Driving pressure：ARDS におけるより高い死亡率と関連

| 結果の詳細 | |
| --- | --- |
| 静的コンプライアンス | 20.5 mL/cmH₂O |


### 3

ドライビングプレッシャーは15 cmH₂Oまで

| 結果の詳細 | |
| --- | --- |
| 静的コンプライアンス | 38.5 mL/cmH₂O |
| 一回換気量 | 7.1 mL/kg の予測体重 |


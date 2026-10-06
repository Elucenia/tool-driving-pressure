<!-- ELUCENIA technical documentation · driving-pressure · zh · no clinical/professional/rights approval -->

# 驱动压与静态顺应性

[条件、来源与许可](https://elucenia.org/zh/tools/driving-pressure)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 潮气量

`vt`

mL · 范围: 100–1500

### 平台压（吸气暂停）

`pplat`

cmH₂O · 范围: 5–60

### 总 PEEP

`peep`

cmH₂O · 范围: 0–30

### 预测体重

`pbw`

kg · 选填 · 范围: 20–120

## 方法版本

ΔP=Pplat−PEEP；Cstat=VT/ΔP；Amato 2015被动通气情境

## 已记录的公式

驱动压 (ΔP) = 平台压 − PEEP.

静态顺应性 = 潮气量 ÷ ΔP (mL/cmH₂O).

## 限制与适用人群

Amato 2015分析了既往九项试验中的3562名急性呼吸窘迫综合征（ARDS）患者，情境为无主动呼吸的机械通气。驱动压以VT/CRS表示，并作为与生存相关的变量进行分析；该关联本身不能确立通用阈值或由此计算指导的治疗干预。应核对测量技术和通气条件。

## 参考文献

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

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

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

驱动压高达 15 cmH₂O

| 结果详情 | |
| --- | --- |
| 静态顺应性 | 28.0 mL/cmH₂O |


### 2

驱动压高于 15 cmH₂O：与 ARDS 中更高的死亡率相关

| 结果详情 | |
| --- | --- |
| 静态顺应性 | 20.5 mL/cmH₂O |


### 3

驱动压高达 15 cmH₂O

| 结果详情 | |
| --- | --- |
| 静态顺应性 | 38.5 mL/cmH₂O |
| 潮气量 | 7.1 mL/kg 预测体重 |


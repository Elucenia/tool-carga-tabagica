<!-- ELUCENIA technical documentation · carga-tabagica · zh · no clinical/professional/rights approval -->

# 吸烟暴露量（包年）

[条件、来源与许可](https://elucenia.org/zh/tools/carga-tabagica)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 每日吸烟支数（平均）

`cig`

支香烟 · 范围: 1–100

### 吸烟年数

`anos`

年 · 范围: 1–80

### 当前情况

`status`

- `0` — 吸烟
- `1` — 既往吸烟者

### 年龄（用于筛查）

`idade`

年 · 选填 · 范围: 18–110

### 戒烟年数（既往吸烟者）

`parou`

年 · 选填 · 范围: 0–80

## 方法版本

每包20支；包年；USPSTF 2021：50–80岁、≥20包年、戒烟≤15年

## 已记录的公式

包年 = （每日支数÷20）×吸烟年数。每包20支。

筛查（USPSTF 2021）： 50–80岁、≥20包年且仍吸烟或戒烟≤15年的成人，每年进行低剂量胸部CT。

## 限制与适用人群

USPSTF 2021标准针对50–80岁、有至少20包年吸烟史且仍吸烟或在过去15年内戒烟的成人，建议每年进行低剂量CT筛查。建议还规定，在戒烟15年后，或健康问题显著限制预期寿命、接受根治性肺手术的能力或意愿时，应停止筛查。包年计算不能评估这些临床条件。

## 参考文献

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

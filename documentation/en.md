<!-- ELUCENIA technical documentation · carga-tabagica · en · no clinical/professional/rights approval -->

# Smoking exposure (pack-years)

[conditions, sources and permissions](https://elucenia.org/en/tools/carga-tabagica)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Cigarettes per day (average)

`cig`

cigarettes · range: 1–100

### Years of smoking

`anos`

years · range: 1–80

### Current status

`status`

- `0` — Currently smokes
- `1` — Former smoker

### Age (for screening)

`idade`

years · optional · range: 18–110

### Years since quitting (former smoker)

`parou`

years · optional · range: 0–80

## Method edition

Packs of 20 cigarettes; pack-years; USPSTF 2021 cutoff: age 50–80, ≥20 pack-years, cessation≤15 years

## Documented formula

Pack-years = (cigarettes/day ÷ 20) × years smoked. One pack contains 20 cigarettes.

Screening (USPSTF 2021): Annual low-dose chest CT for adults aged 50–80 with ≥ 20 pack-years who currently smoke or quit within 15 years.

## Limits and population

The USPSTF 2021 criteria concern annual screening with low-dose CT in adults aged 50–80 years with a history of at least 20 pack-years who currently smoke or quit within the past 15 years. The recommendation also calls for stopping screening after 15 years without smoking or when health conditions substantially limit life expectancy or the ability/willingness to undergo curative lung surgery. The pack-year calculation does not assess these clinical conditions.

## References

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

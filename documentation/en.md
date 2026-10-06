<!-- ELUCENIA technical documentation · driving-pressure · en · no clinical/professional/rights approval -->

# Driving pressure and static compliance

[conditions, sources and permissions](https://elucenia.org/en/tools/driving-pressure)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Tidal volume

`vt`

mL · range: 100–1500

### Plateau pressure (inspiratory pause)

`pplat`

cmH₂O · range: 5–60

### Total PEEP

`peep`

cmH₂O · range: 0–30

### Predicted body weight

`pbw`

kg · optional · range: 20–120

## Method edition

ΔP=Pplat−PEEP; Cstat=VT/ΔP; Amato 2015 passive-ventilation context

## Documented formula

Driving pressure (ΔP) = plateau pressure − PEEP.

Static compliance = tidal volume ÷ ΔP (mL/cmH₂O).

## Limits and population

Amato’s 2015 analysis studied 3562 patients with ARDS from nine previous trials, in the context of ventilation without active breathing. Driving pressure was analyzed as VT/CRS and as a variable associated with survival; that association alone does not establish a universal threshold or a therapeutic intervention guided by the calculation. Measurement technique and ventilatory conditions must be checked.

## References

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

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

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Driving pressure up to 15 cmH₂O

| Result details | |
| --- | --- |
| Static compliance | 28.0 mL/cmH₂O |


### 2

Driving pressure above 15 cmH₂O: associated with higher mortality in ARDS

| Result details | |
| --- | --- |
| Static compliance | 20.5 mL/cmH₂O |


### 3

Driving pressure up to 15 cmH₂O

| Result details | |
| --- | --- |
| Static compliance | 38.5 mL/cmH₂O |
| Tidal volume | 7.1 mL/kg of predicted body weight |


<!-- ELUCENIA technical documentation · driving-pressure · pt-BR · no clinical/professional/rights approval -->

# Driving pressure e complacência estática

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/driving-pressure)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Volume corrente

`vt`

mL · intervalo: 100–1500

### Pressão de platô (pausa inspiratória)

`pplat`

cmH₂O · intervalo: 5–60

### PEEP total

`peep`

cmH₂O · intervalo: 0–30

### Peso predito

`pbw`

kg · opcional · intervalo: 20–120

## Edição do método

ΔP=Pplat−PEEP; Cstat=VT/ΔP; contexto Amato 2015 ventilação passiva

## Fórmula documentada

Driving pressure (ΔP) = pressão de platô − PEEP.

Complacência estática = volume corrente ÷ ΔP (mL/cmH₂O).

## Limites e população

A análise Amato 2015 estudou 3562 pacientes com SDRA de nove ensaios prévios, no contexto de ventilação sem respiração ativa. A driving pressure foi analisada como VT/CRS e como variável associada à sobrevivência; essa associação não estabelece, sozinha, um limiar universal ou uma intervenção terapêutica guiada pelo cálculo. Técnica de medida e condições ventilatórias precisam ser conferidas.

## Referências

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

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

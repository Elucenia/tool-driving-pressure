<!-- ELUCENIA technical documentation · driving-pressure · es · no clinical/professional/rights approval -->

# Presión de distensión y distensibilidad estática

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/driving-pressure)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Volumen corriente

`vt`

mL · intervalo: 100–1500

### Presión meseta (pausa inspiratoria)

`pplat`

cmH₂O · intervalo: 5–60

### PEEP total

`peep`

cmH₂O · intervalo: 0–30

### Peso corporal predicho

`pbw`

kg · opcional · intervalo: 20–120

## Edición del método

ΔP=Pplat−PEEP; Cstat=VT/ΔP; contexto Amato 2015 de ventilación pasiva

## Fórmula documentada

Presión de distensión (ΔP) = presión meseta − PEEP.

Distensibilidad estática = volumen corriente ÷ ΔP (mL/cmH₂O).

## Límites y población

El análisis Amato 2015 estudió 3562 pacientes con SDRA de nueve ensayos previos, en el contexto de ventilación sin respiración activa. La presión de distensión se analizó como VT/CRS y como variable asociada a la supervivencia; esta asociación no establece por sí sola un umbral universal ni una intervención terapéutica guiada por el cálculo. Deben comprobarse la técnica de medición y las condiciones ventilatorias.

## Referencias

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

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

<!-- ELUCENIA technical documentation · driving-pressure · it · no clinical/professional/rights approval -->

# Driving pressure e compliance statica

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/driving-pressure)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Volume corrente

`vt`

mL · intervallo: 100–1500

### Pressione di plateau (pausa inspiratoria)

`pplat`

cmH₂O · intervallo: 5–60

### PEEP totale

`peep`

cmH₂O · intervallo: 0–30

### Peso corporeo predetto

`pbw`

kg · facoltativo · intervallo: 20–120

## Edizione del metodo

ΔP=Pplat−PEEP; Cstat=VT/ΔP; contesto Amato 2015 di ventilazione passiva

## Formula documentata

Pressione di guida (ΔP) = pressione di plateau − PEEP.

Compliance statica = volume corrente ÷ ΔP (mL/cmH₂O).

## Limiti e popolazione

L’analisi Amato 2015 ha studiato 3562 pazienti con ARDS di nove studi precedenti, nel contesto della ventilazione senza respirazione attiva. La driving pressure è stata analizzata come VT/CRS e come variabile associata alla sopravvivenza; tale associazione da sola non stabilisce una soglia universale o un intervento terapeutico guidato dal calcolo. Tecnica di misurazione e condizioni ventilatorie devono essere verificate.

## Riferimenti

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

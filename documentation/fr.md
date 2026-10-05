<!-- ELUCENIA technical documentation · driving-pressure · fr · no clinical/professional/rights approval -->

# Pression motrice et compliance statique

[conditions, sources et autorisations](https://elucenia.org/fr/outils/driving-pressure)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Volume courant

`vt`

mL · intervalle: 100–1500

### Pression de plateau (pause inspiratoire)

`pplat`

cmH₂O · intervalle: 5–60

### PEEP totale

`peep`

cmH₂O · intervalle: 0–30

### Poids corporel prédit

`pbw`

kg · facultatif · intervalle: 20–120

## Édition de la méthode

ΔP=Pplat−PEEP ; Cstat=VT/ΔP ; contexte Amato 2015 ventilation passive

## Formule documentée

Pression motrice (ΔP) = pression plateau − PEEP.

Compliance statique = volume courant ÷ ΔP (mL/cmH₂O).

## Limites et population

L’analyse Amato 2015 a étudié 3562 patients atteints de SDRA issus de neuf essais antérieurs, dans le contexte d’une ventilation sans respiration active. La pression motrice a été analysée comme VT/CRS et comme variable associée à la survie ; cette association n’établit pas, à elle seule, un seuil universel ou une intervention thérapeutique guidée par le calcul. La technique de mesure et les conditions ventilatoires doivent être vérifiées.

## Références

- [Amato MBP et al. Driving pressure and survival in the acute respiratory distress syndrome. N Engl J Med, 2015.](https://doi.org/10.1056/NEJMsa1410639)

- [Fan E et al. An Official American Thoracic Society/European Society of Intensive Care Medicine/Society of Critical Care Medicine Clinical Practice Guideline: Mechanical Ventilation in Adult Patients with Acute Respiratory Distress Syndrome. Am J Respir Crit Care Med, 2017.](https://doi.org/10.1164/rccm.201703-0548ST)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

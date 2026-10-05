<!-- ELUCENIA technical documentation · carga-tabagica · fr · no clinical/professional/rights approval -->

# Exposition tabagique (paquets-années)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/carga-tabagica)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Cigarettes par jour (moyenne)

`cig`

cigarettes · intervalle: 1–100

### Années de tabagisme

`anos`

ans · intervalle: 1–80

### Situation actuelle

`status`

- `0` — Fume actuellement
- `1` — Ancien fumeur

### Âge (pour le dépistage)

`idade`

ans · facultatif · intervalle: 18–110

### Années depuis l’arrêt (ancien fumeur)

`parou`

ans · facultatif · intervalle: 0–80

## Édition de la méthode

Paquets de 20 cigarettes ; paquets-années ; USPSTF 2021 : 50–80 ans, ≥20 paquets-années, sevrage≤15 ans

## Formule documentée

Paquets-années = (cigarettes/jour ÷ 20) × années de tabagisme. Un paquet contient 20 cigarettes.

Dépistage (USPSTF 2021) : Scanner thoracique annuel à faible dose chez les adultes de 50–80 ans avec ≥ 20 paquets-années, fumeurs actuels ou sevrés depuis ≤ 15 ans.

## Limites et population

Les critères USPSTF 2021 concernent le dépistage annuel par tomodensitométrie à faible dose chez les adultes de 50–80 ans ayant au moins 20 paquets-années, fumeurs actuels ou ayant arrêté au cours des 15 dernières années. La recommandation prévoit aussi l’arrêt du dépistage après 15 ans sans tabac ou lorsque des problèmes de santé limitent sensiblement l’espérance de vie ou la capacité ou volonté de subir une chirurgie pulmonaire curative. Le calcul des paquets-années n’évalue pas ces conditions cliniques.

## Références

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

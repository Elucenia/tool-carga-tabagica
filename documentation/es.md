<!-- ELUCENIA technical documentation · carga-tabagica · es · no clinical/professional/rights approval -->

# Exposición tabáquica (paquetes-año)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/carga-tabagica)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Cigarrillos al día (media)

`cig`

cigarrillos · intervalo: 1–100

### Años de tabaquismo

`anos`

años · intervalo: 1–80

### Situación actual

`status`

- `0` — Fuma actualmente
- `1` — Exfumador

### Edad (para el cribado)

`idade`

años · opcional · intervalo: 18–110

### Años desde que dejó de fumar (exfumador)

`parou`

años · opcional · intervalo: 0–80

## Edición del método

Paquetes de 20 cigarrillos; paquetes-año; USPSTF 2021: 50–80 años, ≥20 paquetes-año, abandono≤15 años

## Fórmula documentada

Paquetes-año = (cigarrillos/día ÷ 20) × años fumados. Un paquete contiene 20 cigarrillos.

Cribado (USPSTF 2021): TC torácica anual de baja dosis en adultos de 50–80 años con ≥ 20 paquetes-año que fuman o dejaron hace ≤ 15 años.

## Límites y población

Los criterios USPSTF 2021 se refieren al cribado anual mediante tomografía de baja dosis en adultos de 50–80 años con antecedentes de al menos 20 paquetes-año, fumadores actuales o que dejaron de fumar en los últimos 15 años. La recomendación también indica interrumpir el cribado tras 15 años sin fumar o cuando las condiciones de salud limitan sustancialmente la esperanza de vida o la capacidad/disposición para una cirugía pulmonar curativa. El cálculo de paquetes-año no evalúa estas condiciones clínicas.

## Referencias

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Elegible para el cribado anual de cáncer de pulmón con TC de baja dosis (USPSTF 2021)

| Detalles del resultado | |
| --- | --- |
| Cigarrillos a lo largo de la vida (aprox.) | 146000 |

Fumador actual: cada consulta es una oportunidad para abordar la cesación.


### 2

Carga tabáquica por debajo de 20 paquetes-año

| Detalles del resultado | |
| --- | --- |
| Cigarrillos a lo largo de la vida (aprox.) | 54750 |

Fumador actual: cada consulta es una oportunidad para abordar la cesación.


### 3

Fuera de los criterios de cribado de la USPSTF 2021

| Detalles del resultado | |
| --- | --- |
| Cigarrillos a lo largo de la vida (aprox.) | 438000 |
| Motivo | dejó de fumar hace más de 15 años |


### 4

Elegible para el cribado anual de cáncer de pulmón con TC de baja dosis (USPSTF 2021)

| Detalles del resultado | |
| --- | --- |
| Cigarrillos a lo largo de la vida (aprox.) | 219000 |


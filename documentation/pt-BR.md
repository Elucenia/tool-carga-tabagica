<!-- ELUCENIA technical documentation · carga-tabagica · pt-BR · no clinical/professional/rights approval -->

# Carga tabágica (maços-ano)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/carga-tabagica)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Cigarros por dia (média)

`cig`

cigarros · intervalo: 1–100

### Anos de tabagismo

`anos`

anos · intervalo: 1–80

### Situação atual

`status`

- `0` — Fuma
- `1` — Ex-fumante

### Idade (para o rastreamento)

`idade`

anos · opcional · intervalo: 18–110

### Anos desde que parou (ex-fumante)

`parou`

anos · opcional · intervalo: 0–80

## Edição do método

Maços de 20 cigarros; packyears; corte USPSTF 2021:50–80 anos,≥20 maçosano, cessação≤15 anos

## Fórmula documentada

Maços-ano = (cigarros por dia ÷ 20) × anos de tabagismo. Um maço tem 20 cigarros.

Rastreamento (USPSTF 2021): TC de tórax de baixa dose anual para adultos de 50 a 80 anos com ≥ 20 maços-ano que fumam atualmente ou pararam há até 15 anos.

## Limites e população

Os critérios USPSTF 2021 referem-se a rastreamento anual por tomografia de baixa dose em adultos de 50–80 anos com histórico de pelo menos 20 maços-ano, fumantes atuais ou que cessaram nos últimos 15 anos. A recomendação também determina interromper o rastreamento após 15 anos sem fumar ou quando condições de saúde limitam substancialmente a expectativa de vida ou a capacidade/disposição para cirurgia pulmonar curativa. O cálculo de maços-ano não avalia essas condições clínicas.

## Referências

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

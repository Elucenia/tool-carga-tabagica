<!-- ELUCENIA technical documentation · carga-tabagica · it · no clinical/professional/rights approval -->

# Esposizione al fumo (pacchetti-anno)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/carga-tabagica)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Sigarette al giorno (media)

`cig`

sigarette · intervallo: 1–100

### Anni di fumo

`anos`

anni · intervallo: 1–80

### Situazione attuale

`status`

- `0` — Fuma attualmente
- `1` — Ex fumatore

### Età (per lo screening)

`idade`

anni · facoltativo · intervallo: 18–110

### Anni dalla cessazione (ex fumatore)

`parou`

anni · facoltativo · intervallo: 0–80

## Edizione del metodo

Pacchetti di 20 sigarette; pacchetti-anno; USPSTF 2021: 50–80 anni, ≥20 pacchetti-anno, cessazione≤15 anni

## Formula documentata

Pacchetti-anno = (sigarette/giorno ÷ 20) × anni di fumo. Un pacchetto contiene 20 sigarette.

Screening (USPSTF 2021): TC toracica annuale a bassa dose per adulti di 50–80 anni con ≥ 20 pacchetti-anno, fumatori attuali o cessazione da ≤ 15 anni.

## Limiti e popolazione

I criteri USPSTF 2021 riguardano lo screening annuale mediante TC a bassa dose negli adulti di 50–80 anni con una storia di almeno 20 pacchetti-anno, fumatori attuali o che hanno smesso negli ultimi 15 anni. La raccomandazione prevede anche di interrompere lo screening dopo 15 anni senza fumare o quando le condizioni di salute limitano sostanzialmente l’aspettativa di vita o la capacità/disponibilità a sottoporsi a chirurgia polmonare curativa. Il calcolo dei pacchetti-anno non valuta queste condizioni cliniche.

## Riferimenti

- [US Preventive Services Task Force; Krist AH et al. Screening for lung cancer: US Preventive Services Task Force recommendation statement. JAMA, 2021.](https://doi.org/10.1001/jama.2021.1117)

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

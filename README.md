# Codice sconto Comet, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Comet** da [shopilo.it](https://shopilo.it/negozi/comet.it). Restituisce **coupon Comet** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-comet](https://shopilo-it.github.io/codice-sconto-comet/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-comet
cd codice-sconto-comet
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Comet",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su smartphone e accessori",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/comet.it"
  }
]
```

## Coupon Comet disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su smartphone e accessori | [shopilo.it](https://shopilo.it/negozi/comet.it) |

Codici attivi: **[shopilo.it/negozi/comet.it](https://shopilo.it/negozi/comet.it)**

## Domande frequenti

### Come utilizzo un codice sconto Comet?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/comet.it), aggiungi i prodotti al carrello su Comet e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Comet?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Comet piu recenti?
La pagina [shopilo.it/negozi/comet.it](https://shopilo.it/negozi/comet.it) viene aggiornata quotidianamente con i codici sconto Comet, voucher Comet e coupon promozionali Comet piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Comet

Comet e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/comet.it) trovi i migliori codici sconto Comet, coupon Comet verificati e voucher Comet attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-comet
```

```javascript
const { fetchCoupons } = require('codice-sconto-comet');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)

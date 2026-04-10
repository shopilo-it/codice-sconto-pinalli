# Codice sconto Pinalli, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Pinalli** da [shopilo.it](https://shopilo.it/negozi/pinalli.it). Restituisce **coupon Pinalli** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-pinalli](https://shopilo-it.github.io/codice-sconto-pinalli/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-pinalli
cd codice-sconto-pinalli
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Pinalli",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su cosmetici e profumi",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/pinalli.it"
  }
]
```

## Coupon Pinalli disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su cosmetici e profumi | [shopilo.it](https://shopilo.it/negozi/pinalli.it) |

Codici attivi: **[shopilo.it/negozi/pinalli.it](https://shopilo.it/negozi/pinalli.it)**

## Domande frequenti

### Come utilizzo un codice sconto Pinalli?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/pinalli.it), aggiungi i prodotti al carrello su Pinalli e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Pinalli?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Pinalli piu recenti?
La pagina [shopilo.it/negozi/pinalli.it](https://shopilo.it/negozi/pinalli.it) viene aggiornata quotidianamente con i codici sconto Pinalli, voucher Pinalli e coupon promozionali Pinalli piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Pinalli

Pinalli e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/pinalli.it) trovi i migliori codici sconto Pinalli, coupon Pinalli verificati e voucher Pinalli attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-pinalli
```

```javascript
const { fetchCoupons } = require('codice-sconto-pinalli');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)

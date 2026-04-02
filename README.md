# Cod reducere evoMAG — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere evoMAG** de pe [shopilo.ro](https://shopilo.ro/magazin/evomag.ro). Returneaza **cupoane evoMAG** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-evomag](https://shopilo-ro.github.io/cod-reducere-evomag/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-evomag
cd cod-reducere-evomag
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "evoMAG",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% reducere la toata comanda",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/evomag.ro"
  }
]
```

## Cupoane evoMAG disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 10% | 10% reducere la toata comanda | [shopilo.ro](https://shopilo.ro/magazin/evomag.ro) |

Codurile active: **[shopilo.ro/magazin/evomag.ro](https://shopilo.ro/magazin/evomag.ro)**

## Intrebari frecvente

### Cum folosesc un cod de reducere evoMAG?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/evomag.ro), adauga produsele in cos pe evoMAG, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele evoMAG?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri evoMAG?
Pagina [shopilo.ro/magazin/evomag.ro](https://shopilo.ro/magazin/evomag.ro) este actualizata zilnic cu cele mai noi cod reducere evoMAG, voucher evoMAG si cupon promotional evoMAG.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre evoMAG

evoMAG este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/evomag.ro) cele mai bune cod reducere evoMAG, cupoane evoMAG verificate si voucher evoMAG active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-evomag
```

```javascript
const { fetchCoupons } = require('cod-reducere-evomag');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)

# Code promo Courir, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Courir** depuis [shopilo.fr](https://shopilo.fr/reductions/courir.com). Renvoie les **coupons Courir** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-courir](https://shopilo-fr.github.io/code-promo-courir/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-courir
cd code-promo-courir
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Courir",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les sneakers",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/courir.com"
  }
]
```

## Coupons Courir disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les sneakers | [shopilo.fr](https://shopilo.fr/reductions/courir.com) |

Codes actifs : **[shopilo.fr/reductions/courir.com](https://shopilo.fr/reductions/courir.com)**

## Questions frequentes

### Comment utiliser un code promo Courir ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/courir.com), ajoutez les produits a votre panier sur Courir et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Courir ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Courir les plus recents ?
La page [shopilo.fr/reductions/courir.com](https://shopilo.fr/reductions/courir.com) est mise a jour quotidiennement avec les codes promo Courir, bons de reduction Courir et coupons promotionnels Courir les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Courir

Courir est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/courir.com), retrouvez les meilleurs codes promo Courir, coupons Courir verifies et bons de reduction Courir actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-courir
```

```javascript
const { fetchCoupons } = require('code-promo-courir');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)

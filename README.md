# Analyse de Portefeuille — CAC 40 (2024)

## Description
Analyse financière comparative de 5 actions du CAC 40 en 2024. 
Projet Python d'exploration de données boursières, extraction via API et visualisation des indicateurs clés (rendements, volatilité).

**Objectif** : Analyser les performances et caractéristiques de risque/rendement pour 5 valeurs majeures du marché français.

## Actions analysées

- **TotalEnergies (TTE)** — Énergie
- **BNP Paribas (BNP)** — Finance
- **Airbus (AIR)** — Aéronautique
- **LVMH (MC)** — Luxe
- **Sanofi (SAN)** — Pharmacie
  
## Méthodologie

### Données
- **Source** : Yahoo Finance API (yfinance)
- **Période** : 01/01/2024 - 31/12/2024
- **Fréquence** : Données quotidiennes

### Calculs
1. **Rendement annualisé** : (Prix final - Prix initial) / Prix initial × 100
2. **Volatilité annualisée** : Écart-type des rendements quotidiens × √252
3. **Rendements quotidiens** : log(Prix t / Prix t-1)

### Visualisations
- Évolution des prix normalisés
- Distribution des rendements
- Comparaison volatilité/rendement


## Résultats clés (2024)
| Action | Rendement | Volatilité |
|---|---|---|
| TotalEnergies | +13.44% | 23.23% |Meilleure performance |
| LVMH | +8.65% | 17.81% |Bon ratio risque/rendement |
| BNP Paribas | +2.50% | 23.29% |Faible rendement  |
| Airbus | -6.88% | 28.66% |Négatif & volatil |
| Sanofi | -9.31% | 19.16% | Pire performance |


## Installation & Utilisation

### Prérequis
```bash
pip install pandas yfinance matplotlib seaborn
```

### Lancer l'analyse
```bash
jupyter notebook analyse_portefeuille_cac40.ipynb
```

Ou en Python :
```python
python analyse_portefeuille_cac40.py
```

---

##  Fichiers du projet
- `analyse_portefeuille_cac40.ipynb` — Notebook complet avec analyses
- `analyse_cac40.png` — Graphique des résultats
- `README.md` — Ce fichier

---

##  Limitations
- Analyse sur 1 an seulement (ne reflète pas les tendances long terme)
- Ne considère pas les dividendes
- Pas d'analyse des corrélations entre valeurs
- Données ajustées Yahoo Finance (peut avoir des décalages)

---


##  Améliorations futures
- [ ] Ajouter corrélations intra-portefeuille
- [ ] Intégrer rendement du dividende
- [ ] Backtesting stratégies simples
- [ ] Élargir à 20+ actions du CAC 40
- [ ] Analyse sectorielle

---

## 👤 Auteure
**Ibtissem Lagha**  
 Intéressée par : Data Analysis | Python | Visualisation  
 [LinkedIn](https://linkedin.com/in/ibtissem-lagha-741865336)

---

## 📝 Notes
Projet personnel pour développer compétences en analyse de données et Python.

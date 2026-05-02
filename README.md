# Analyse de Portefeuille CAC 40 : Performance & Risque (2024)

## Description

Analyse financière comparative de 5 actions du CAC 40 en 2024. Ce projet ne se contente pas d'extraire des chiffres : il vise à transformer des données boursières brutes en insights stratégiques pour comprendre la dynamique risque/rendement du marché français.

**Objectif** : Déterminer quels actifs ont réellement créé de la valeur en 2024 en neutralisant le "bruit" de la volatilité.
---
## Actions analysées

- **TotalEnergies (TTE)** — Énergie
- **BNP Paribas (BNP)** — Finance
- **Airbus (AIR)** — Aéronautique
- **LVMH (MC)** — Luxe
- **Sanofi (SAN)** — Pharmacie
- 
  ---
  
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

---
## Résultats clés (2024)

| Action | Rendement | Volatilité |Diagnostic Analyste|
|---|---|---|
| TotalEnergies | +13.44% | 23.23% |Meilleure performance |Top Performer : Capte la hausse du secteur énergie avec une volatilité maîtrisée.|
| LVMH | +8.65% | 17.81% |Bon ratio risque/rendement |Profil Défensif : Meilleure résilience du panel face aux turbulences de marché.|
| BNP Paribas | +2.50% | 23.29% |Faible rendement  |Inertie : Une volatilité quasi identique à TotalEnergies pour un gain 5x inférieur.|
| Airbus | -6.88% | 28.66% |Négatif & volatil |Risque Maximal : Performance négative accentuée par la plus forte instabilité du groupe.|
| Sanofi | -9.31% | 19.16% | Pire performance |Baisse Structurelle : Faible volatilité mais incapacité à générer du rendement.|

Le constat métier : L'analyse révèle que le prix d'une action ne fait pas tout. Airbus est l'actif le plus "dangereux" de 2024, tandis que LVMH confirme son statut de valeur refuge avec le risque le plus bas.

---
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

=> Biais temporel : Une analyse sur 12 mois est insuffisante pour conclure sur la solidité à long terme d'une entreprise.
=> Dividendes : Le CAC 40 étant un indice à dividendes élevés, leur omission sous-évalue le rendement réel pour l'investisseur (notamment pour TTE et SAN).
=> Indépendance : Ce modèle suppose que les actions sont indépendantes, or elles réagissent souvent en bloc aux annonces de la BCE.

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

 Future apprentie Data Analyst & BI — Curieuse de comprendre les histoires que cachent les chiffres.
 [LinkedIn](https://linkedin.com/in/ibtissem-lagha-741865336)

---

## 📝 Notes
Projet personnel pour développer compétences en analyse de données et Python.

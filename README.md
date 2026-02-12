# Analyse des ventes d’une PME – Projet Dev IA

## Contexte

Ce projet a pour objectif de réaliser une première analyse des ventes d’une PME à partir d’un extrait de données couvrant 20 jours d’activité.

L’analyse repose sur :
- SQL pour l’exploration et les calculs
- Python (Pandas + Plotly) pour la visualisation

---

## Données

Le jeu de données contient les colonnes suivantes :

- date  
- produit  
- prix  
- qte  
- region  

Hypothèse de calcul :  
Le chiffre d’affaires est défini comme :

CA = prix × qte

---

## Analyses SQL réalisées

Les requêtes SQL ont été exécutées sur sqliteonline et exportées.
Elles permettent de répondre aux questions suivantes :

1. Chiffre d’affaires total  
2. Ventes par produit (volume et chiffre d’affaires)  
3. Ventes par région (volume et chiffre d’affaires)  

Les requêtes sont disponibles dans :
`sql/queries.sql`

Les résultats synthétisés sont présentés dans :
`docs/fiche_synthese.md`

---

## Visualisations Python

Trois graphiques ont été développés à l’aide de Plotly :

- Ventes (volume) par région 
- Volume des ventes par produit  
- Chiffre d’affaires par produit  

Pour générer les visualisations :

```bash
python3 app.py
```

---

## Structure du projet

Les fichiers HTML générés se trouvent dans :

`outputs/`

```
.
├── app.py
├── data/
│  └── ventes.csv
├── requirements.txt
├── sql/
│  └── queries.sql
├── docs/
│  └── fiche_synthese.md
├── outputs/
│  ├── ventes-par-region.html
│  ├── volume-par-produit.html
│  └── ca-par-produit.html
```

---

## Technologies utilisées
- Python 3  
- Pandas  
- Plotly  
- SQLite (sqliteonline)

Ce projet peut être exécuté localement (via Python 3 et `requirements.txt`) ou directement dans GitHub Codespaces grâce au dossier `.devcontainer`.

---

## Synthèse

Cette analyse permet :

- d’identifier les produits les plus performants,
- de comparer volume vendu et rentabilité,
- de repérer les régions générant le plus de chiffre d’affaires.

Le projet répond aux livrables demandés : export SQL, fiche synthèse et dépôt GitHub complété avec visualisations.



# GridMind — Intelligent Energy Forecasting & Optimization Platform

## 1. Contexte

Le système électrique français produit de grandes quantités de données relatives à la consommation, à la production d’électricité, aux énergies renouvelables, aux échanges énergétiques et aux émissions de CO₂.

Les données ouvertes de RTE et les données météorologiques permettent d’étudier le comportement du système électrique français et de construire des modèles de prévision et d’aide à la décision.

## 2. Problématique

Comment utiliser les données énergétiques et météorologiques pour prévoir la consommation électrique française, détecter les comportements inhabituels et recommander les meilleurs créneaux pour consommer de l’électricité ?

## 3. Objectif général

Construire une plateforme de Data Engineering et de Machine Learning capable de :

- collecter et préparer des données énergétiques réelles ;
- prévoir la consommation électrique nationale ;
- comparer plusieurs méthodes de prévision ;
- détecter les consommations inhabituelles ;
- identifier les créneaux ayant une faible intensité carbone ;
- recommander un planning de consommation optimisé ;
- présenter les résultats dans une application simple.

## 4. Utilisateurs visés

La plateforme pourra être utilisée par :

- un analyste énergétique ;
- une entreprise souhaitant déplacer certaines consommations ;
- un gestionnaire énergétique ;
- un étudiant ou chercheur étudiant le système électrique ;
- un décideur souhaitant comprendre les prévisions et les anomalies.

## 5. Résultat principal attendu

L’utilisateur sélectionne une date ou une période.

La plateforme affiche :

- la consommation électrique historique ;
- la consommation prévue pour les prochaines 24 heures ;
- les écarts entre les valeurs réelles et prévues ;
- les anomalies détectées ;
- les créneaux recommandés pour consommer avec une intensité carbone plus faible.

## 6. Périmètre géographique

La première version concerne la France au niveau national.

Les données régionales pourront être intégrées dans une version future.

## 7. Granularité temporelle

Les données seront analysées avec une granularité de 30 minutes lorsque les sources le permettent.

## 8. Sources envisagées

- RTE / Open Data Réseaux Énergies ;
- Météo-France ;
- calendrier des jours fériés ;
- calendrier des vacances scolaires.

## 9. Contraintes

- le projet est réalisé par RIHAM KADDOUR BAKIR ;
- les données utilisées doivent être accessibles légalement ;
- les sources et licences doivent être mentionnées ;
- les résultats des modèles doivent être évalués ;
- les données futures ne doivent pas être utilisées pour prédire le passé ;
- le projet doit être reproductible et documenté.

## 10. Technologies envisagées

- Python ;
- SQL ;
- Pandas ou Polars ;
- Parquet ;
- PostgreSQL ;
- Scikit-learn ;
- LightGBM ou XGBoost ;
- MLflow ;
- FastAPI ;
- Streamlit ou React ;
- Git et GitHub ;
- Docker.

## 11. Critères de réussite

Le projet sera considéré comme réussi si :

- les données sont récupérées automatiquement ;
- les données sont nettoyées et contrôlées ;
- une baseline de prévision est disponible ;
- un modèle de Machine Learning est comparé à la baseline ;
- la validation respecte l’ordre temporel ;
- les prévisions sont accessibles par une API ;
- les résultats sont présentés dans une interface ;
- le projet peut être exécuté à partir de sa documentation.


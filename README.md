# GridMind

GridMind est une plateforme de prévision et d’optimisation du système électrique français.

## Objectifs

- collecter et préparer des données énergétiques réelles ;
- prévoir la consommation électrique nationale ;
- détecter les comportements inhabituels ;
- identifier les créneaux les moins carbonés ;
- optimiser une consommation sous contraintes ;
- présenter les résultats dans une application.

## Sources prévues

- RTE / Open Data Réseaux Énergies ;
- Météo-France ;
- calendrier des jours fériés et vacances scolaires.

## Périmètre du MVP

La première version prévoit la consommation électrique nationale à 24 heures, détecte les écarts inhabituels et recommande des créneaux de consommation bas-carbone.

## Architecture cible

Sources → Ingestion → Stockage → Feature Engineering → Modèles → API → Application

## Statut

Projet en cours de cadrage.

## Avertissement

GridMind est un projet étudiant. Les prévisions et recommandations fournies ne doivent pas être utilisées comme seules bases pour une décision opérationnelle critique.

## Données et licences

Les données restent la propriété de leurs producteurs respectifs. Les sources, licences et conditions de réutilisation seront indiquées dans la documentation du projet.

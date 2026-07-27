# Périmètre du MVP GridMind

## Fonctionnalités obligatoires

### 1. Collecte des données

- récupérer les données historiques de RTE ;
- récupérer les données météorologiques nécessaires ;
- récupérer les jours fériés ;
- conserver les données originales.

### 2. Préparation des données

- nettoyer les données ;
- harmoniser les dates ;
- contrôler les doublons ;
- traiter les valeurs manquantes ;
- joindre les données énergétiques, météorologiques et calendaires ;
- créer un dataset destiné au Machine Learning.

### 3. Prévision de consommation

- construire une baseline basée sur la semaine précédente ;
- construire un modèle LightGBM ou XGBoost ;
- prévoir la consommation des prochaines 24 heures ;
- comparer les résultats avec MAE, RMSE et WAPE.

### 4. Détection d’anomalies

- comparer la consommation observée à la consommation attendue ;
- attribuer un niveau de gravité aux écarts ;
- afficher les anomalies dans l’application.

### 5. Recommandation bas-carbone

- utiliser l’intensité carbone disponible ou estimée ;
- identifier les créneaux futurs les moins carbonés ;
- recommander un créneau de consommation.

### 6. Restitution

- exposer les résultats par une API FastAPI ;
- créer une interface simple ;
- documenter les sources, modèles et limites ;
- exécuter le projet avec Docker.

## Fonctionnalités reportées après le MVP

- prévision solaire ;
- prévision éolienne ;
- clustering des régimes énergétiques ;
- modèle LSTM ;
- Transformer temporel ;
- déploiement Kubernetes ;
- assistant conversationnel ;
- analyse régionale ;
- prédiction des prix de l’électricité.

## Règle du projet

Une fonctionnalité du MVP doit être terminée, testée et documentée avant de commencer une fonctionnalité optionnelle.

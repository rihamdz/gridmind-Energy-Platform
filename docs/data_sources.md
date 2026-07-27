# Sources de données — GridMind

## 1. RTE — éCO₂mix national consolidé

### Producteur

RTE — Réseau de Transport d’Électricité

### Utilisation dans GridMind

Les données RTE seront utilisées pour :

- analyser la consommation électrique française ;
- prévoir la consommation des prochaines 24 heures ;
- analyser la production nucléaire, hydraulique, éolienne et solaire ;
- étudier les échanges d’électricité ;
- analyser ou prévoir les émissions de CO₂ ;
- détecter les comportements énergétiques inhabituels.

### Données recherchées

- date et heure ;
- consommation réelle ;
- consommation prévue à J-1 ;
- consommation prévue à J ;
- production nucléaire ;
- production hydraulique ;
- production éolienne ;
- production solaire ;
- production thermique ;
- échanges physiques ;
- taux ou émissions de CO₂.

### Granularité attendue

Une observation toutes les 30 minutes.

### Format envisagé

- CSV ;
- JSON via API ;
- Parquet après transformation.

### Portail

Open Data Réseaux Énergies — ODRÉ

### Licence

Licence Ouverte version 2.0 — Etalab.

### Citation prévue

Source : RTE, données éCO₂mix disponibles sur le portail Open Data Réseaux Énergies.

### Précautions

- préserver les données originales dans la zone Bronze ;
- ne pas modifier les fichiers sources ;
- enregistrer la date de téléchargement ;
- conserver le nom du jeu de données ;
- vérifier les unités de mesure ;
- vérifier les conditions inscrites sur la fiche officielle du jeu de données.


## 2. Météo-France

### Producteur

Météo-France

### Utilisation dans GridMind

Les données météorologiques seront utilisées pour améliorer les prévisions de :

- consommation électrique ;
- production solaire ;
- production éolienne.

### Données recherchées

- date et heure ;
- température ;
- vitesse du vent ;
- direction du vent ;
- rayonnement solaire ;
- nébulosité ;
- humidité, si elle est pertinente.

### Format envisagé

- API ;
- CSV ;
- JSON ;
- Parquet après transformation.

### Licence

La licence exacte devra être vérifiée sur la fiche du jeu de données utilisé.

### Citation prévue

Source : Météo-France.

### Précautions

- distinguer la météo observée de la météo prévue ;
- vérifier la fréquence des observations ;
- vérifier les unités ;
- vérifier la couverture géographique ;
- conserver la source et la date d’extraction.


## 3. Jours fériés

### Producteur envisagé

API officielle du gouvernement français.

### Utilisation dans GridMind

Identifier si une date correspond à un jour férié, car les jours fériés peuvent modifier la consommation électrique.

### Données recherchées

- date ;
- nom du jour férié ;
- zone géographique.

### Variable finale

is_holiday :

- 1 si le jour est férié ;
- 0 sinon.

### Licence

À vérifier sur la fiche officielle de l’API.

### Citation prévue

Source : data.gouv.fr.

## 4. Vacances scolaires

### Producteur envisagé

Ministère de l’Éducation nationale / data.gouv.fr.

### Utilisation dans GridMind

Identifier les périodes de vacances scolaires susceptibles d’influencer la consommation électrique.

### Données recherchées

- date de début ;
- date de fin ;
- zone académique ;
- description de la période.

### Variable finale

is_school_holiday :

- 1 si la date appartient à une période de vacances ;
- 0 sinon.

### Licence

À vérifier sur la fiche officielle du jeu de données.

### Citation prévue

Source : Ministère de l’Éducation nationale / data.gouv.fr.

## 5. Règles générales de traçabilité

Pour chaque extraction, GridMind conservera :

- le nom du producteur ;
- le nom du jeu de données ;
- l’adresse de la source ;
- la licence ;
- la date et l’heure d’extraction ;
- la période couverte ;
- le nombre de lignes récupérées ;
- le format du fichier ;
- le nom du fichier original.

Les données originales seront conservées sans modification dans la zone Bronze.

Les transformations seront réalisées dans les zones Silver et Gold.

## 6. Sources non encore retenues

Les sources suivantes pourront être étudiées après le MVP :

- prix de l’électricité ;
- données énergétiques régionales ;
- données de consommation par secteur ;
- données européennes ENTSO-E ;
- facteurs d’émission complémentaires.

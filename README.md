## Fuel prices per type in France visualisation and prediction
> This project aims at understanding how fuel prices evolved over time per type and per station in France. All data is available online. This project was primarly developed on Google Colab for a school project. The purpose of this project is to have a first use of Pyspark for data management and prediction processes. Language used for commentary is French.

## Data source
> All data are available online. Choropleth segmentation were obtained via https://france-geojson.gregoiredavid.fr

## Script structure
#### QUESTION 1 : Préparation des données - étape 1
1) Lire et fusionner les fichiers carburants (Prix)
2) Fractionner la date en heure, année et semaine
3) Rendre les données disponibles sous forme de tableau afin de pouvoir utiliser Spark SQL
4) Statistiques de base et carburants ayant le moins d'intérêts
   
#### QUESTION 2 : Préparation des données - étape 2
1) Calculer l'indice des prix / jour / carburant
2) Calculer l'indice de la semaine
   
#### QUESTION 3 : Visualisation des données
1) Grouper par carburant et index de la semaine pour obtenir la moyenne des prix/semaine
2) Obtenir l'information mois/année des index semaines
3) Affichage avec seaborn et matplotlib
   
#### BONUS : Visualisation des données
1) Grouper par codes postaux, nom de caburant et d'année
2) Rajouter des 0 pour les codes postaux à 4 positions pour créer une colonne de code de département
3) Obtenir automatiquement des arrays des années et des noms de carburants
4) Accéder aux départements via la source https://france-geojson.gregoiredavid.fr
5) Créer une carte interactive
6) Itérer l'affichage des carburants par année
   
#### QUESTION 4 : Modélisation - Prévision du prix le lendemain
1) Préparation des données
2) Régression linéaire
3) Random Forest

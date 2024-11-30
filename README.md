##Prédiction de l'infection par le SARS-CoV-2 (COVID-19)
#Description du projet
Ce projet vise à analyser des données médicales pour prédire si un individu est infecté par le SARS-CoV-2 (COVID-19) en fonction de divers paramètres biologiques et viraux. À travers une combinaison de nettoyage de données, d'ingénierie des caractéristiques et de machine learning, un modèle prédictif a été développé pour fournir des diagnostics précis.

#Objectif
- Identifier les variables les plus significatives pour prédire l'infection.
- Construire et évaluer un modèle de machine learning performant pour classer les résultats des tests en positif ou négatif.
- Fournir un outil pour l’aide au diagnostic médical.
#Données utilisées
- Source des données : Un fichier Excel contenant des informations cliniques et biologiques de patients.
- Colonnes clés :
Résultat du test SARS-CoV-2 (SARS-Cov-2 exam result).
Variables biologiques telles que Monocytes, Leukocytes, et Platelets.
Variables virales.
#Étapes principales
1. Exploration et nettoyage des données
Analyse initiale :
Vérification des types de données.
Inspection des valeurs manquantes (seuil : 90 % de valeurs manquantes).
Visualisations :
Distribution des variables pour les résultats positifs et négatifs.
Analyse des variables les plus discriminantes.
2. Prétraitement des données
Encodage :
Transformation des valeurs catégoriques (ex. positive → 1, negative → 0).
Ingénierie des caractéristiques :
Ajout de nouvelles colonnes, telles que est malade, basée sur les résultats viraux.
Imputation :
Gestion des valeurs manquantes avec des approches adaptées.
3. Modélisation et évaluation
Modèle utilisé : Support Vector Machine (SVM) avec recherche d'hyperparamètres via RandomizedSearchCV.
Entraînement et test :
Division des données en ensembles d'entraînement et de test (80 %/20 %).
Évaluation des performances à l'aide de métriques telles que la précision, le rappel, et l'AUC-ROC.
4. Courbe précision-rappel
Analyse de la courbe précision-rappel pour ajuster le seuil de décision du modèle en fonction des besoins spécifiques.

📊 Analyse des dépenses annuelles des clients
🎯 Objectif du projet

Ce projet vise à analyser et prédire la dépense annuelle des clients à partir de variables démographiques, professionnelles et financières (âge, revenu mensuel, ancienneté, type de contrat, secteur, région).

L’objectif est double :

comprendre la structure des données et les relations entre les variables

construire un modèle de régression capable d’estimer la dépense annuelle

Ce dépôt correspond à une version enrichie du projet initial, avec l’ajout de visualisations et de sorties détaillées du modèle.

📘 Projet initial (description complète)

La description détaillée du contexte, de la problématique et de la méthodologie initiale est disponible ici :
👉 https://github.com/souleymane2021/projet_ml_depense_annuelle

Le fond de l’analyse et l’interprétation principale du modèle (notamment du R²) restent identiques.

🧹 Nettoyage et préparation des données

Les étapes suivantes ont été appliquées :

suppression des doublons

traitement des valeurs manquantes :

moyenne pour les variables numériques

modalité la plus fréquente pour les variables catégorielles

correction des valeurs incohérentes (revenus négatifs)

séparation des variables numériques et catégorielles

normalisation et standardisation adaptées aux types de variables

encodage des variables catégorielles (OneHotEncoder)

Ces étapes garantissent des données cohérentes et exploitables par le modèle.

📊 Analyse descriptive et visualisation
🔹 Statistiques descriptives

Les statistiques descriptives (moyenne, écart-type, minimum, maximum, quartiles) permettent de :

observer la dispersion des variables numériques

identifier les variables présentant une forte variabilité

mieux comprendre l’échelle des données avant modélisation

🔹 Distributions des variables numériques

Les histogrammes par classes montrent que :

certaines variables sont concentrées sur des intervalles précis

d’autres présentent une dispersion plus large, indiquant des profils clients variés

Cela justifie l’utilisation de techniques de normalisation.

🔹 Corrélations

La matrice de corrélation met en évidence :

des relations plus ou moins fortes entre certaines variables numériques

une corrélation variable avec la dépense annuelle

Ces observations suggèrent que la dépense annuelle dépend de plusieurs facteurs combinés, et pas d’une seule variable.

🔹 Variables catégorielles

Les barplots permettent de visualiser :

la répartition des clients selon le type de contrat, le secteur et la région

d’éventuels déséquilibres entre catégories

Ces informations sont importantes pour interpréter les prédictions du modèle.

🔹 Relation avec la variable cible

Les scatter plots entre chaque variable numérique et la dépense annuelle montrent :

des tendances globales, mais non strictement linéaires

une dispersion importante, indiquant la complexité du comportement client

La courbe triée de la dépense annuelle met en évidence une forte hétérogénéité entre les clients.

🤖 Modélisation

Un Random Forest Regressor a été utilisé au sein d’un pipeline incluant :

le prétraitement des données

l’entraînement du modèle

l’évaluation sur un jeu de test

🔹 Métriques d’évaluation

Les métriques utilisées sont :

MAE (Mean Absolute Error)

MSE (Mean Squared Error)

RMSE (Root Mean Squared Error)

R² (coefficient de détermination)

Le coefficient R² indique la proportion de la variance de la dépense annuelle expliquée par le modèle, ce qui permet d’évaluer sa capacité prédictive globale.

🔮 Prédictions

Le modèle est également utilisé pour prédire la dépense annuelle de nouveaux clients à partir de leurs caractéristiques.

Ces prédictions illustrent :

l’utilisation concrète du modèle

sa capacité à généraliser à de nouveaux profils clients

🧠 Conclusion

Ce projet montre :

une démarche complète de machine learning en régression

l’importance de l’exploration visuelle des données

l’intérêt de combiner analyse descriptive, visualisation et modélisation

La version actuelle met l’accent sur la lisibilité, la reproductibilité et la compréhension des résultats, tout en conservant la méthodologie du projet initial.

🔧 Technologies utilisées

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

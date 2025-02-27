# Projet d'Analyse de Données de Santé et Bien-être

##  Description du Projet
Ce projet vise à analyser un dataset contenant divers **indicateurs de santé, bien-être et vie quotidienne** afin de **classifier les individus en trois catégories** selon leur état de santé.
## Objectif :
Optimiser la classification des individus et analyser les tendances de santé à partir des données disponibles. Identifier les profils **à risque** et mieux comprendre l’impact des différents facteurs sur l’état de santé.

##  Structure du Dataset
Le dataset comporte **10 000 observations** et **20 variables explicatives** représentant des indicateurs clés tels que :
- **Âge, Taille, Poids, Revenu, Expérience, Niveau d'éducation**
- **IMC (Indice de Masse Corporelle), Niveau de stress, Nombre d'enfants, Dépenses**
- **Exercice physique, Alimentation, Sommeil, Pression artérielle, Cholestérol**
- **Activité physique, Satisfaction, Risque global**

La variable **`target`** est la **variable cible** et représente la classification des individus en **trois catégories** :
- **Classe 0 : Sain et Actif** 🟢
- **Classe 1 : Modéré** 🟡
- **Classe 2 : À Risque** 🔴

## Étapes de l'Analyse
### ** Prétraitement des Données**
- Séparation des **variables explicatives et de la cible**.
- **Standardisation** des données (centrage-réduction) avec `StandardScaler`.
- **Affichage de la matrice de corrélation** pour analyser les relations entre les variables.

### ** Réduction de Dimension avec PCA**
- **Application de la PCA** pour conserver **95% de la variance**.
- **Visualisation de la variance expliquée** par chaque composante principale.

### ** Modélisation Supervisée**
- **Régression Logistique** avec **validation croisée**.
- **Prédictions et Matrice de Confusion**.
- **Évaluation des performances** avec précision, rappel et F1-score.
- **Affichage de la Courbe ROC** pour analyser la qualité du modèle.

### ** Visualisation du PCA**
- **Projection des données en 2D et 3D** avec les trois classes colorées.

### ** Optimisation des Modèles avec Grid Search**
- **KNN (K-Nearest Neighbors)** avec recherche du **meilleur K impaire**.
- **Arbre de décision** avec **optimisation de la profondeur (`max_depth`) et des feuilles (`min_samples_leaf`)**.
- **Affichage de l'arbre de décision final**.

### ** Clustering Non Supervisé avec K-Means**
- **Méthode du coude** pour choisir **le nombre optimal de clusters K**.
- **Application de K-Means et visualisation des résultats**.

### Outils et Librairies Utilisées
- **Python 3.x**
- `pandas`, `numpy` : Manipulation des données
- `matplotlib`, `seaborn` : Visualisation des données
- `sklearn` : Machine Learning (PCA, Régression Logistique, KNN, Arbre de décision, K-Means)


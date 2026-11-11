# Machine Learning Projects

Ce dépôt contient une série de notebooks de machine learning et d'intelligence artificielle couvrant les concepts fondamentaux ainsi que des applications concrètes sur différents types de données : données tabulaires, images et texte.

Les notebooks ont été conçus pour explorer, comprendre et mettre en pratique les méthodes de data science et de deep learning, avec un accent sur l'analyse exploratoire, l'ACP, les réseaux de neurones, les CNN et les RNN.

## Sommaire

- [Présentation du projet](#présentation-du-projet)
- [Contenu du dépôt](#contenu-du-dépôt)
- [Objectifs pédagogiques](#objectifs-pédagogiques)
- [Technologies utilisées](#technologies-utilisées)
- [Pré-requis](#pré-requis)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Données utilisées](#données-utilisées)
- [Structure du projet](#structure-du-projet)
- [Notes et recommandations](#notes-et-recommandations)

## Présentation du projet

Ce projet regroupe plusieurs exercices et travaux pratiques autour du machine learning, avec une progression logique qui suit les étapes classiques d'un projet IA :

1. Analyse exploratoire des données
2. Préparation et nettoyage des données
3. Réduction de dimensions (ACP)
4. Modélisation supervisée
5. Réseaux de neurones artificiels
6. CNN pour l'analyse d'images
7. RNN pour l'analyse de textes et des sentiments

L'objectif est d'apprendre à manipuler des datasets réels et à appliquer des méthodes de pointe dans un environnement Python, avec une forte dimension pédagogique.

## Contenu du dépôt

### 1. 01_data_exploration.ipynb
Notebook dédié à l'exploration d'un dataset de détection de fraude bancaire.

Il inclut :
- chargement du dataset via KaggleHub
- inspection des colonnes et du schéma des données
- statistiques descriptives
- analyse des valeurs manquantes
- visualisation des distributions et des relations
- préparation des données pour une étape de modélisation

### 2. DIAK_test1.ipynb
Travail sur la réduction de dimensions par Analyse en Composantes Principales (ACP).

Il couvre :
- chargement du dataset digits de scikit-learn
- visualisation des chiffres manuscrits
- standardisation des variables
- application de l'ACP
- interprétation de la variance expliquée
- visualisation des données dans l'espace PCA

### 3. DIAK_test2.ipynb
Travail pratique sur les réseaux de neurones artificiels (ANN) pour un problème de classification binaire.

Le dataset utilisé est le dataset Breast Cancer Wisconsin, avec un modèle de classification permettant de distinguer les tumeurs malignes et bénignes.

Les aspects abordés :
- chargement et compréhension du dataset
- séparation train / test
- normalisation des caractéristiques
- construction d'un réseau de neurones
- évaluation des performances
- interprétation des résultats

### 4. DIAK_test3.ipynb
Travail pratique sur les réseaux de neurones convolutifs (CNN) appliqués aux images du dataset MNIST.

Il inclut :
- chargement des images du dataset MNIST
- visualisation de quelques chiffres
- redimensionnement des images
- ajout de la dimension de canal (grayscale)
- normalisation des pixels
- création d'un modèle CNN
- entraînement et évaluation

### 5. DIAK_test4.ipynb
Projet sur les réseaux de neurones récurrents (RNN) pour l'analyse de sentiments sur le dataset IMDB.

Il traite :
- chargement des critiques IMDB
- encodage des mots et padding des séquences
- visualisation des données texte
- création d'un modèle RNN
- apprentissage sur des critiques positives/négatives
- interprétation des performances du modèle

## Objectifs pédagogiques

Ce projet permet de maîtriser plusieurs compétences clés en apprentissage automatique :

- comprendre les données et leur structure
- nettoyer et prétraiter les jeux de données
- utiliser des outils de visualisation pour explorer les distributions et les relations
- appliquer correctement les méthodes de réduction de dimensions
- construire des modèles de classification supervisée
- comprendre les mécanismes des réseaux de neurones
- appliquer les CNN aux données image
- utiliser les RNN pour traiter des séquences textuelles
- évaluer correctement les modèles via des métriques adaptées

## Technologies utilisées

Le projet est principalement développé avec Python et les bibliothèques suivantes :

- Python 3.x
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- KaggleHub

## Pré-requis

Avant de lancer les notebooks, il est recommandé d'avoir :

- un environnement Python 3.9 ou supérieur
- Jupyter Notebook ou JupyterLab installé
- une connexion Internet pour télécharger les datasets depuis Kaggle ou depuis les bibliothèques associées
- un environnement GPU facultatif pour accélérer l'entraînement des modèles CNN/RNN

## Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/diak224-dot/Machine-Learning-Projects.git
cd Machine-Learning-Projects
```

### 2. Créer un environnement virtuel

```bash
python -m venv venv
```

Sur Windows :

```bash
venv\Scripts\activate
```

Sur Linux / macOS :

```bash
source venv/bin/activate
```

### 3. Installer les dépendances

```bash
pip install -U pip
pip install numpy pandas matplotlib seaborn scikit-learn jupyter kagglehub tensorflow
```

> Note : selon votre configuration, TensorFlow peut nécessiter des versions spécifiques selon votre système d'exploitation et votre matériel. Si nécessaire, référez-vous à la documentation officielle de TensorFlow pour choisir la bonne version.

## Utilisation

### Lancer Jupyter

```bash
jupyter notebook
```

ou

```bash
jupyter lab
```

Ensuite, ouvrez le notebook souhaité dans le navigateur et exécutez les cellules dans l'ordre.

### Ouvrir directement dans Google Colab

Les notebooks peuvent également être ouverts dans Google Colab via les badges intégrés dans les fichiers ipynb.

## Données utilisées

Ce projet exploite plusieurs datasets standards et populaires dans la communauté du machine learning :

- Fraud Detection Dataset (données bancaires / détection de fraude)
- Breast Cancer Wisconsin dataset
- MNIST dataset
- IMDB movie reviews dataset

Ces datasets permettent de couvrir différents types d'apprentissage automatique :

- classification tabulaire
- réduction de dimensions
- vision par ordinateur
- traitement du langage naturel

## Structure du projet

```text
Machine-Learning-Projects/
├── 01_data_exploration.ipynb
├── DIAK_test1.ipynb
├── DIAK_test2.ipynb
├── DIAK_test3.ipynb
├── DIAK_test4.ipynb
├── README.md
└── .gitignore (si ajouté ultérieurement)
```

## Notes et recommandations

- Il est conseillé d'exécuter les notebooks dans l'ordre numérique : `01_data_exploration.ipynb`, puis `DIAK_test1.ipynb`, `DIAK_test2.ipynb`, `DIAK_test3.ipynb`, `DIAK_test4.ipynb`.
- Le projet est pédagogique et conçu pour l'apprentissage progressif des concepts de ML et de deep learning.
- La qualité des résultats dépend fortement du matériel disponible (mémoire RAM, GPU, version des bibliothèques).
- Certaines dépendances peuvent varier selon votre système et selon la version de TensorFlow installée.

## Licence

Ce projet est fourni à des fins pédagogiques. Vérifiez les licences des datasets utilisés et les conditions d'utilisation des bibliothèques tierces selon votre contexte.

## Auteurs

Ce dépôt a été réalisé dans le cadre d'un apprentissage et d'un travail pratique en machine learning et deep learning.

## Conclusion

Ce projet constitue un ensemble de travaux pratiques couvrant les bases et les applications avancées de l'intelligence artificielle. Il est particulièrement utile pour les étudiants, les apprenants en data science et les personnes souhaitant se former aux méthodes de machine learning à travers des exemples concrets et applicatifs.

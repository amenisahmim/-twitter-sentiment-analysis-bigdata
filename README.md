# 🐦 Analyse des Sentiments sur Twitter avec Apache Spark

[![Python](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/)
[![PyPI](https://img.shields.io/pypi/v/pyspark)](https://pypi.org/project/pyspark/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## 🌟 Introduction
Ce projet consiste à **analyser les sentiments des tweets** en utilisant **Apache Spark** pour le traitement distribué et le machine learning.  
Il inclut également une **simulation de streaming** pour effectuer des prédictions en temps réel.

---

## 📁 Structure du projet

- `twitter-sentiment-analysis-spark-nlp.ipynb` : Notebook principal
- `twitter_training.csv` : Dataset (à ajouter localement)
- `requirements.txt` : Dépendances Python
- `.gitignore` : Fichiers ignorés par Git
- `LICENSE` :Licence MIT

---

## 🛠️ Installation

Cloner le dépôt :
git clone https://github.com/amenisahmim/-twitter-sentiment-analysis-bigdata.git

cd analyse-des-sentiments-twitter-bigdata

Installer les dépendances :
pip install -r requirements.txt

---

# 🏗️ Workflow du projet - Analyse des Sentiments sur Twitter

---

## PARTIE 1 : Chargement et exploration des données massives
- Initialisation d'un environnement Spark distribué
- Lecture du fichier CSV `twitter_training.csv`
- Exploration distribuée : statistiques descriptives, distribution des sentiments
- Visualisation avec Matplotlib et Seaborn
- Identification des colonnes principales : `id`, `topic`, `sentiment`, `text`

---

## PARTIE 2 : Manipulation avancée des DataFrames & Spark SQL
- **Nettoyage du texte :**
  - Transformation en minuscules
  - Suppression d'URLs, mentions, hashtags, emojis et caractères spéciaux
  - Mots vides (stopwords) et lemmatisation
- Tokenisation et vectorisation (Bag-of-Words + TF-IDF)
- Analyses avec Spark SQL :
  - Distribution des sentiments et des sujets
  - Longueur moyenne des tweets par sentiment
- Visualisations avancées : boxplots, WordClouds

---

## PARTIE 3 : Stockage distribué et performances
- Sauvegarde des données en JSON et Parquet
- Comparaison des performances : temps de lecture JSON vs Parquet
- Simulation d'un HDFS local pour stockage distribué

---

## PARTIE 4 : Machine Learning distribué
- Transformation des labels textuels en numériques
- Modèles entraînés :
  - Bayes naïf
  - Régression logistique
  - Arbre de décision
  - Forêt aléatoire
- Évaluation : précision, score F1
- Pipeline complet Spark ML pour NLP et classification distribuée

---

## PARTIE 5 : Streaming simulé – Prédiction en temps réel
- Simulation de flux de tweets réalistes
- Nettoyage et vectorisation en temps réel
- Prédiction de sentiment sur chaque tweet
- Affichage dynamique de la distribution des sentiments
- Export des résultats en CSV et stockage simulé HDFS

---

## 📊 Visualisations
- Histogrammes de distribution des sentiments
- Boxplots de longueur de tweets par sentiment
- WordClouds des mots les plus fréquents
- Graphiques en streaming pour le suivi en temps réel

---

## ⚡ Technologies utilisées
- Python 3.10
- Pandas, Matplotlib, Seaborn
- NLTK pour le NLP
- Scikit-learn pour ML classique
- Apache Spark pour traitement distribué et ML
- HDFS local pour stockage distribué
- WordCloud pour visualisation des mots fréquents

---

## 📝 Auteur
**Amani Sahmim** – Étudiante en Ingénierie Systèmes Embarqués & IoT

---

## 📄 Licence
Ce projet est sous licence **MIT** – voir le fichier [LICENSE](LICENSE)

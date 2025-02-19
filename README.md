# README - Analyse de la Survie des Patients VIH

## Introduction
Ce projet vise à analyser la survie des patients atteints du VIH à partir de données longitudinales. L'objectif principal est de comprendre les facteurs influençant la mortalité des patients et d'évaluer l'efficacité de deux traitements antirétroviraux : didanosine (ddI) et zalcitabine (ddC).

Le VIH (Virus de l'Immunodéficience Humaine) affaiblit le système immunitaire en détruisant les cellules CD4, un biomarqueur clé pour surveiller la progression de la maladie. L'étude se concentre sur des patients ayant échoué ou ne tolérant pas la thérapie AZT (zidovudine) et répartis aléatoirement entre les deux traitements alternatifs.

Les principales questions de recherche sont :
- Quels sont les facteurs influençant la survie des patients ?
- Existe-t-il une différence significative entre l'efficacité des traitements ddI et ddC ?
- Quelle est la relation entre le taux de cellules CD4 et le risque de mortalité ?

## Modélisation et méthodologie
### 1. Préparation des données
L'étape initiale consiste à charger et explorer les données afin de s'assurer qu'elles sont correctement formatées et exemptes d'incohérences. Cela inclut la détection et la gestion des valeurs manquantes ainsi que l'élimination des doublons.

Dans ce projet, aucune valeur manquante ni doublon n'a été détecté. Cependant, pour affiner l'analyse statistique, un dataset nommé `unique-data` a été créé en supprimant les colonnes `CD4` et `time-obs`. Cette approche permet d'éviter de compter plusieurs fois les patients en raison des mesures répétées du taux de CD4.

### 2. Statistiques descriptives et visualisation
L'analyse exploratoire des données permet de mieux comprendre la distribution des variables, d'identifier des tendances et de repérer d'éventuelles anomalies avant d'appliquer des modèles plus avancés. Les principales étapes de cette phase incluent :
- Le calcul de statistiques descriptives (moyennes, médianes, écarts-types, etc.).
- La visualisation des données via des histogrammes, des boîtes à moustaches et des courbes de survie.

## Technologies utilisées
- **Langages** : Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Lifelines)
- **Environnement** : Jupyter Notebook
- **Méthodes statistiques** : Modèles de régression de Cox, Kaplan-Meier, tests de comparaison de survie

## Résultats attendus
L'objectif final est d'apporter des réponses précises aux questions de recherche en identifiant les facteurs de risque et en comparant l'efficacité des traitements. Les résultats obtenus pourront être utilisés pour améliorer la prise en charge des patients atteints du VIH.

## Auteurs
Projet réalisé par ATHOUMANI Ibroihima  athoumani.ibroihima@gmail.com .




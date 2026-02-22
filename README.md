# Projet Endrix : Détection Automatique des Aides de l'État

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboarding-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

Pour ce projet, réalisé dans le cadre de mon stage de fin d'études, j'ai travaillé sur une problématique réelle de cabinet d'expertise comptable : **l'optimisation du conseil client.**

> **Note de confidentialité :** Les données présentées dans ce dépôt sont **fictives**. Un générateur de données synthétiques (via la librairie Python `Faker`) a été créé pour simuler la structure réelle du portefeuille du cabinet tout en respectant le secret professionnel.

## Aperçu des données
Ce jeu de données simulé est composé de **100 entreprises** (lignes) et **25 colonnes**.
Il regroupe des informations comptables et structurelles essentielles pour l'analyse :

*   **Identification :** ID, Nom, Secteur d'activité, Statut juridique (SARL, SAS, etc.).
*   **Données Financières :** Chiffre d'affaires 2023, Dépenses Énergie, Dépenses R&D, Dettes sociales.
*   **Données Structurelles :** Date de création (pour l'ancienneté), Effectif, Région, Zone (ZFU).
*   **Indicateurs Calculés :** Éligibilité ACRE, CIR, Aide Énergie, etc.

<img width="1818" height="495" alt="image" src="https://github.com/user-attachments/assets/f6ae1de8-bcbd-4be2-87a4-734936b5e11e" />

## Objectif du projet
L'objectif était de répondre à une problématique métier concrète :
> **Comment transformer des données comptables brutes en opportunités de financement pour les clients, via un outil d'aide à la décision automatisé ?**

Il s'agissait d'automatiser l'identification des entreprises éligibles à **5 aides publiques majeures** (ACRE, CIR, Aide Énergie, Aide Régionale, URSSAF).

## Compétences mises en avant
Pendant ce projet, j'ai dû mettre à l'épreuve mes connaissances techniques et métiers :

*   **Génération de données :** Utilisation de la librairie `Faker` pour créer un dataset réaliste et anonymisé.
*   **Feature Engineering :** Création d'algorithmes et de conditions logiques pour traduire des règles juridiques en code Python (ex: *Si Part Energie > 3% ET Baisse CA > 30% Alors Éligible*).
*   **Nettoyage de données (Data Cleaning) :** Gestion des valeurs manquantes (imputation par médiane/moyenne) et typage des données.
*   **Visualisation :** Création de Treemaps (via `Squarify`) et Boxplots pour analyser la répartition des aides.
*   **Business Intelligence :** Conception d'un tableau de bord interactif et décisionnel sous **Power BI**.

## Carte mentale du projet
Afin de mieux m'approprier ce projet et structurer ma démarche, j'ai réalisé cette carte mentale. Elle résume le flux de travail, de la compréhension des besoins comptables à la restitution visuelle.

![Projet_Accounting](https://github.com/MazarsLoris/Projet_Accounting/blob/main/Carte%20mentale/Endrix.png)

## Conclusion du projet

Ce projet a permis de passer d'une analyse manuelle et chronophage à une solution automatisée capable de scanner un portefeuille client en quelques secondes. J'ai pu lier des compétences techniques (Python/Power BI) à une compréhension métier forte (comptabilité/fiscalité).

### Résultats clés de l’analyse (sur données fictives)
*   **Taux d'éligibilité :** Environ 40% des entreprises de l'échantillon sont éligibles à au moins une aide.
*   **Cumul des aides :** L'analyse a révélé que 18 entreprises pouvaient prétendre à plusieurs dispositifs simultanément, représentant un levier financier important.
*   **Disparités géographiques :** Les entreprises en Zones Franches Urbaines (ZFU) sont surreprésentées parmi les bénéficiaires multiples.
*   **Aides spécifiques :** L'ACRE concerne très peu d'entreprises (critères stricts de création), tandis que l'aide URSSAF (report de charges) est la plus fréquente pour les entreprises en difficulté.

### Compétences Python renforcées
*   Maîtrise des **masques booléens** pour créer les colonnes d'éligibilité (`True`/`False`).
*   Utilisation avancée de `Pandas` pour le **feature engineering** (calcul de ratios, d'ancienneté).
*   Génération de **données synthétiques** pour contourner les contraintes de confidentialité.
*   Visualisation exploratoire avec `Matplotlib` et `Squarify`.

### Utilisation de Power BI
*   Mise en place de **KPIs dynamiques** (nombre d'entreprises éligibles par aide).
*   Utilisation de la **mise en forme conditionnelle** (Rouge/Vert) pour une lecture immédiate par les comptables.
*   Création de **filtres croisés** pour explorer les données par Région ou par Secteur d'activité.

### En résumé
Ce projet illustre ma capacité à **créer de la valeur** à partir de données brutes. Il ne s'agissait pas seulement de coder, mais de fournir un outil opérationnel pour les experts-comptables, permettant in fine d'optimiser la trésorerie de leurs clients.

Je suis désormais capable de gérer un projet Data de A à Z : de la définition du besoin métier à la livraison d'un dashboard décisionnel.

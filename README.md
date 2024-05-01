# Analyse de Séries Temporelles avec ARIMA et SARIMA

## Table des matières 📝
1. [Introduction](#introduction)
2. [Mes objectifs](#mes-objectifs)
3. [Compétences acquises](#compétences-acquises)
4. [Technologies](#technologies)
5. [Description](#description)
6. [Démarche utilisée](#démarche-utilisée)
7. [Conclusion](#conclusion)
8. [Références](#références)
9. [Contactez moi](#contact)

## Introduction
Dans ce projet, j'ai exploré et appliqué des modèles ARIMA (AutoRegressive Integrated Moving Average) et SARIMA (Seasonal AutoRegressive Integrated Moving Average) pour l'analyse de séries temporelles des prix de clôture d'Amazon. Les modèles ARIMA et SARIMA sont largement utilisés dans la modélisation des séries temporelles pour faire des prévisions et capturer les tendances, les saisons et les cycles dans les données.

### Modèle ARIMA (AutoRegressive Integrated Moving Average)
Le modèle ARIMA est une combinaison de trois composants : 
- **AutoRegressive (AR)** : Cela implique la régression linéaire des valeurs actuelles sur les valeurs passées.
- **Integrated (I)** : La différenciation des observations pour rendre la série temporelle stationnaire.
- **Moving Average (MA)** : La moyenne mobile qui modélise la dépendance entre une observation et un résidu d'erreur décalé dans le temps.

Mathématiquement, le modèle ARIMA(p, d, q) est défini par :

$$ Y_t = c + \phi_1 Y_{t-1} + \phi_2 Y_{t-2} + ... + \phi_p Y_{t-p} + \theta_1 e_{t-1} + \theta_2 e_{t-2} + ... + \theta_q e_{t-q} + e_t $$

Où :
- $Y_t$ : Valeur observée à l'instant $t$
- $c$ : Constante
- $\phi$ : Coefficients AR
- $\theta$ : Coefficients MA
- $e_t$ : Erreur résiduelle à l'instant $t$

### Modèle SARIMA (Seasonal AutoRegressive Integrated Moving Average)
Le modèle SARIMA est une extension du modèle ARIMA qui prend également en compte les composantes saisonnières dans les données. Il inclut des paramètres supplémentaires pour modéliser les variations saisonnières dans la série temporelle.

Mathématiquement, le modèle $SARIMA(p, d, q)(P, D, Q)_{s}$ est défini par :

$$ Y_t = c + \phi_1 Y_{t-1} + \phi_2 Y_{t-2} + ... + \phi_p Y_{t-p} + \theta_1 e_{t-1} + \theta_2 e_{t-2} + ... + \theta_q e_{t-q} + e_t +  \phi_1 Y_{t-s} + \phi_2 Y_{t-2s} + ... + \phi_P Y_{t-Ps} + \theta_1 e_{t-s} + \theta_2 e_{t-2s} + ... + \theta_Q e_{t-Qs} + e_t $$

Où les termes AR, MA et résiduels sont appliqués à la série décalée par une période saisonnière $s$.

## Mes objectifs 🎯
Dans ce projet, mon objectif était de :
- Analyser les séries temporelles des prix de clôture d'Amazon.
- Appliquer les modèles ARIMA et SARIMA pour faire des prévisions sur les prix futurs.
- Utiliser des tests statistiques tels que le test Augmented Dickey-Fuller (ADF), le test de Ljung-Box, le test de Breusch-Pagan, et le test de Jarque-Bera pour valider les modèles.
- Comparer les performances des modèles et sélectionner le meilleur pour les prévisions.

## Compétences acquises ⚡
Dans le cadre de ce projet, j'ai développé les compétences suivantes :
- Analyse et modélisation mathématique et statistique des séries temporelles.
- Utilisation des modèles ARIMA et SARIMA pour faire des prévisions et capturer les tendances et les saisons dans les données.
- Utilisation de tests statistiques pour évaluer la stationnarité des séries, la présence d'autocorrélation et d'hétéroscédasticité.
- Utilisation de la méthode d'information d'Akaike (AIC) pour la sélection de modèle.
- Utilisation de la validation croisée pour évaluer les performances des modèles.

## Technologies 🖥️
Les technologies utilisées dans ce projet comprennent :
- Python : Utilisé pour le traitement des données, l'analyse statistique, la modélisation et la visualisation.
- Bibliothèques Python telles que pandas, numpy, statsmodels, matplotlib, pmdarima, etc.

## Description 📋
Ce projet consiste à appliquer les modèles ARIMA et SARIMA pour l'analyse de séries temporelles des prix de clôture d'Amazon. J'ai collecté les données historiques, exploré les tendances et les saisons, prétraité les données, ajusté les modèles, évalué les performances et fait des prévisions pour les prix futurs.

## Démarche utilisée

1- Extraction des Données Historiques d'AMAZON avec yfinance et pandas

2- Analyse Visuelle des Données de Prix de Clôture d'Amazon

3- Effectuer du Test ADF pour vérifier la stationnarité 

4- Trouver l'Ordre de Différenciation (d) et les Termes AR(p) et MA(q) dans le Modèle ARIMA 

5- Tests de Validation sur les Résidus pour Chaque Terme

6- Comparaison des Résultats et Choix du Meilleur Terme (0,1,0)

7- Calcul de Prévisions Hors Échantillon

8- Utilisation du SARIMA et du Auto-ARIMA



## Conclusion
Ce projet a démontré l'efficacité des modèles ARIMA et SARIMA dans l'analyse et la prévision des séries temporelles. Les compétences acquises dans ce projet peuvent être appliquées à divers domaines tels que la finance, l'économie, la météo, la santé, etc., où l'analyse des séries temporelles est essentielle pour la prise de décision.

## Contactez moi 📨

- **LinkedIn:** [Bilal Fatian](https://www.linkedin.com/in/bilal-fatian-806813254/)
- **Gmail:** [fatian.bilal@gmail.com](mailto:fatian.bilal@gmail.com)


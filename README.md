# Projet : Data Warehouse pour le Suivi des Ventes

Ce projet est une démonstration complète d'un pipeline ETL et d'une solution de Business Intelligence, réalisé avec Talend, MySQL et Power BI.

## Objectif

L'objectif était de construire un data warehouse en étoile pour analyser les revenus des ventes par produit, par vendeur, par client et dans le temps.

## Outils utilisés

* **ETL :** Talend Open Studio
* **Base de données (DWH) :** MySQL
* **Visualisation :** Power BI

## Comment l'exécuter

1.  Exécutez le script SQL pour créer la base de données `DWH_SALES` et ses tables.
2.  Ouvrez le projet Talend et configurez la connexion `CONN_DWH_SALES` à votre base MySQL.
3.  Exécutez les jobs Talend dans cet ordre :
    * Feed_Dim_product
    * Feed_Dim_Period
    * Feed_Dim_Customers
    * ALIM_DIM_VENDORS
    * Feed_Fact
4.  Ouvrez le fichier .pbix dans Power BI et actualisez les données.

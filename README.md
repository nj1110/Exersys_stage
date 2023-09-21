# Exersys_stage

<br>
<br>

**1. Objectif du stage et structure du repository :**

L'objectif du projet est de développer un système de recommandation de repas combinant les méthodes classiques de recommandation par apprentissage des préférences utilisateurs (axe 1 du projet) et l'intégration des contraintes nutritionnelles (axe2 du projet).
Les données de ce repository concernent exclusivement l'axe 1. 

Deux modèles ont été testés: 
- le modèle FiltreCollab,  basé sur une approche de type filtrage collaboratif avec apprentissage d'un espace de représentation des aliments à l'aide de Word2Vec
- le modèle RNN qui exploite le caractère séquentiel des repas, basé sur l'utilisation de réseau de neurones récurrents
  
Les préférences utilisateurs sont des préférences implicites : il s'agit des données de consommation des adultes de l'enquête INCA2.

Pour le développement et le test des modèles, les repas ont été séparés en 2 types: 

(1) les petits dejeuners (repas caractérisés par des consommations plus "répétitives") 

(2) les déjeuners et diners (repas plus complexes et caractérisés par une plus grande variété de consommations)

<br>
<br>

**2. Source des données de consommations alimentaires utilisées :**

Les données de l'enquête INCA 2 utilisées ici correspondent à 3 fichiers : 
- Table_conso.csv 
- Table_indiv.csv 
- Nomenclature_3.csv

Ces 3 tables sont disponibles à l'adresse: 
https://www.data.gouv.fr/fr/datasets/donnees-de-consommations-et-habitudes-alimentaires-de-letude-inca-2-3/

Les 2 fichiers Details_recettes.xls et Liste_ingredients.xls sont issus de ces données.
Les recettes de l'enquête INCA figurent dans le fichier Recettes_inca2_v1.

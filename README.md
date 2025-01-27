# Implémentation du Deformable Bi-level Routing Attention (DBRA) pour la Classification d'Images
## Introduction
Cette implémentation se concentre sur l'utilisation du mécanisme Deformable Bi-level Routing Attention (DBRA) dans le cadre de la classification d'images. Le DBRA est une approche novatrice qui combine :

### Attention déformable : Permet une sélection dynamique des régions pertinentes dans une image, améliorant ainsi l'efficacité et la précision.
### Approche bi-niveau : Offre un équilibre entre une attention locale détaillée et une attention globale simplifiée, capturant des informations à plusieurs échelles.
Grâce à cette méthode, les Vision Transformers (ViTs) peuvent traiter des données visuelles complexes tout en maintenant une efficacité computationnelle élevée.

## Caractéristiques principales
### Flexibilité spatiale : Le mécanisme déformable permet d’ajuster dynamiquement les points de référence pour capturer les caractéristiques importantes des objets dans une image.
### Attention hiérarchique : Une double approche qui combine une attention fine au niveau local et une vue d’ensemble au niveau global.
### Performance robuste : Amélioration notable des résultats sur des tâches de classification d'images tout en optimisant les coûts de calcul.

## Structure de l'implémentation
### Prétraitement des données : Chargement et normalisation des images pour une utilisation optimale dans le modèle.
### Architecture DBRA : Extraction des points de référence dynamiques.
Application de l'interpolation bilinéaire pour capturer les caractéristiques des zones pertinentes.
Calcul de l’attention bi-niveau pour combiner les informations locales et globales.
### Entraînement :
Utilisation d’un dataset standard pour la classification (CIFAR-10).
Optimisation via des algorithmes tels que AdamW.
### Évaluation : Calcul des métriques de performance comme l'accuracy, le F1-score, et l'AUC.
### Résultats
L’utilisation du DBRA pour la classification d’images a permis :
Une augmentation significative de l’accuracy par rapport aux ViTs standards.
Une meilleure gestion des images contenant des objets complexes ou des arrière-plans encombrés.
Une réduction des calculs inutiles grâce à la flexibilité déformable.
Prérequis
Framework : TensorFlow 
Environnement : GPU (NVIDIA CUDA 11.0 ou plus recommandé).
## Dépendances :
Python 3.8 ou plus.
tensorflow 
numpy, matplotlib, et autres bibliothèques pour le traitement des données.

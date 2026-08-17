# IA-CNN-Ship-Detection-BMZ
Engineering school project ; CNN built from scratch ; Classify ships pictures from any Data Base

Description du Projet
Ce notebook a pour objectif de réaliser un projet d'apprentissage automatique de bout en bout, en se concentrant sur un problème de classification d'images. Nous utiliserons le dataset 'Ships Dataset' de Kaggle et développerons un Réseau de Neurones Convolutionnel (CNN) 'from scratch' pour classer les navires.

Détails du Dataset et de la Tâche
Source du Dataset : Kaggle ('Ships Dataset' - vinayakshanawad)
Type de Données : Images (navires)
Tâche : Classification de navires en catégories telles que 'navire militaire', 'navire commercial', 'navire de pêche', etc. Ces classifications serviront à déterminer le statut pour un passage (e.g., 'menace', 'ok pour passage', 'à contrôler').
Nombre de Samples : Sera déterminé après le chargement et le prétraitement du dataset.
Formatage des Données : Nécessitera un redimensionnement et une normalisation des images.
Architecture du Réseau de Neurones : Réseau de Neurones Convolutionnel (CNN), conçu et entraîné 'from scratch'.
Objectifs
Réaliser un apprentissage 'from scratch' d'un CNN pour la classification d'images.
Présenter les statistiques clés : nombre total de paramètres du modèle, accuracy pour les ensembles d'entraînement et de test.
Visualiser les courbes de loss et d'accuracy pour l'entraînement et le test.
Assurer la reproductibilité de l'ensemble du notebook.
Bilan du Projet
Points positifs
Le modèle se compile et s'exécute sans erreur.
La classification par classe fonctionne correctement, avec un mappage cohérent vers les catégories de danger (Menace, À contrôler, Ok pour passage).
Il est possible de tester le modèle sur des images importées manuellement (en dehors du jeu de test), ce qui le rend utilisable dans un contexte réel.
Points négatifs
La confiance des prédictions est nettement améliorée, proche de 1, mais la classification est quand même fausse parfois.
Axes d'amélioration
Explorer les pistes suivantes pourrait permettre d'améliorer significativement la confiance et la précision du modèle :

Transfer learning : utiliser un modèle pré-entraîné (ResNet, EfficientNet, etc.) plutôt qu'un CNN from scratch, pour bénéficier d'une meilleure base de départ.
Plus de données et d'epochs : un dataset plus large et davantage d'epochs d'entraînement auraient réduit l'incertitude des prédictions.
Architecture plus profonde : ajouter des couches, affiner le dropout et intégrer de la batch normalization pour mieux généraliser.
GPU plus puissant : les limitations de Google Colab (mémoire, temps de session) ont contraint nos expérimentations.

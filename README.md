# 🚢 IA-CNN-Ship-Detection-BMZ

> **Engineering school project** | CNN built from scratch | Classify ships pictures from any Database

---

## 📝 Description du Projet
Ce notebook a pour objectif de réaliser un projet d'apprentissage automatique de bout en bout, en se concentrant sur un problème de **classification d'images**. 

Nous développons un **Réseau de Neurones Convolutionnel (CNN) *from scratch*** pour classer des navires et leur attribuer un statut de sécurité automatisé.

---

## 📊 Détails du Dataset & Tâche

* **Source du Dataset :** [Kaggle - Ships Dataset (vinayakshanawad)](https://kaggle.com) *(Pensez à ajouter le lien exact de votre dataset ici !)*
* **Type de Données :** Images de navires.
* **Formatage des Données :** Redimensionnement et normalisation des images.
* **Architecture :** CNN conçu, configuré et entraîné de A à Z.

### 🎯 La Tâche de Classification
Le modèle catégorise les navires (ex: *militaire, commercial, pêche*) afin de déterminer automatiquement leur **statut de passage** :
* 🔴 **Menace**
* 🟡 **À contrôler**
* 🟢 **Ok pour passage**

---

## 🚀 Objectifs du Notebook

- [x] Réaliser un apprentissage *from scratch* d'un CNN pour la classification d'images.
- [x] Présenter les statistiques clés (nombre de paramètres, accuracy train/test).
- [x] Visualiser les courbes de `loss` et d' `accuracy` (entraînement et test).
- [x] Assurer la reproductibilité totale de l'ensemble du notebook.

---

## 📈 Bilan du Projet

### 👍 Points positifs
* **Stabilité :** Le modèle se compile et s'exécute sans aucune erreur.
* **Logique métier :** La classification par classe fonctionne correctement, avec un mappage cohérent vers les catégories de danger.
* **Prêt pour le test :** Il est possible de tester le modèle sur des images importées manuellement (hors jeu de test) pour une utilisation en contexte réel.

### 👎 Points négatifs
* **Fiabilité :** La confiance des prédictions est nettement améliorée (proche de 1), mais la classification finale reste parfois fausse.

---

## 🛠️ Axes d'Amélioration

Pour dépasser les limites actuelles du modèle, plusieurs pistes sont envisagées :

1. **Transfer Learning :** Utiliser un modèle pré-entraîné (`ResNet`, `EfficientNet`, etc.) plutôt qu'un CNN *from scratch* pour bénéficier d'une meilleure base de départ.
2. **Data & Epochs :** Augmenter la taille du dataset et le nombre d'époques d'entraînement pour réduire l'incertitude des prédictions.
3. **Optimisation de l'Architecture :** Rendre le réseau plus profond (ajouter des couches, affiner le *dropout* et intégrer de la *batch normalization*) pour une meilleure généralisation.
4. **Ressources :** Utiliser un GPU plus puissant (les limitations de mémoire et de temps de session de Google Colab gratuit ont contraint nos expérimentations).

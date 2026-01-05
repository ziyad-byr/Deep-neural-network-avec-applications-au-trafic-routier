# Simulation et Optimisation du Trafic Routier (Deep Neural Network approach)

Ce projet propose une modélisation mathématique et une simulation du flux de trafic routier. Il utilise des méthodes de résolution numérique "fait maison" pour optimiser les paramètres de déplacement des véhicules afin de minimiser les erreurs de trajectoire ou de flux.

## 🎯 Objectif du projet
L'objectif est de simuler le comportement de $N$ voitures sur une portion de route en fonction de conditions initiales aléatoires (loi normale). Le projet implémente un solveur numérique pour traiter les équations différentielles régissant le mouvement et utilise une boucle d'optimisation pour ajuster les poids du modèle (inspiré des réseaux de neurones) afin de réduire l'erreur globale.

## 🛠️ Stack Technique
* **Langage :** Python 3
* **Librairies de calcul :** `NumPy` pour la manipulation de matrices et le calcul numérique.
* **Visualisation :** `Matplotlib` pour le rendu des courbes d'erreur et des simulations.
* **Algorithmes :** Implémentation d'un solveur ODE (Équations Différentielles Ordinaires) personnalisé et d'un algorithme de correction itératif.

## 🚀 Fonctionnalités clés
* **Génération stochastique :** Initialisation des positions et vitesses des véhicules via une distribution normale.
* **Solveur sur mesure :** Utilisation de la fonction `solveur_fait_maison` pour prédire l'état futur du trafic.
* **Optimisation itérative :** Calcul de la norme d'erreur et ajustement des paramètres sur 150 itérations pour converger vers une solution optimale.
* **Analyse de scalabilité :** Test du modèle sur différentes tailles de flottes (de 3 à 100 voitures).

## 📊 Résultats
Le script génère des graphiques montrant la convergence de l'erreur en fonction du nombre d'itérations. Plus la flotte est importante, plus la complexité de l'optimisation augmente, permettant d'étudier les limites du modèle.

## 💻 Installation et Utilisation
1. Cloner le dépôt :
```bash
git clone [https://github.com/TON_PSEUDO/mon-projet-data-ia.git](https://github.com/TON_PSEUDO/mon-projet-data-ia.git)
```
2. Installer les dépendances :
pip install numpy matplotlib
3. Lancer le notebook : Ouvrez le fichier .ipynb dans Jupyter ou VS Code et exécutez toutes les cellules.

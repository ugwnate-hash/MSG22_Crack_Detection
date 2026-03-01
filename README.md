# Détection de Fissures dans la Maçonnerie par Deep Learning

Ce projet implémente des algorithmes d'apprentissage supervisé (Réseaux de Neurones et CNN) pour la détection automatisée de fissures sur des images de maçonnerie. Il s'inscrit dans le cadre du projet **MSG22_ML_2025** et s'appuie sur des architectures pré-entraînées issues de la recherche.

## Auteurs
* Arthur Calvi
* Raphaël Leclercq
* Clément Desodt
* Xavier Jourdain

## Objectifs du projet
1. **Classification binaire** : Distinguer les images de maçonnerie saines (Classe 0) des images présentant des fissures (Classe 1).
2. **Comparaison d'architectures** : Évaluer les performances d'un Perceptron Multicouche (MLP) par rapport à des Réseaux de Neurones Convolutifs (ConvNet).
3. **Transfer Learning** : Charger, évaluer et affiner (fine-tuning) des modèles de recherche pré-entraînés (**Architecture A** et **Architecture B**).
4. **Optimisation des hyperparamètres** : Implémentation d'un GridSearch pour trouver la meilleure combinaison d'apprentissage.

## Arborescence du projet

Pour que le notebook fonctionne correctement en local, votre dossier doit être structuré de la manière suivante :

```text
📂 MSG22_Crack_Detection/
├── 📄 SupervisedLearning_CrackDetection_Part4.ipynb  # Le notebook principal
├── 📄 requirements.txt                                       # Dépendances Python
├── 📄 README.md                                              # Documentation
├── 📄 CNN_architecture_A_batch_size_20_epochs_200            # Poids pré-entraînés (Modèle A)
├── 📄 CNN_architecture_B_batch_size_20_epochs_200            # Poids pré-entraînés (Modèle B)
└── 📂 Images/                                                # Dataset des images
    ├── 📂 0/                                                 # Images SANS fissure
    └── 📂 1/                                                 # Images AVEC fissure
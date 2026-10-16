# Reconnaissance de panneaux de signalisation (GTSRB)

Projet de Deep Learning — Master 1, Fondamentaux du Deep Learning (2026-2027).
Auteur : Pariston Kamis.

Classification des 43 classes de panneaux du dataset **GTSRB** avec Keras / TensorFlow : réseau dense de référence, CNN, expériences d'amélioration (Dropout, Data Augmentation, BatchNorm, Early Stopping) et analyse des erreurs.

| Modèle | Accuracy validation | Accuracy test |
|---|---|---|
| Réseau dense (référence) | 78,8 % | — |
| CNN de base | 93,7 % | — |
| CNN final (BatchNorm + Dropout + Early Stopping) | 99,0 % | **97,7 %** |

## Contenu

- `projet_panneaux_gtsrb.ipynb` : notebook complet, exécuté, avec toutes les explications.
- `traffic_sign_cnn.keras` : modèle final entraîné, pour la démonstration sans ré-entraînement.

## Exécution

Ouvrir le notebook dans Google Colab (GPU recommandé) puis *Exécution → Tout exécuter*. Le dataset GTSRB est téléchargé automatiquement via `torchvision`.

Dépendances : `tensorflow`, `torchvision`, `scikit-learn`, `pandas`, `matplotlib`, `pillow`.

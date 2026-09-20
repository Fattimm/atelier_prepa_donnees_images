# Atelier Préparation de Données Images

Nettoyage et préparation d'un dataset d'images de déchets (cardboard, glass,
metal, paper, plastic, trash) en vue de l'entraînement d'un modèle de
classification.

## Structure du projet

atelier_prepa_donnees_images/
├── notebooks/
│ └── atelier_prepa_donnees_images.ipynb
├── reports/
│ └── audit_images.csv
└── data/
├── raw/ # dataset original, en lecture seule
│ ├── cardboard/
│ ├── glass/
│ ├── metal/
│ ├── paper/
│ ├── plastic/
│ └── trash/
└── cleaned/ # généré lors du nettoyage


## Installation

```bash
python -m venv venv
source venv/bin/activate   # Windows : venv\Scripts\activate
pip install pillow numpy pandas
```

## Utilisation

1. Placer les images dans `data/raw/<classe>/`
2. Lancer Jupyter et ouvrir `notebooks/atelier_prepa_donnees_images.ipynb`
3. Exécuter les cellules dans l'ordre

## Sortie

`reports/audit_images.csv` contient les résultats de l'audit du dataset
(images corrompues, doublons, classes déséquilibrées, etc.).
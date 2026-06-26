# Cardinal Buoy Detection

Détection et classification de **bouées cardinales** (Nord / Sud / Est / Ouest) dans des
images maritimes, réalisée dans le cadre du module Image (FISE — Télécom Saint-Étienne).

Le projet compare trois familles d'approches sur le même problème :

| Dossier      | Approche                          | Notebooks |
|--------------|-----------------------------------|-----------|
| `classical/` | Traitement d'image classique (segmentation couleur, morphologie) | `Classical_method_V1.ipynb`, `Classical_method_V2.ipynb` |
| `ML/`        | Machine learning « shallow »      | `ML_distance_based_classification.ipynb`, `ML_kmeans_classification.ipynb`, `ML_mask_knn_FINAL.ipynb` |
| `DP/`        | Deep learning                     | `DP_cnn_classification.ipynb`, `YOLO_Finetuning.ipynb` |

## Contenu

- `setup.ipynb` — préparation de l'environnement et des données.
- `test_images_analysis.ipynb` — analyse exploratoire des images de test.
- `demo_soutenance.ipynb` — démonstration de soutenance.
- `project_report.pdf` — rapport complet du projet.
- `Soutenance_Bouees_Cardinales.pptx` — support de présentation.

## Méthodes

1. **Classique** — segmentation par couleur (espaces HSV/Lab), opérations morphologiques
   et extraction de la signature des marques (cônes) pour déduire le type de cardinale.
2. **ML** — classification par distance, k-means et k-NN sur masques/descripteurs.
3. **Deep Learning** — un CNN de classification et un YOLO fine-tuné pour la détection.

## Utilisation

Les notebooks sont indépendants ; ouvrir celui de la méthode souhaitée (Jupyter / Colab).
Commencer par `setup.ipynb` pour mettre en place l'environnement.

## Auteurs

Projet Image FISE — Posseme (Télécom Saint-Étienne).

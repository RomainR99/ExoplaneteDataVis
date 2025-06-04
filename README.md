# 🌌 Exoplanet Clustering & Visualization Project

Ce projet a pour objectif d'explorer, visualiser et regrouper des exoplanètes à l’aide d’algorithmes d’apprentissage non supervisé, notamment **KMeans**, et de réaliser une analyse descriptive basée sur leurs caractéristiques physiques.

---

## 📊 Objectifs

- Nettoyer et préparer les données d’exoplanètes (issues de la NASA Exoplanet Archive ou autre base).
- Visualiser les distributions de variables comme la masse, le rayon ou la distance orbitale.
- Appliquer l'algorithme de **KMeans** pour découvrir des groupes naturels d'exoplanètes.
- Évaluer les clusters avec le **Silhouette score**.
- Interpréter les groupes en fonction des caractéristiques astrophysiques.

---

## 🧪 Données utilisées

Les colonnes principales utilisées dans l’analyse sont :

- `pl_bmasse` : Masse de la planète (en masses terrestres)
- `pl_rade` : Rayon de la planète (en rayons terrestres)
- `pl_orbsmax` : Demi-grand axe de l’orbite (en UA)
- `st_teff` : Température effective de l’étoile hôte (en K)
- `discoverymethod` : Méthode de détection (utilisée pour comparaison)
- `habitable` : Indication d’habitabilité (si disponible)

---

## 🛠️ Librairies utilisées

- `pandas`, `numpy` : manipulation de données
- `matplotlib`, `seaborn` : visualisation
- `sklearn` :
  - `StandardScaler`, `PCA` pour la préparation et la réduction de dimension
  - `KMeans` pour le clustering
  - `silhouette_score` pour évaluer la cohérence des clusters

---

## 🌀 Méthodologie

1. **Nettoyage des données** :
   - Suppression des doublons et lignes incomplètes
   - Sélection des colonnes pertinentes

2. **Standardisation** :
   - Normalisation des données numériques pour appliquer KMeans efficacement.

3. **Détermination du nombre de clusters** :
   - Méthode du coude (Elbow method)
   - Validation par **Silhouette score**

4. **Visualisation des clusters** :
   - Réduction en 2D via PCA
   - Coloration selon les labels des clusters

---

## 📈 Résultats

- Nombre optimal de clusters : **3**
- **Silhouette Score** obtenu : **0.44**
- Interprétation des clusters :
  - **Cluster 0** : Petites planètes proches de leur étoile
  - **Cluster 1** : Géantes gazeuses à distance modérée
  - **Cluster 2** : Objets massifs et très éloignés, souvent autour d’étoiles froides

## Groupe
    - Brendan
    - Soufiane
    - Mustapha
    - Romain





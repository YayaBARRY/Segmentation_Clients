# Segmentation des Clients d'Expresso Sénégal avec PySpark et MLlib

## Objectif du projet

Ce projet vise à segmenter les clients de l’opérateur téléphonique Expresso Sénégal à partir de données de consommation (voix, data, recharges, régularité, fidélité, churn...) à l’aide de **PySpark** (traitement distribué) et de **Power BI** (visualisation), dans le but d’identifier des profils clients distincts et d'orienter des actions commerciales ciblées.

## Technologies utilisées

- Python 3.10
- PySpark (Spark MLlib)
- Power BI Desktop
- Pandas
- FPDF (pour les exports PDF)
  

## Structure du projet

1. Données source clients Expresso
2. Résumé des valeurs manquantes
3. Données enrichies avec clusters
4. Rapport d'interprétation PDF
5. rapport_segmentation_cients_expresso.pdf
   

## Pipeline de traitement

1. **Chargement et nettoyage**
2. **Encodage & vectorisation**
3. **Réduction de dimension (PCA)**
4. **Clustering (KMeans)**
5. **Analyse & interprétation**
6. **Export (CSV / PDF / DOCX)**
   

## Résumé des profils détectés

| Cluster | Profil | Recommandation |
|--------:|--------|----------------|
| 0 | Data-only silencieux | Packs Data low-cost |
| 1 | Premium fidèles | Programme VIP |
| 2 | Clients standards | Fidélisation + upsell |
| 3 | Utilisateurs voix actifs | Packs voix personnalisés |
| 4 | Clients volatils | Réactivation ou abandon |


## Prochaine étape

Visualisation avancée des segments sur Power BI :
- Répartition géographique (REGION)
- Churn par cluster
- Analyse multidimensionnelle croisée

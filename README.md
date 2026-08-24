# Retail Sales Analysis

Ce dépôt contient un notebook Jupyter d'analyse des ventes (retail) et les fichiers associés.

**Objectif business :**

Améliorer la performance commerciale en identifiant les produits, régions et segments les plus rentables, détecter les sources de pertes (commandes déficitaires), comprendre la saisonnalité des ventes et proposer des actions (optimisation des remises, priorisation des catégories et ciblage clients) pour augmenter le chiffre d'affaires et la marge.

**Dataset & méthode :**

- Source : jeu de données "Sample - Superstore" (extrait local dans Downloads).
- Traitement : nettoyage, enrichissement (année/mois/cohorte, marge, délai de livraison), export CSV, chargement SQLite pour analyses SQL.
- Analyses : EDA (pandas, matplotlib, seaborn), requêtes agrégées SQL, visualisations, analyse de cohortes.

**Technologies utilisées :**

- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn
- statsmodels
- SQLite / SQL
- Git / GitHub

**Résumé des graphiques et interprétation (extraits du notebook) :**

- Distribution des Sales / Profit : histogrammes montrant la concentration du chiffre d'affaires et la dispersion du profit ; attention aux extrêmes (outliers) qui influencent la médiane et la variance.

- Matrice de corrélation : met en évidence les relations entre Sales, Quantity, Discount, Profit, Profit Margin et Shipping Days. Par exemple, une corrélation négative entre Discount et Profit suggère que des remises élevées réduisent la rentabilité.

- Boxplot - Profit par Catégorie : compare la distribution du profit entre catégories (Furniture, Office Supplies, Technology). Permet d'identifier les catégories avec forte variabilité ou présence fréquente de pertes.

- Boxplot - Impact de la remise sur le Profit : montre comment les niveaux de remise affectent le profit ; utile pour définir seuils de remise acceptables.

- Heatmap Profit (Région × Catégorie) : identifie les régions où chaque catégorie performe le mieux en terme de profit — utile pour prioriser le mix produit par région.

- Heatmap saisonnalité (Année × Mois) : visualise les pics saisonniers de chiffre d'affaires par mois et par année, pour préparer stocks et campagnes marketing.

- Barres Cohorte (Nombre de clients / Profit par cohorte) : analyse l'apport des clients par année d'acquisition — détecte cohortes plus rentables ou à faible rétention.

- Insights rapides (chiffres clefs) : CA total, profit total, marge moyenne, % de commandes déficitaires, remise moyenne, meilleure région & catégorie en profit — résumé opérationnel immédiat.

Pour des explications détaillées des graphiques et des chiffres, voir le notebook : [Retail-Sales-Analysis/Anlayse_Sales.ipynb](Retail-Sales-Analysis/Anlayse_Sales.ipynb)

---

Si vous le souhaitez, je peux :

- Générer un requirements.txt précis à partir des imports du notebook.
- Ajouter des recommandations opérationnelles détaillées basées sur les résultats (ex : limiter remises pour telle catégorie, focus sur telle région).

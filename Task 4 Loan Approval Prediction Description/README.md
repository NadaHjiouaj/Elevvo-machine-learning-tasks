# Projet de Prédiction d'Approbation de Prêt

## 📌 Description du Projet

Ce projet vise à développer un modèle de machine learning capable de prédire si une demande de prêt bancaire sera approuvée ou refusée en fonction de diverses caractéristiques du demandeur (revenu, score de crédit, actifs, etc.). Le notebook Jupyter fourni contient l'ensemble du processus, de l'exploration des données à l'évaluation des modèles.

---

## 📊 Structure du Projet

Le notebook est organisé en plusieurs sections :

1. **Installation et Import des Bibliothèques**
2. **Chargement et Exploration des Données**
3. **Nettoyage et Prétraitement des Données**
4. **Analyse Exploratoire des Données (EDA)**
5. **Préparation des Données pour l'Apprentissage**
6. **Entraînement et Évaluation des Modèles**
7. **Optimisation des Hyperparamètres**
8. **Gestion du Déséquilibre des Classes (SMOTE / UnderSampling)**
9. **Évaluation Finale et Métriques**

---

## 🛠️ Technologies Utilisées

- **Python 3**
- **Pandas / NumPy** : Manipulation des données
- **Matplotlib / Seaborn** : Visualisation
- **Scikit-learn** : Modèles de ML, prétraitement, évaluation
- **Imbalanced-learn** : Gestion du déséquilibre des classes
- **Google Colab** : Environnement d'exécution

---

## 📁 Jeu de Données

Le jeu de données (`loan_approval_dataset.csv`) contient 4269 entrées et 13 caractéristiques, notamment :

- `loan_id` : Identifiant du prêt
- `no_of_dependents` : Nombre de personnes à charge
- `education` : Niveau d'éducation
- `self_employed` : Indépendant ou non
- `income_annum` : Revenu annuel
- `loan_amount` : Montant du prêt
- `loan_term` : Durée du prêt
- `cibil_score` : Score de crédit
- `residential_assets_value` : Valeur des actifs résidentiels
- `commercial_assets_value` : Valeur des actifs commerciaux
- `luxury_assets_value` : Valeur des actifs de luxe
- `bank_asset_value` : Valeur des actifs bancaires
- `loan_status` : Statut du prêt (Approved / Rejected)

---

## 🔍 Résultats Clés

- **Distribution des classes** : 2656 prêts approuvés, 1613 refusés (ratio de déséquilibre ~0.61)
- **Modèles testés** : Régression Logistique, Arbre de Décision, Forêt Aléatoire
- **Techniques d'équilibrage** : SMOTE et RandomUnderSampler
- **Métriques d'évaluation** : Accuracy, Precision, Recall, F1-score, AUC-ROC

---

## 🚀 Comment Exécuter le Projet

1. Téléchargez le notebook et le jeu de données.
2. Ouvrez le notebook dans Google Colab ou Jupyter.
3. Exécutez les cellules dans l'ordre.
4. Assurez-vous d'importer le fichier `loan_approval_dataset.csv` lorsque Colab le demande.

---

## 📈 Améliorations Possibles

- Essayer d'autres modèles (XGBoost, LightGBM, etc.)
- Optimiser davantage les hyperparamètres
- Feature engineering supplémentaire
- Validation croisée plus poussée


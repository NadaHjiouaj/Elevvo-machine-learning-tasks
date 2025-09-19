<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Score Prediction</title>
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: #f8f9fa;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 2rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        
        h1, h2, h3 {
            color: var(--primary);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .badge {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 0.3rem 0.6rem;
            border-radius: 4px;
            font-size: 0.8rem;
            margin-right: 0.5rem;
            margin-bottom: 0.5rem;
        }
        
        section {
            background: white;
            padding: 1.5rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin: 1.5rem 0;
        }
        
        .card {
            background: var(--light);
            padding: 1.2rem;
            border-radius: 8px;
            border-left: 4px solid var(--secondary);
        }
        
        .highlight {
            background-color: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid #e9ecef;
            margin: 1.5rem 0;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            margin: 1rem 0;
        }
        
        .tech-item {
            background: #e9ecef;
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }
        
        .env-badge {
            background-color: #f1f8ff;
            color: #0366d6;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            display: inline-flex;
            align-items: center;
            margin: 0.5rem 0;
            border: 1px solid #d1e5fa;
        }
        
        .env-badge img {
            width: 20px;
            margin-right: 8px;
        }
        
        footer {
            text-align: center;
            margin-top: 3rem;
            padding: 1.5rem;
            color: #6c757d;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>📊 Student Score Prediction</h1>
        <p class="subtitle">Analyse prédictive des performances académiques grâce au Machine Learning</p>
    </header>

    <section>
        <h2>📖 Aperçu du Projet</h2>
        <p>Ce projet se concentre sur la prédiction des résultats d'examens étudiants en utilisant des techniques d'apprentissage automatique. L'analyse comprend l'exploration de données, la visualisation et la modélisation prédictive à partir d'un jeu de données contenant diverses caractéristiques liées à la performance étudiante.</p>
        
        <div class="env-badge">
            <span>Environnement de développement: <strong>Google Colab</strong></span>
        </div>
        
        <div class="highlight">
            <p>L'utilisation de Google Colab a permis un environnement de calcul haute performance avec accès à des ressources GPU, facilitant l'expérimentation et l'itération rapide des modèles sans contraintes matérielles.</p>
        </div>
    </section>

    <section>
        <h2>🎯 Objectifs</h2>
        <p>Développer un modèle prédictif capable d'estimer les scores d'examens étudiants en fonction de divers facteurs académiques et socio-économiques, avec pour applications potentielles :</p>
        
        <div class="grid">
            <div class="card">
                <h3>Identification des facteurs clés</h3>
                <p>Déterminer les variables ayant le plus d'impact sur la performance académique</p>
            </div>
            <div class="card">
                <h3>Intervention préventive</h3>
                <p>Anticiper les difficultés des étudiants pour mettre en place un accompagnement ciblé</p>
            </div>
            <div class="card">
                <h3>Optimisation des ressources</h3>
                <p>Allouer plus efficacement les ressources éducatives en fonction des besoins prédits</p>
            </div>
        </div>
    </section>

    <section>
        <h2>📊 Jeu de Données</h2>
        <p>Le jeu de données <code>student_performance.csv</code> contient <strong>6607 observations et 20 variables</strong>, incluant à la fois des caractéristiques numériques et catégorielles :</p>
        
        <div class="grid">
            <div class="card">
                <h3>Variables principales</h3>
                <ul>
                    <li>Heures d'étude</li>
                    <li>Assiduité</li>
                    <li>Heures de sommeil</li>
                    <li>Résultats antérieurs</li>
                    <li>Implication parentale</li>
                </ul>
            </div>
            <div class="card">
                <h3>Variables supplémentaires</h3>
                <ul>
                    <li>Niveau de motivation</li>
                    <li>Accès à Internet</li>
                    <li>Environnement d'étude</li>
                    <li>Ressources supplémentaires</li>
                </ul>
            </div>
            <div class="card">
                <h3>Variable cible</h3>
                <ul>
                    <li><strong>Exam_Score</strong> - Score à l'examen (variable à prédire)</li>
                </ul>
            </div>
        </div>
    </section>

    <section>
        <h2>🛠️ Méthodologie & Technologies</h2>
        
        <h3>Stack technique</h3>
        <div class="tech-stack">
            <span class="tech-item">Python</span>
            <span class="tech-item">Pandas</span>
            <span class="tech-item">NumPy</span>
            <span class="tech-item">Matplotlib</span>
            <span class="tech-item">Seaborn</span>
            <span class="tech-item">Scikit-learn</span>
            <span class="tech-item">Google Colab</span>
        </div>
        
        <h3>Processus d'analyse</h3>
        <ol>
            <li><strong>Chargement et exploration des données</strong> - Analyse préliminaire et statistiques descriptives</li>
            <li><strong>Nettoyage et prétraitement</strong> - Gestion des valeurs manquantes et transformation des variables</li>
            <li><strong>Analyse exploratoire (EDA)</strong> - Visualisations et identification des patterns</li>
            <li><strong>Ingénierie des caractéristiques</strong> - Création de nouvelles variables pertinentes</li>
            <li><strong>Modélisation</strong> - Entraînement et optimisation d'algorithmes de régression</li>
            <li><strong>Évaluation et validation</strong> - Mesure des performances et analyse des résultats</li>
        </ol>
    </section>

    <section>
        <h2>📈 Modèles et Résultats</h2>
        
        <h3>Algorithmes utilisés</h3>
        <div class="grid">
            <div class="card">
                <h4>Régression Linéaire</h4>
                <p>Modèle de base pour établir une référence de performance</p>
            </div>
            <div class="card">
                <h4>Régression Polynomiale</h4>
                <p>Extension pour capturer les relations non-linéaires</p>
            </div>
            <div class="card">
                <h4>Autres modèles</h4>
                <p>Forêts aléatoires, Gradient Boosting selon les besoins</p>
            </div>
        </div>
        
        <h3>Métriques d'évaluation</h3>
        <p>Les performances des modèles ont été évaluées à l'aide de plusieurs métriques standard :</p>
        <ul>
            <li><strong>MAE (Mean Absolute Error)</strong> - Erreur absolue moyenne</li>
            <li><strong>MSE (Mean Squared Error)</strong> - Erreur quadratique moyenne</li>
            <li><strong>R² Score</strong> - Coefficient de détermination</li>
        </ul>
        
        <div class="highlight">
            <p>Le modèle optimal a atteint un score R² de 0.89, démontrant une capacité prédictive élevée pour estimer les scores d'examens à partir des variables disponibles.</p>
        </div>
    </section>

    <section>
        <h2>🚀 Exécution du Projet</h2>
        <p>Le projet a été développé dans un notebook Jupyter exécuté sur Google Colab, permettant :</p>
        
        <div class="grid">
            <div class="card">
                <h3>Reproductibilité</h3>
                <p>Code et résultats entièrement reproductibles</p>
            </div>
            <div class="card">
                <h3>Collaboration</h3>
                <p>Partage aisé avec la communauté</p>
            </div>
            <div class="card">
                <h3>Performance</h3>
                <p>Accès à des ressources de calcul sans configuration complexe</p>
            </div>
        </div>
        
        <h3>Instructions d'exécution</h3>
        <ol>
            <li>Accéder au notebook sur Google Colab</li>
            <li>Télécharger le jeu de données lorsque demandé</li>
            <li>Exécuter les cellules séquentiellement</li>
            <li>Optionnellement : modifier les paramètres ou expérimenter avec différents modèles</li>
        </ol>
    </section>

    <section>
        <h2>📋 Conclusions et Perspectives</h2>
        
        <h3>Principales conclusions</h3>
        <ul>
            <li>Les résultats antérieurs et les heures d'étude sont les prédicteurs les plus importants</li>
            <li>L'implication parentale et le sommeil ont un impact significatif sur la performance</li>
            <li>Le modèle démontre une précision satisfaisante pour la prédiction des scores</li>
        </ul>
        
        <h3>Limitations et améliorations futures</h3>
        <ul>
            <li>Extension à des données multi-sources (plus d'établissements)</li>
            <li>Intégration de techniques avancées comme le deep learning</li>
            <li>Développement d'une interface de prédiction interactive</li>
            <li>Validation sur des données en temps réel</li>
        </ul>
    </section>

    <footer>
        <p>Projet académique d'analyse prédictive - Développé avec Google Colab</p>
        <p>© 2023 - Portfolio Data Science</p>
    </footer>
</body>
</html>

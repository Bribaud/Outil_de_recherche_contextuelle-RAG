# Outil de recherche contextuelle (Retrieval Augmented Generation) 💻📚

**IA Recherche Contextuelle** est une application web interactive développée avec Streamlit qui implémente un système de Retrieval Augmented Generation (RAG). L'outil permet aux utilisateurs d'analyser automatiquement le contenu de plusieurs articles web en entrant simplement leurs URLs. Grâce à une architecture sophistiquée combinant le découpage intelligent de texte, la génération d'embeddings sémantiques via le modèle `all-MiniLM-L6-v2` de Hugging Face, et l'indexation vectorielle FAISS pour des recherches ultra-rapides, l'application offre une expérience fluide pour interroger les documents en langage naturel. Propulsée par Claude 3 Opus d'Anthropic, elle génère des réponses précises et contextuelles accompagnées de leurs sources, transformant ainsi la façon dont on accède à l'information en ligne en quelques secondes seulement.

![Logo du projet](img.png)

## Fonctionnalités de l'application

- Extraction automatique du contenu des articles à partir des URL fournies.
- Division intelligente du texte en segments pour un traitement plus efficace.
- Génération d’embeddings via Hugging Face (`all-MiniLM-L6-v2`) pour une meilleure compréhension sémantique.
- Indexation et stockage des embeddings dans FAISS pour une recherche rapide.
- Possibilité de poser des questions en langage naturel sur les articles traités.
- Affichage des résultats avec les sources d'information correspondantes.

## Installation

1. Clonez ce dépôt sur votre machine locale en exécutant :

   ```bash
   git clone https://github.com/votre-repo.git
   ```

2. Accédez au répertoire du projet :

   ```bash
   cd votre-repo
   ```

3. Installez les dépendances requises avec `pip` :

   ```bash
   pip install -r requirements.txt
   ```

4. Configurez votre clé API en créant un fichier `.env` à la racine du projet et en ajoutant votre clé API :

   ```env
   ANTHROPIC_API_KEY=your_api_key_here
   ```

## Usage

1. Exécutez l'application Streamlit avec la commande suivante :

   ```bash
   streamlit run main.py
   ```


2. L'application web s'ouvrira automatiquement dans votre navigateur.


3. Dans les premières barres, vous pourrez entrer les URL des articles à analyser.


4. Lancez le traitement des articles en cliquant sur **"Lancer la recherche"**.


5. L'application effectuera le chargement des articles, la segmentation du texte, la génération d’embeddings et l’indexation dans FAISS.


6. Une fois le traitement terminé, posez une question et obtenez une réponse basée sur le contenu des articles.

## Structure du projet

1. main.py : Le script principal de l'application Streamlit.


2. requirements.txt : Une liste des paquets Python requis pour le projet.


3. .env : Fichier de configuration pour stocker votre clé API.

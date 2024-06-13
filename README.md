# IA générative en action: Intégrez les LLM dans vos applications

Ce repo contient les quelques notebooks Jupyter de démo associés au meetup dont une replay est disponible sur le [site de younup](https://lnkd.in/enf-y6Jg)

Le fichier `.env.example` à la racine contient les quelques variables nécessaires (clé OpenAI, url Redis ou Neo4J, etc.). Faire une copie de ce fichier, le renommer `.env` et renseigner ses propres variables.

Le fichier `docker-compose` à la racine contient une instance Redis ainsi qu'une instance Neo4J nécessaires à certaines démo.

### 01-Simple QA chat with memory

Implémentation d'un simple Chat bot avec mémoire
La mémoire utilisée est pour l'exemple est un simple tableau en mémoire.

### 02-Retrival Augmented Generation

Implémentation d'un système RAG.

La vector store utilisé est Redis (disponible dans le `docker-compose` à la racine du repo).

La mémoire est-elle aussi persistée dans l'instance Redis

### 03-RAG youtube.ipynb

Implémentation d'un système RAG similaire au précédent mais dont la source de donnée est une liste de vidéo Youtube.

### 04-Agent with tools

Implémentation d'un agent simple disposant d'un Tool de type "Recherche Internet".

La recherche utilise le service [Tavily Search](https://docs.tavily.com/) disposant d'un free tier.

### 05-RAG knowledge graph

Implémentation d'un système RAG augmenté par une graphe de connaissance.

La partie Vector Store/Knowledge graph est gérée via Neo4j (disponible dans le `docker-compose` à la racine du repo).

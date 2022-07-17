# TweetEvalEmotion

## Présentation

Le modèle BERT (Bidirectional Encoder Representations from Transformers) est l’un des premiers modèles transformeur (transformer). BERT est un modèle auto-attentif, ce qui lui permet de développer une compréhension statistique du langage avec lequel il a été entrainé sans requérir d’étiquetage des données (data labelling).

Nous avons spécialisé un modèle de pointe (state-of-the-art), variante de BERT : le modèle DeBERTaV3 (base) dans le but de détecter 4 types d’émotion dans les tweets du jeu de données (dataset) TweetEval Emotion.

NowUrCrown est une startup qui développe une plateforme de suivi d’audience pour les influenceurs du célèbre réseau social Twitter. Avec son application, elle propose notamment un tableau de bord présentant des statistiques et leurs visualisations et souhaite augmenter son offre de services (et d’indicateurs) grâce à des modèles prédictifs.

Afin de démontrer comment résoudre la problématique de NowUrCrown, nous avons implémenté un modèle de pointe, DeBERTaV3, et comparé ses performances à une baseline. Nous avons démontré que DeBERTaV3 dépasse largement le score F1 macro-moyenné de notre algorithme de référence USE sur le jeu de validation ainsi que le score de BERT (de 5.2 points) et de TimeLMs (de 2.2 points) sur le jeu de test de TweetEval Emotion.

## Données

GitHub du jeu de données utilisé: [Git](https://github.com/cardiffnlp/tweeteval)

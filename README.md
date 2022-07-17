# TweetEvalEmotion

## Présentation

Le modèle BERT (Bidirectional Encoder Representations from Transformers) est l’un des premiers modèles transformeur (transformer). BERT est un modèle auto-attentif, ce qui lui permet de développer une compréhension statistique du langage avec lequel il a été entrainé sans requérir d’étiquetage des données (data labelling). Autrement dit, ce type de modèle peut être entrainé de manière auto-supervisée (self-supervised learning). C’est un avantage considérable dans le domaine du traitement du langage naturel (Natural Langage Processing - NLP) où la création de jeux de données supervisées représente un travail considérable pour l’homme.

NowUrCrown est une startup qui développe une plateforme de suivi d’audience pour les influenceurs du célèbre réseau social Twitter. Avec son application, elle propose notamment un tableau de bord présentant des statistiques et leurs visualisations et souhaite augmenter son offre de services (et d’indicateurs) grâce à des modèles prédictifs.
L’un des objectifs de l’entreprise est d’avoir la capacité de détecter les sentiments présents dans les tweets afin d’offrir aux influenceurs une compréhension plus poussée de leur audience. NowUrCrown a d’ores et déjà implémenté l’algorithme Universal Sentence Encoder (USE) dont les performances ne sont pas satisfaisantes, elle a donc fait appel à nous pour implémenter un modèle de pointe dans une preuve de concept (POC).

Nous avons utilisé le jeu de données TweetEval afin de réaliser le POC. Le jeu de données est composé de 7 (sous) jeux de données qui permettent d’entrainer des algorithmes sur des tâches de classification binaire et multiple. Nous avons sélectionné la tâche « Emotion », qui regroupe 4 classes : « colère » (« anger »), « joie » (« joy »), « tristesse » (« sadness »), « optimisme » (« optimism »), et avons donc fait face à une problématique de classification multiple.

Afin de démontrer comment résoudre la problématique de NowUrCrown, nous avons implémenté un modèle de pointe, DeBERTaV3, et comparé ses performances à une baseline. Nous avons démontré que DeBERTaV3 dépasse largement le score F1 macro-moyenné de notre algorithme de référence USE sur le jeu de validation ainsi que le score de BERT (de 5.2 points) et de TimeLMs (de 2.2 points) sur le jeu de test de TweetEval Emotion.

## Données

GitHub du jeu de données utilisé: [Git](https://github.com/cardiffnlp/tweeteval)

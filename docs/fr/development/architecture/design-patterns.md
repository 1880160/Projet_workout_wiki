# Modèles de conception utilisés dans le projet

## Composite

Le modèle composite sera utilisé pour structurer nos routes. Par conséquent, les sous-routes seront contenues dans des sous-dossiers avec une structure similaire aux routes de l'API/frontend.

## Singleton

NestJs utilise le singleton par défaut dans son dépôt.

## Décorateur

Le décorateur sera utilisé pour injecter du code dans les fonctions et les routes
afin de réduire considérablement la quantité de code et d'améliorer la lisibilité du code.

## Observateur

Le serveur utilisera les SSE (Server Side Events) pour notifier le client des notifications en temps réel telles que les alertes d'entraînement et les demandes d'évaluation d'exercices.

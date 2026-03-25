# Patrons de conception utilisés dans le projet

## Composite

Le patron composite sera utilisé pour structurer nos routes. Par conséquent, les sous-routes seront contenues dans des sous-dossiers selon une structure similaire aux routes de l'API/frontend.

## Singleton

NestJs utilise le patron singleton par défaut dans son dépôt.

## Décorateur

Le patron décorateur sera utilisé pour injecter du code dans les fonctions et les routes
afin de réduire considérablement la quantité de code et d'améliorer la lisibilité du code.

## Observateur

Le serveur utilisera les SSE (Server Side Events) pour notifier le client en temps réel, notamment pour les alertes d'entraînement et les demandes de révision d'exercices.

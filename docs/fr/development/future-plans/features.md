# Fonctionnalités

Voici la liste des fonctionnalités qui sont prévues ou en discussion.

## Fonctionnalités prévues

Ce sont les fonctionnalités sur lesquelles l'accent sera mis car elles sont confirmées comme nécessaires ou souhaitées pour l'application.
Notez que les corrections de bogues et la refactorisation du code de l'application ne sont pas incluses ici.

### La page d'entraînement « Lecture/Exécution »

Cette page est destinée à être utilisée pendant un entraînement. Elle aura une interface simple qui affiche les exercices d'une séance d'entraînement. Elle disposera de fonctionnalités telles qu'un minuteur, un moyen de marquer les exercices comme terminés et un changement automatique d'exercices pour les entraînements de type circuit.

### Application mobile avec capacitorjs

L'interface utilisateur recevra une version mobile utilisant capacitor. Cela facilitera l'utilisation de l'application lorsqu'on l'utilise loin d'un ordinateur. De plus, capacitor ne nécessite pas de réécrire l'implémentation web, ce qui permettra de synchroniser facilement avec l'interface web.

## Fonctionnalités en discussion

Ce sont des fonctionnalités qui ne sont pas encore confirmées, mais qui sont sérieusement envisagées.

### Rendre l'application client d'abord

Cela permettra de faire en sorte que l'application ne nécessite pas de backend pour fonctionner. Le backend ne sera requis que pour la synchronisation.
Rxdb, Powersync ou Electric Sql pourraient être utilisés pour synchroniser une base de données sqlite locale avec une base de données plus importante.

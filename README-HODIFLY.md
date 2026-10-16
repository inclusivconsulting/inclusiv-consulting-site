# Déploiement du site INCLUSIV avec Hodifly

## Paramètres du projet

- Type : site statique
- Branche recommandée : `main`
- Chemin du paquet : racine du dépôt
- Commande de build : aucune
- Dossier de sortie : `dist`
- Runtime : `none`
- Variables d'environnement obligatoires : aucune

Le fichier `hodifly.json` placé à la racine versionne ces paramètres avec le site.

## Vérification avant déploiement

Le dossier `dist` doit toujours contenir `index.html` et le dossier `assets`.
Les chemins des ressources doivent rester relatifs afin que le site fonctionne aussi bien à la racine d'un domaine que dans un sous-dossier.

## Premier déploiement

1. Publier ce dépôt sur GitHub ou GitLab.
2. Ouvrir Hodifly dans cPanel et connecter le compte GitHub ou le projet GitLab.
3. Créer un projet à partir du dépôt et sélectionner la branche `main`.
4. Choisir le domaine ou le sous-dossier de destination.
5. Vérifier les paramètres détectés : site statique, aucune commande de build et sortie `dist`.
6. Créer le projet. Hodifly lance immédiatement le premier déploiement.
7. Consulter le journal de déploiement et vérifier que `dist/index.html` a été publié.

Les déploiements suivants seront déclenchés automatiquement à chaque push sur la branche sélectionnée.

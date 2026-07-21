# Solid-R_Nanterre
# Hébergement et gestion — Solid'R

## Structure fournie

- `index.html` : site public principal.
- `admin.html` : page d'administration simple.
- `content.json` : fichier de contenu dynamique.
- `img/` : dossier des photos, vidéos et logo.

## Héberger sur GitHub Pages

1. Créer un dépôt GitHub, par exemple `solidr-site`.
2. Envoyer tous les fichiers du dossier dans le dépôt.
3. Aller dans **Settings > Pages**.
4. Choisir la branche principale (`main`) et le dossier racine (`/root`).
5. GitHub Pages publiera automatiquement le site.

Le site sera ensuite accessible sur une URL du type :
`https://ton-compte.github.io/solidr-site/`

## Gestion simple sans code

### Méthode actuelle

La personne qui gère le site peut :
1. Ouvrir `admin.html`.
2. Entrer le mot de passe.
3. Modifier les champs.
4. Télécharger le nouveau `content.json`.
5. Remplacer l'ancien fichier dans GitHub.

### Ajouter une nouvelle image

1. Mettre l'image dans le dossier `img/`.
2. Dans `admin.html`, renseigner par exemple `./img/nouvelle-photo.jpg`.
3. Générer puis télécharger `content.json`.
4. Republier sur GitHub.

## Sécurité

La page admin fournie est simple, mais **ce n'est pas une sécurité serveur forte**. Le mot de passe est côté client, donc suffisant pour une démo ou une petite gestion interne, mais pas pour un environnement sensible.

## Recommandation sécurisée ensuite

Pour une vraie gestion simple + plus sécurisée, je te conseille ensuite :

### Option recommandée
- GitHub Pages pour le site public.
- Decap CMS (ancien Netlify CMS) ou TinaCMS pour l'édition sans code.
- Authentification GitHub pour les personnes autorisées.
- Les contenus restent dans GitHub, avec historique et contrôle.

### Pourquoi c'est mieux
- pas de code à écrire pour la gestion courante ;
- seules les personnes autorisées peuvent publier ;
- chaque changement est versionné ;
- la galerie et la "dernière action" peuvent être modifiées plus proprement.

## Ce que je te conseille concrètement

1. Utiliser tout de suite la version fournie pour voir le rendu.
2. Héberger le site sur GitHub Pages.
3. Dans un second temps, migrer la partie admin vers Decap CMS pour avoir une vraie édition sécurisée et simple.

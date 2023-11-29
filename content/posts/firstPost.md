+++
title = 'Début avec Hugo'
date = 2023-11-14T11:38:14+01:00
draft = false
summary = "Résumé des concepts vus en cours"
+++

![Logo hugo](https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Logo_of_Hugo_the_static_website_generator.svg/512px-Logo_of_Hugo_the_static_website_generator.svg.png)

## Mes débuts avec Hugo

### Initialisation du projet

***Les nouvelles notions apprises de cette partie:***
- ***Créer un site avec hugo***
- ***Choisir et installer un thème***
- ***Démarré le serveur de développement Hugo***

Je n'avais jamais utiliser (ni même entendu parler de Hugo), j'ai pu donc dans ce cours m'initier à ce générateur de site statiques.
Après avoir installer Hugo, j'ai pu **créer un site avec la commande**:
```
hugo new site nomDeMonSite
```

Après être entrer dans le dossier du site, j'ai initialisé un nouveau dépôt Git et j'y ai installer un nouveau thème.
```
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git
```

J'ai ensuite démarré le serveur de développement de Hugo pour pouvoir afficher mon site:
```
hugo server
```
Et également j'ai pu voir comment démarré le serveur tout en incluant les **drafts**:
```
hugo server -D
```

### Premiers contenu et Surcharge de templates
***Les nouvelles notions apprises de cette partie:***
- ***Créer un nouveau contenu en ligne de commande avec Hugo***
- ***Surcharger des templates***
- ***Ajouter/Modifier du CSS au thème choisi***

Après avoir afficher mon site, j'ai créer mon premier contenu.
```
hugo new content posts/firstPost.md
```
Également, en suivant le cours (pdf) j'ai pu **surcharger** le template que j'avais choisi. J'ai donc modifié des parties spécifiques, le header et le footer du thème tout en ajouter ma propre feuille de style css.
- Surcharge du header + footer: créations des fichiers dans **layout/partials/** avec le même noms du fichier du thème pour le surcharger
- Pour le css, même chose sauf qu'il faut créer le fichier dans static/css/ + ajouter un lien vers la feuille de style créer dans un nouveau fichier **layouts/partials/head-additions.html**

### Hébergement de mon site Hugo

***Les nouvelles notions apprises de cette partie:***
- ***Déployer un site Hugo sur GitHub Pages***
- ***Déployer un site Hugo avec GitHub Actions***

Pour le déploiement nous avons commencer par voir comment déployer mon site avec GitHub Pages.
Pour cela dans le dossier public j'ai fais un **git init**, créer une nouvelle branche **git branch -M gh-pages**, add commit et push sur mon repo.
Et pour terminer j'ai configurer GitHub Pages en sélectionnant ma nouvelle branche dans mon repo github (Settings-->Pages)

Nous avons ensuite vu comment déployer le site avec GitHub Actions. Pour cela j'ai remodifié les settings de mon repo en sélectionnant *GitHub Actions*. J'ai ensuite créer un fichier *github/workflows/hugo-deploy.yml* + repris le contenu du fichier yaml qu'il y avait dans la doc officiel de Hugo. J'ai add commit et push et de nouveau mon site ce déployait automatiquement quand je pushais des modifications
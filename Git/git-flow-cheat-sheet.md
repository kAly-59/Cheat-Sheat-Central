# GitFlow Cheat Sheet

## Install Git Flow via apt-get
```
sudo apt-get update
sudo apt-get install git-flow
```

### Verify Git Flow installation
```
git flow version
```

### Initialisation
```
git flow innit
```

## Création d'une Nouvelle Fonctionnalité
```bash
git flow feature start nom-de-la-fonctionnalite
```

## Finalisation de la Fonctionnalité
```bash
git flow feature finish nom-de-la-fonctionnalite
```

## Création d'une Version
```bash
git flow release start numero-de-version
```
## Finalisation d'une Version
```bash
git flow release finish numero-de-version
```

## Correction de Bugs
```bash
git flow hotfix start nom-du-correctif
```
```bash
git flow hotfix finish nom-du-correctif
```

## Publier et Partager Votre Travail
```bash
git push origin nom-de-la-branche
```

# GIT Cheat Sheet

## Installation Git

### Installation
```
sudo apt install git
```
### Mettre à jour
```
sudo apt upgrade git
sudo apt-get update #Exécuter si des problèmes de mise à jour sont rencontrés
```
### Configurer Git (Nom et Adresse Email)
```
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```
### Vérifier la version de Git installée
```
git --version
```
---

## Pousser des Modifications ##

### 1. Accéder au fichier :
   ```
   code nom.du.fichier.md
   ```
### 2. Ajouter les modifications au suivi de Git avec `git add` :
   ```
   git add nom.du.fichier.md
   ```
   Ou (Pour tout les fichiers)
   ```
   git add .
   ```
### 3. Effectuer un commit avec un message descriptif :
   ```
   git commit -m "Information sur la/les modifications"
   ```
### 4. Pousser les modifications vers votre branche principale (`main`) sur GitHub :
   ```
   git push origin main
   ```

---

## Mettre à jour un Fork GitHub origin/upstream ##

### 1. Ajouter/Modifier le dépôt source en tant que remote :
   ```
   git remote add origin/upstream "Lien GIT"
   ```
### 2. Récupérer les dernières modifications depuis le dépôt original avec `git fetch` :
   ```
   git fetch origin/upstream "branch"
    
   ```
### 3. Fusionner les modifications dans votre branche locale (par exemple, `main`) :
   ```
   git merge origin/upstream "branch"
   ```
### 4. Pousser les modifications vers votre fork sur GitHub :
   ```
   git push origin "branch"
   ```
### Voir les remotes :
   ```
   git remote -v
   ```
Exemple :
   ```
   origin  git@github.com:kAly-59/cheat-sheets-github-cli.git (fetch)
   origin  git@github.com:kAly-59/cheat-sheets-github-cli.git (push)
   upstream        https://github.com/Simplon-hdf/cheat-sheets-github-cli.git (fetch)
   upstream        https://github.com/Simplon-hdf/cheat-sheets-github-cli.git (push) #Upstream toujours en https
   ```

---

## GIT SWITCH

### 1. **Vérifier l'état actuel :**
   ```
   git status
   ```

### 2. **Lister les branches :**
   ```
   git branch
   ```

### 3. **Changer de branche existante :**
   ```
   git switch nom-de-la-branche
   ```

### 4. **Créer une nouvelle branche et y basculer (à partir d'une branche distante) :**
   ```
   git switch -c nom-de-la-nouvelle-branche origin/nom-de-la-branche-distante
   ```

---

## Commandes Git ##

1. **`git init` :**
   - *Fonctionnement :* Initialise un nouveau dépôt Git dans un répertoire existant.
   - *Utilité :* Utilisé pour commencer un nouveau projet Git. Le répertoire devient un dépôt Git, prêt à enregistrer les modifications.

2. **`git add` :** (UNIQUE / . / ALL)
   - *Fonctionnement :* Ajoute des modifications spécifiques (ou tous les fichiers modifiés) à la staging area (zone de préparation).
   - *Utilité :* Sélectionne les modifications à inclure dans le prochain commit. Peut ajouter des fichiers individuels (`git add nom_du_fichier`) ou tous les fichiers modifiés (`git add .` ou `git add --all`).

3. **`git status` :**
   - *Fonctionnement :* Affiche l'état des fichiers dans le répertoire de travail et de la staging area.
   - *Utilité :* Permet de voir les fichiers modifiés, ceux dans la staging area et si tout est prêt pour le commit.

4. **`git commit` :**
      ```
      git commit -m "Message du commit"
      ```
   - *Fonctionnement :* Crée un nouveau commit avec les modifications de la staging area.
   - *Utilité :* Enregistre les modifications dans l'historique du projet. Le message de commit décrit les changements effectués.

6. **`git pull` :**
   - *Fonctionnement :* Récupère les modifications depuis un dépôt distant et les fusionne dans votre branche actuelle.
   - *Utilité :* Met à jour votre copie locale avec les dernières modifications du dépôt distant.

7. **`git push` :**
      ```
      git push origin nom_de_la_branche
      ```
   - *Fonctionnement :* Envoie les commits locaux vers un dépôt distant.
   - *Utilité :* Partage vos modifications avec les collaborateurs en poussant les commits vers le dépôt distant. Remplacez `nom_de_la_branche` par le nom de votre branche.

9. **`git clone` :**
   - *Fonctionnement :* Crée une copie locale d'un dépôt distant existant.
   - *Utilité :* Permet de créer une copie de travail d'un projet distant sur votre machine pour contribuer au projet.

10. **`git remote` :**
   - *Fonctionnement :* Gère les dépôts distants associés à votre projet local.
   - *Utilité :* Permet d'ajouter, afficher ou supprimer des dépôts distants. Vous pouvez également renommer ou mettre à jour les URL des dépôts distants avec cette commande.

---

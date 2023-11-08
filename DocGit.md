# GIT

1. [Installation Git](#Installation-Git)
2. [Installer GitHub CLI](#Installer-GitHub-CLI)
3. [Installation Git Flow ](#Installation-Git-Flow)
5. [Pousser des Modifications](#Pousser-des-Modifications)
6. [Mettre à jour un Fork GitHub](#Mettre-à-jour-un-Fork-GitHub)
7. [Git Switch](#Git-Switch)
8. [SSH pour GitHub](#SSH-pour-GitHub)

## 1. Installation Git
### 1. Installation
```
sudo apt install git
```
### 2. Mettre à jour
```
sudo apt upgrade git
sudo apt-get update #Exécuter si des problèmes de mise à jour sont rencontrés
```
### 3. Configurer Git (Nom et Adresse Email)
```
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```
### Vérifier la version de Git installée
```
git --version
```

***  

## Installer GitHub CLI ##

### 1. **Installation :**
```
sudo apt update
sudo apt install gh
```
### 2. **Vérifier l'installation :**
```
gh --version
```
### 3. **S'authentifier avec votre compte GitHub :**
```
gh auth login
```

***

## Installation Git Flow 

### Install Git Flow via apt-get
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

***

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

   ***

## Mettre à jour un Fork GitHub ##

### 1. Ajouter le dépôt source en tant que remote :
   ```
   git remote add upstream "Lien GIT"
   ```
### 2. Récupérer les dernières modifications depuis le dépôt original avec `git fetch` :
   ```
   git fetch origin "main"
   ```
   Ou
   ```
   git pull upstream main 
   ```
### 3. Fusionner les modifications dans votre branche locale (par exemple, `main`) :
   ```
   git merge upstream/main
   ```
### 4. Pousser les modifications vers votre fork sur GitHub :
   ```
   git push origin main
   ```
### Voir les remotes :
   ```
   git remote -v
   ```
   
***

## GIT SWITCH ##

###1. **Vérifier l'état actuel :**
   ```
   git status
   ```

###2. **Lister les branches :**
   ```
   git branch
   ```

###3. **Changer de branche existante :**
   ```
   git switch nom-de-la-branche
   ```

###4. **Créer une nouvelle branche et y basculer (à partir d'une branche distante) :**
   ```
   git switch -c nom-de-la-nouvelle-branche origin/nom-de-la-branche-distante
   ```
   
***

## SSH pour GitHub ##

### 1. **Générer une nouvelle clé SSH :**
   ```
   ssh-keygen -t ed25519 -C "your_email@example.com"
   ```
### 2. **Démarrer l'agent SSH en arrière-plan :**
   ```
   eval "$(ssh-agent -s)"
   ```
### 3. **Ajouter votre clé privée SSH à ssh-agent :**
   ```
   ssh-add ~/.ssh/id_ed25519
   ```
### 4. **Ajouter une nouvelle clé SSH à votre compte GitHub :**
   Suivez les instructions de GitHub pour ajouter votre clé SSH à votre compte :
   - [Ajouter une nouvelle clé SSH à votre compte GitHub](https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
### **Vérifier les clés SSH existantes :**
   ```
   ls -al ~/.ssh
   ```
   Cette commande affiche les clés SSH existantes dans votre répertoire `~/.ssh`.

***

## Gestion des Permissions sur Linux ##

### **Vérifier les Droits :**
Pour vérifier les permissions d'un dossier sous Linux, utilisez la commande `ls -l` dans un terminal :
```
ls -l /chemin/vers/le/dossier
```

### **Modifier les Droits :**
Pour modifier les permissions d'un dossier sous Linux et permettre à tous les utilisateurs d'écrire dans le dossier `DocForm`, utilisez `chmod` avec `sudo` pour ajouter la permission d'écriture pour les autres utilisateurs (`o+w`). Assurez-vous de remplacer `/chemin/vers/DocForm` par le chemin d'accès réel du dossier que vous souhaitez modifier :
```
sudo chmod o+w /chemin/vers/DocForm
```

***

## Définitions et Concepts Git ##

### **Local :**
Votre copie du dépôt sur votre machine locale, où vous effectuez des modifications et travaillez sur votre code.

### **Origin :**
Le dépôt distant à partir duquel vous avez cloné votre projet. C'est généralement votre fork personnel du dépôt original.

### **Upstream :**
Le dépôt distant original à partir duquel votre fork a été créé. C'est le dépôt que vous souhaitez mettre à jour régulièrement avec les dernières modifications.

### **Chiffrement Asymétrique :**
Un système de chiffrement qui utilise deux clés distinctes : une clé publique pour chiffrer les données et une clé privée correspondante pour les déchiffrer. La clé publique peut être partagée, tandis que la clé privée doit être gardée secrète.

### **SemVer (Semantic Versioning) :**
Une convention de versionnement standardisée qui spécifie comment attribuer des numéros de version à un logiciel de manière significative. Une version SemVer est généralement représentée sous la forme de MAJOR.MINOR.PATCH, indiquant des changements majeurs, mineurs et de correctifs respectivement.

### **Fusion (Merge) :**
La fusion est une méthode pour intégrer les modifications d'une branche dans une autre. Elle crée un nouveau commit de fusion qui représente l'état combiné des deux branches. La fusion préserve l'historique original des branches, ce qui permet de suivre l'évolution du code de manière détaillée.

### **Ré-ensemencement (Rebase) :**
Le ré-ensemencement est une technique pour intégrer les modifications en modifiant l'historique des commits. Il retire les commits de la branche source de leur emplacement d'origine et les applique un par un sur la branche cible. Cela crée une ligne d'historique linéaire et nette, sans les commits de fusion supplémentaires. Le ré-ensemencement peut rendre l'historique du projet plus facile à suivre, mais il modifie l'historique existant et peut entraîner des conflits.

En résumé, la fusion crée un historique plus complexe mais sécurisé, tandis que le ré-ensemencement crée un historique linéaire et lisible, mais peut être risqué en modifiant l'historique existant. Le choix entre les deux dépend des préférences de l'équipe et des exigences du projet spécifique.

***

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

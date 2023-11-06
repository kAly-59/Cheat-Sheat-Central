# GIT

**Installation sur Linux :**
```
sudo apt install git
```

**Configuration de Git :**
```
git --version
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```

***  

### TUTO

1. Acceder au fichier :
   ```
   code nom.du.fichier.md
   ```
2. ADD :
   ```
   git add nom.du.fichier.md
   ```
3. COMMIT :
   ```
   git commit -m "Information sur la/les modifications"
   ```
4. PUSH : 
   ```
   git push origin main
   ```
5. REMOTE (Ajouter le dépôt distant upstream) :
   ```
   git remote add upstream "Lien GIT"
   ```
6. VERIFIER REMOTE :
   ```
   git remote -v
   ```
7. FETSH (Récupérer les dernières modifications depuis le dépôt original) :
   ```
   git fetch upstream + git merge
   ```
8. MERGE (Mettre à jour votre branche principale (habituellement main ou master) avec les modifications du dépôt original) :
   ```
   git checkout main
   ```
   ```
   git merge upstream/main
   ```
   
***

### Definitions

- **Local :** Votre copie du dépôt sur votre machine locale.
- **Origin :** Le dépôt distant à partir duquel vous avez cloné.
- **Upstream :** Le dépôt distant original à partir duquel votre fork a été créé.

**Chiffrement Asymétrique :**
- Le chiffrement asymétrique utilise deux clés distinctes :
   - *Une clé publique :* pour chiffrer les données et une clé privée correspondante pour les déchiffrer. La clé publique peut être partagée ou publiée largement.
   - *Une clé privée :* doit être gardée secrète. Cela élimine la nécessité d'un échange sécurisé de clés, mais les opérations de chiffrement et de déchiffrement sont généralement plus lentes que dans le chiffrement symétrique.

**SemVer** https://www.conventionalcommits.org/fr/v1.0.0/
   - Semantic Versioning (SemVer). SemVer est une convention de versionnement standardisée qui spécifie comment attribuer des numéros de version à un logiciel de manière significative.
   - Une version est généralement représentée sous la forme de MAJOR.MINOR.PATCH.

***
## *SSH*
https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
```
 ssh-keygen -t ed25519 -C "your_email@example.com"
```

*Démarrez l’agent SSH en arrière-plan.*
```
eval "$(ssh-agent -s)"
```
*Ajoutez votre clé privée SSH à ssh-agent.*
```
ssh-add ~/.ssh/id_ed25519
```
*Ajout d’une nouvelle clé SSH à votre compte GitHub :*
(https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
```
cat ~/.ssh/id_ed25519.pub
```
### *Vérification des clés SSH existantes*
https://docs.github.com/fr/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys
```
ls -al ~/.ssh
```

***

### Vérifier les Droits

Pour vérifier les permissions d'un dossier sous Linux, utilisez la commande `ls -l` dans un terminal. Par exemple :

```bash
ls -l /chemin/vers/le/dossier
```

Cette commande affichera une liste détaillée des fichiers et dossiers dans le répertoire spécifié, y compris les informations sur les permissions pour le propriétaire, le groupe et les autres utilisateurs.

### Modifier les Droits

Pour modifier les permissions d'un dossier sous Linux et permettre à tous les utilisateurs d'écrire dans le dossier `DocForm`, utilisez la commande `chmod` avec `sudo` pour ajouter la permission d'écriture pour les autres utilisateurs (`o+w`). Assurez-vous de remplacer `/chemin/vers/DocForm` par le chemin d'accès réel du dossier que vous souhaitez modifier. Par exemple :

```bash
sudo chmod o+w /chemin/vers/DocForm
```

***

## COMMANDES

1. **`git init` :**
   - *Fonctionnement :* Initialise un nouveau dépôt Git dans un répertoire existant.
   - *Utilité :* Utilisé pour commencer un nouveau projet Git. Le répertoire devient un dépôt Git, prêt à enregistrer les modifications.

2. **`git add` :** ( UNIQUE / . / ALL )
   - *Fonctionnement :* Ajoute des modifications spécifiques (ou tous les fichiers modifiés) à la staging area (zone de préparation).
   - *Utilité :* Sélectionne les modifications à inclure dans le prochain commit. Peut ajouter des fichiers individuels (`git add nom_du_fichier`) ou tous les fichiers modifiés (`git add all`).

3. **`git status` :**
   - *Fonctionnement :* Affiche l'état des fichiers dans le répertoire de travail et de la staging area.
   - *Utilité :* Permet de voir les fichiers modifiés, ceux dans la staging area, et si tout est prêt pour le commit.

4. **`git commit` :**
      ```
      git commit -m "Test"
      ```
   - *Fonctionnement :* Crée un nouveau commit avec les modifications de la staging area.
   - *Utilité :* Enregistre les modifications dans l'historique du projet. Un message de commit (`-m "Message du commit"`) décrit les changements effectués.

6. **`git pull` :**
   - *Fonctionnement :* Récupère les modifications depuis un dépôt distant et les fusionne dans votre branche actuelle.
   - *Utilité :* Met à jour votre copie locale avec les dernières modifications du dépôt distant.

7. **`git push` :**
      ```
      git push origin main
      ```
   - *Fonctionnement :* Envoie les commits locaux vers un dépôt distant.
   - *Utilité :* Partage vos modifications avec les collaborateurs en poussant les commits vers le dépôt distant.

9. **`git clone` :**
   - *Fonctionnement :* Crée une copie locale d'un dépôt distant existant.
   - *Utilité :* Permet de créer une copie de travail d'un projet distant sur votre machine pour contribuer au projet.

10. **`git remote` :**
   - *Fonctionnement :* Gère les dépôts distants associés à votre projet local.
   - *Utilité :* Permet d'ajouter, afficher ou supprimer des dépôts distants. Vous pouvez également renommer ou mettre à jour les URL des dépôts distants avec cette commande.

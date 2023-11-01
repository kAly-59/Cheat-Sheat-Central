## Raccourcis de Navigation

- **Ctrl + A :** Aller au début de la ligne.
- **Ctrl + E :** Aller à la fin de la ligne.
- **Ctrl + U :** Supprimer du curseur au début de la ligne.
- **Ctrl + K :** Supprimer du curseur à la fin de la ligne.
- **Ctrl + W :** Supprimer le mot précédent (en partant du curseur).
- **Ctrl + L :** Effacer l'écran (fonctionne comme la commande "clear").

## Raccourcis de Copie/Coller :

- **Ctrl + Shift + C :** Copier du texte (sélectionné avec la souris).
- **Ctrl + Shift + V :** Coller du texte dans le terminal.

## Raccourcis de Gestion de l'Historique :

- **Ctrl + R :** Rechercher dans l'historique des commandes.
- **!! :** Exécuter la dernière commande.
- **!n :** Exécuter la n-ème commande dans l'historique (remplacez "n" par le numéro de commande).

## Raccourcis pour la Gestion des Onglets :

- **Ctrl + Shift + T :** Ouvrir un nouvel onglet.
- **Ctrl + Shift + W :** Fermer l'onglet actuel.

## Raccourcis pour la Navigation Entre les Onglets :

- **Ctrl + Page Up / Page Down :** Aller à l'onglet précédent/suivant.

## Autres Raccourcis Utiles :

- **Tab :** Auto-complétion des fichiers et dossiers dans le répertoire courant.
- **Ctrl + D :** Déconnexion du terminal (équivalent à la commande "exit").
- **Ctrl + C :** Interrompre l'exécution d'une commande en cours.
- **Ctrl + Z :** Mettre une commande en arrière-plan.
- **fg :** Reprendre une commande en arrière-plan en premier plan.

---

### Commandes Utiles :

- **`touch fichier.md` :** Création de fichier.
- **`nano fichier.md` :** Lire fichier & modifier.
- **`cat fichier.md` :** Lecture dans le terminal.
- **`ls` :** Voir les fichiers.

---

### GIT :

**Installation sur Linux :** sudo apt install git
```

**Configuration de Git :**
```
git --version
git config --global user.name "Votre Nom"
git config --global user.email "votre@email.com"
```

1. **`git init` :**
   - *Fonctionnement :* Initialise un nouveau dépôt Git dans un répertoire existant.
   - *Utilité :* Utilisé pour commencer un nouveau projet Git. Le répertoire devient un dépôt Git, prêt à enregistrer les modifications.

2. **`git add` :**
   - *Fonctionnement :* Ajoute des modifications spécifiques (ou tous les fichiers modifiés) à la staging area (zone de préparation).
   - *Utilité :* Sélectionne les modifications à inclure dans le prochain commit. Peut ajouter des fichiers individuels (`git add nom_du_fichier`) ou tous les fichiers modifiés (`git add .`).

3. **`git status` :**
   - *Fonctionnement :* Affiche l'état des fichiers dans le répertoire de travail et de la staging area.
   - *Utilité :* Permet de voir les fichiers modifiés, ceux dans la staging area, et si tout est prêt pour le commit.

4. **`git commit` :**
   - *Fonctionnement :* Crée un nouveau commit avec les modifications de la staging area.
   - *Utilité :* Enregistre les modifications dans l'historique du projet. Un message de commit (`-m "Message du commit"`) décrit les changements effectués.

5. **`git pull` :**
   - *Fonctionnement :* Récupère les modifications depuis un dépôt distant et les fusionne dans votre branche actuelle.
   - *Utilité :* Met à jour votre copie locale avec les dernières modifications du dépôt distant.

6. **`git push` :**
   - *Fonctionnement :* Envoie les commits locaux vers un dépôt distant.
   - *Utilité :* Partage vos modifications avec les collaborateurs en poussant les commits vers le dépôt distant.

7. **`git clone` :**
   - *Fonctionnement :* Crée une copie locale d'un dépôt distant existant.
   - *Utilité :* Permet de créer une copie de travail d'un projet distant sur votre machine pour contribuer au projet.

8. **`git remote` :**
   - *Fonctionnement :* Gère les dépôts distants associés à votre projet local.
   - *Utilité :* Permet d'ajouter, afficher ou supprimer des dépôts distants. Vous pouvez également renommer ou mettre à jour les URL des dépôts distants avec cette commande.

---

### Markdown :

#### Titres :
```markdown
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
```

#### Images :
```markdown
![Texte alternatif](URL_de_l_image)
```

#### Listes :
```markdown
- Élément 1
- Élément 2
  - Sous-élément A
  -

 Sous-élément B
```

#### Texte En Italique et Gras :
```markdown
*Texte en italique*
**Texte en gras**
```

#### Bloc de Code :
```markdown
```
Code ici
```
```

#### Citations :
```markdown
> Ceci est une citation.
```

#### Tableaux :
```markdown
| En-tête 1 | En-tête 2 |
|-----------|-----------|
| Cellule 1 | Cellule 2 |
```

#### Liens :
```markdown
[Texte du lien](URL)
```

---

### Option Commandes :

- **Options Courtes :** Généralement représentées par un seul tiret suivi d'une lettre (par exemple, -l).
- **Options Longues :** Précédées de deux tirets (par exemple, --color).
- **Combinaison d'Options :** Parfois, plusieurs courtes options peuvent être combinées après un seul tiret (par exemple, `ls -la`).
- **Options avec Arguments :** Certaines options nécessitent un argument pour spécifier une valeur.

- **Aide et Documentation :** Pour connaître les options disponibles pour une commande, utilisez les options `-h` ou `--help` (par exemple, `ls --help` affiche l'aide pour la commande ls).

---

[Documentation Terminator](https://terminator-gtk3.readthedocs.io/en/latest/)

---

#### Différence Entre CLI et GUI :

Une interface en ligne de commande (CLI) permet aux utilisateurs de donner des instructions à un ordinateur en tapant des commandes textuelles, tandis qu'une interface graphique (GUI) permet aux utilisateurs d'interagir avec l'ordinateur à travers des éléments visuels tels que des fenêtres, des icônes et des boutons en utilisant une souris.

---

#### Le Shell, Qu'est-ce que C'est ?

Un shell est un programme informatique qui agit comme une interface utilisateur en ligne de commande pour interagir avec un système d'exploitation. Il permet de taper des commandes et exécute des programmes correspondants, gère la redirection de flux de données, la création de processus et l'exécution de scripts. Les shells offrent des fonctionnalités avancées telles que l'historique des commandes, l'autocomplétion et la gestion des variables d'environnement.

---

#### Alias :

Un alias sous Linux est un raccourci personnalisé pour une commande ou une série de commandes. Il simplifie l'utilisation des commandes fréquemment utilisées en remplaçant leur nom par un mot-clé ou une abréviation.

---

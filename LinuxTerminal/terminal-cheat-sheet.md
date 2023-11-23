# Terminal Linux Cheat Sheet

- [Raccourcis de Navigation](#raccourcis-de-navigation)
- [Raccourcis de Copie/Coller](#raccourcis-de-copiecoller)
- [Raccourcis de Gestion de l'Historique](#raccourcis-de-gestion-de-lhistorique)
- [Raccourcis pour la Gestion des Onglets](#raccourcis-pour-la-gestion-des-onglets)
- [Raccourcis pour la Navigation Entre les Onglets](#raccourcis-pour-la-navigation-entre-les-onglets)
- [Autres Raccourcis Utiles](#autres-raccourcis-utiles)
- [Commandes Utiles](#commandes-utiles)
- [Markdown](#markdown)
- [Option Commandes](#option-commandes)
- [Documentation Terminator](#documentation-terminator)
- [Différence Entre CLI et GUI](#différence-entre-cli-et-gui)
- [Le Shell, Qu'est-ce que C'est ?](#le-shell-quest-ce-que-cest)
- [Alias](#alias)

---
## Raccourcis

### Navigation
- **Ctrl + A :** Aller au début de la ligne.
- **Ctrl + E :** Aller à la fin de la ligne.
- **Ctrl + U :** Supprimer du curseur au début de la ligne.
- **Ctrl + K :** Supprimer du curseur à la fin de la ligne.
- **Ctrl + W :** Supprimer le mot précédent (en partant du curseur).
- **Ctrl + L :** Effacer l'écran (fonctionne comme la commande "clear").

### Copie/Coller
- **Ctrl + Shift + C :** Copier du texte (sélectionné avec la souris).
- **Ctrl + Shift + V :** Coller du texte dans le terminal.

### Gestion de l'Historique
- **Ctrl + R :** Rechercher dans l'historique des commandes.
- **!! :** Exécuter la dernière commande.
- **!n :** Exécuter la n-ème commande dans l'historique (remplacez "n" par le numéro de commande).

### Gestion des Onglets
- **Ctrl + Shift + T :** Ouvrir un nouvel onglet.
- **Ctrl + Shift + W :** Fermer l'onglet actuel.

### Navigation Entre les Onglets
- **Ctrl + Page Up / Page Down :** Aller à l'onglet précédent/suivant.

### Autres
- **Tab :** Auto-complétion des fichiers et dossiers dans le répertoire courant.
- **Ctrl + D :** Déconnexion du terminal (équivalent à la commande "exit").
- **Ctrl + C :** Interrompre l'exécution d'une commande en cours.
- **Ctrl + Z :** Mettre une commande en arrière-plan.
- **fg :** Reprendre une commande en arrière-plan en premier plan.
- 
### Commandes Utiles
- **`touch fichier.md` :** Création de fichier.
- **`nano fichier.md` :** Lire fichier & modifier.
- **`cat fichier.md` :** Lecture dans le terminal.
- **`ls` :** Voir les fichiers.

---

## Markdown

### Titres :
```markdown
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
```

### Liens :
```markdown
[Texte du lien](URL)
```

### Images :
```markdown
![Texte alternatif](URL_de_l_image)
```

### Listes :
```markdown
- Élément 1
- Élément 2
  - Sous-élément A
  - Sous-élément B
```

### Texte En Italique et Gras :
```markdown
*Texte en italique*
**Texte en gras**
```

### Bloc de Code :
```markdown
```

### Citations :
```markdown
> Ceci est une citation.
```

#### Tableaux :
```markdown
| En-tête 1 | En-tête 2 |
|-----------|-----------|
| Cellule 1 | Cellule 2 |
```

---

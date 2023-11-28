 # Cheat Sheet npm (Ubuntu)

## Gestion des Paquets
### Installer un package localement
```bash
npm install <package_name>
```

### Installer un package globalement
```bash
npm install -g <package_name>
```

### Mettre à jour un package spécifique
```bash
npm update <package_name>
```

### Mettre à jour tous les packages
```bash
npm update
```

### Supprimer un package localement
```bash
npm uninstall <package_name>
```

### Supprimer un package global
```bash
npm uninstall -g <package_name>
```

---

## Gestion des Projets
### Initialiser un projet npm (créer un `package.json`)
```bash
npm init
```

### Exécuter un script spécifique

```bash
npm run <script_name>
```

### Installer uniquement les dépendances de production

```bash
npm install --only=prod
```

---

## Autres Commandes Utiles
### Voir les packages installés localement
```bash
npm list
```

### Voir les packages installés globalement
```bash
npm list -g
```

### Obtenir de l'aide sur une commande spécifique
```bash
npm <command> --help
```

---
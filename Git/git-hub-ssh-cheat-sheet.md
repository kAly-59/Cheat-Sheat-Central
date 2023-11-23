# GitHub SSH Sheat Cheat ##

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

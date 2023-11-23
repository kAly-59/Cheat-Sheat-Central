# PostgreSQL Cheat Sheet

## Installation de PostgreSQL sur Ubuntu

1. Ouvrez votre terminal WSL.
2. Mettez à jour vos paquets Ubuntu : 
    ```bash
    sudo apt update
    ```
3. Installez PostgreSQL (et le paquet -contrib qui a quelques utilitaires utiles) avec : 
    ```bash
    sudo apt install postgresql postgresql-contrib
    ```
4. Confirmez l'installation et obtenez le numéro de version : 
    ```bash
    psql --version
    ```

**Après votre première installation, et chaque fois que vous redémarrez votre machine, vous devrez également redémarrer le service postgres, sinon vous obtiendrez une erreur 'Le serveur est-il en cours d'exécution ?'.**

5. Démarrez votre service postgres : 
    ```bash
    sudo service postgresql start
    ```
6. Connectez-vous au service postgres et ouvrez le shell psql : 
    ```bash 
    sudo -u postgres psql
    ```
7. Vous verrez votre ligne de commande changer pour ressembler à ceci : 
    ```sql
    postgres=#
    ```
8. L'utilisateur admin par défaut, postgres, a besoin d'un mot de passe assigné pour se connecter à une base de données. Pour définir un mot de passe : 
    ```sql
    \password postgres
    ```
    Vous obtiendrez une invite pour entrer votre nouveau mot de passe. Fermez et rouvrez votre terminal.

<br>

---

<br>

## Création & suppression base de données

1. Pour voir quelles bases de données vous avez disponibles, dans l'invite MySQL, entrez : 
    ```sql
    \l
    ```
2. Pour créer une nouvelle base de données, entrez : 
    ```sql
    CREATE DATABASE nom_de_la_base_de_donnees;
    ```
3. Pour supprimer une base de données, entrez : 
    ```sql
    DROP DATABASE nom_de_la_base_de_donnees;
    ```

<br>

---

<br>

## Création & suppression compte utilisateur

1. Ouvrez une fenêtre de terminal.
2. Connectez-vous à PostgreSQL :
    ```bash 
    sudo -u postgres psql
    ```
3. Créer un nouvel utilisateur, `CREATE USER` :
    ```sql
    CREATE USER nom_utilisateur WITH PASSWORD 'mot_de_passe';
    ```
4. Supprimer un utilisateur, `DROP USER` :
    ```sql
    DROP USER nom_utilisateur;
    ```
5. Voir les utilisateurs :
    ```sql
    \du
    ```

**Note :** Assurez-vous d'avoir les privilèges nécessaires pour créer et supprimer des utilisateurs dans PostgreSQL. De plus, faites attention lorsque vous supprimez des utilisateurs, car cela peut affecter l'accès aux bases de données et aux tables.

---


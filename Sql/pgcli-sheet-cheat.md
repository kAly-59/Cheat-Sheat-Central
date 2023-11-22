# Installation `pgcli` :

## Installation :

### Assurez-vous que `pip` est installé :
Si vous n'avez pas encore installé `pip`, vous pouvez le faire en exécutant la commande suivante dans votre terminal :
```bash
sudo apt update
sudo apt install python3-pip
```
### Installation de `pgcli` :
Après avoir installé `pip`, exécutez la commande suivante pour installer `pgcli` :
```bash
sudo pip3 install pgcli
```
### Utilisation de `pgcli` :

Utiliser `pgcli` pour vous connecter à votre base de données PostgreSQL en utilisant la commande suivante :
```bash
pgcli -h <hôte> -U <utilisateur> -d <base_de_données>
```

<br>

***

<br>

## Création d'une base de données :

**Connexion à PostgreSQL :** 
```bash
pgcli -h <hôte> -U <utilisateur>
```
**Création & Suppression base de données :**

```sql
CREATE DATABASE <nom_de_la_base_de_données>;
```
```sql
DROP DATABASE <nom_de_la_base_de_données>;
```

<br>

***

<br>

```markdown
## pgcli Cheat Sheet

### Connexion à la base de données
- Connexion à une base de données : `pgcli -h <hôte> -U <utilisateur> -d <base_de_données>`
- Déconnexion : `\q`

### Commandes utiles
- Afficher toutes les tables : `\dt`
- Afficher la structure d'une table : `\d+ <nom_table>`
- Afficher les bases de données : `\l`
- Changer de base de données : `\c <nom_base_de_données>`
- Afficher l'aide : `\?`

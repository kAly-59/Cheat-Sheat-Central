# PostgreSQL Cheat Sheet

## Installation (Ubuntu)

**Mettez à jour vos paquets Ubuntu :**
```bash
sudo apt update
```
**Installez PostgreSQL (et le paquet -contrib qui a quelques utilitaires utiles) avec :**
```bash
sudo apt install postgresql postgresql-contrib
```
**Numéro de version :**
```bash
psql --version
```

## Initialisation
***Chaque fois que vous redémarrez votre machine, vous devrez également redémarrer le service postgres.***

**Démarrez votre service postgres :** 
```bash
sudo service postgresql start
```

**Connexion à PostgreSQL en tant qu'utilisateur superutilisateur (postgres par défaut) :**
```bash 
sudo -u postgres psql
```

**Pour se connectez avec un utilisateur spécifique, à une bdd spécifique**

```bash
psql -U VOTRE_UTILISATEUR -d NOM_DE_LA_BASE_DE_DONNEES
```

**Vous verrez votre ligne de commande changer pour ressembler à ceci :** 
```sql
postgres=#
```



<br>

---

<br>

## Création & suppression & modification base de données

### BDD

**Créer une nouvelle base de données, entrez :**
```sql
CREATE DATABASE nom_de_la_base_de_donnees;
```

**Supprimer une base de données, entrez :**
```sql
DROP DATABASE nom_de_la_base_de_donnees;
```

**Voir bases de données :**
```sql
\l
```

**Importer Fichier SQL :**
```sql
\i <nom_fichier.sql>
```

### Table

***Creation Table (Exemple) :***
```sql
CREATE TABLE mock_data (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    email VARCHAR(50),
    gender VARCHAR(50),
    ip_address VARCHAR(15)
);
```

**Voir vos tables :**
```sql
\d+
```

<br>

---

<br>

## Création & suppression & modification d'utilisateur

**Créer un nouvel utilisateur, `CREATE USER` :**
```sql
CREATE USER nom_utilisateur WITH PASSWORD 'mot_de_passe';
```

**Supprimer un utilisateur, `DROP USER` :**
```sql
DROP USER nom_utilisateur;
```

**Accordez le statut de superutilisateur à un rôle :**
```sql
ALTER ROLE <utilisateur> WITH SUPERUSER;
```

**L'utilisateur admin par défaut, postgres, a besoin d'un mot de passe assigné pour se connecter à une base de données. Pour définir un mot de passe :** 
```sql
\password postgres
```

**Voir les utilisateurs :**
```sql
\du
```

<br>

---

<br>

## Type de données SQL

### Types Numériques :

- **`INT`** : Type de données pour les nombres entiers, représentant des valeurs entières dans une plage spécifique. En général, il utilise 4 octets de stockage.
- **`NUMERIC`** : Utilisé pour stocker des nombres décimaux ou à virgule flottante avec une précision arbitraire. Ce type est idéal pour des calculs précis impliquant des décimales.
- **`SERIAL`** : Un type spécial dans PostgreSQL qui est généralement utilisé pour créer des colonnes d'identité auto-incrémentées. En interne, il crée une séquence associée à la colonne.

### Types Chaînes de Caractères :

- **`CHAR`** : Utilisé pour stocker des chaînes de longueur fixe. Il remplit les espaces vides à droite si la chaîne est plus courte que la longueur spécifiée.
- **`VARCHAR`** : Type de données pour les chaînes de longueur variable. Il stocke les données de manière plus efficiente que `CHAR` en utilisant uniquement l'espace nécessaire pour la chaîne.
- **`TEXT`** : Utilisé pour stocker de grandes quantités de texte. Il n'a pas de limite de longueur spécifique (ou a une limite très élevée) et est souvent utilisé pour des contenus textuels volumineux.

### Types Dates :

- **`TIME`** : Stocke des informations sur l'heure du jour, sans tenir compte de la date. Il peut inclure des heures, minutes, secondes et fractions de seconde.
- **`DATE`** : Utilisé pour stocker des dates, sans tenir compte de l'heure. Stocke l'année, le mois et le jour.
- **`TIMESTAMP`** : Permet de stocker à la fois la date et l'heure précise.

### Autres :

- **`BOOLEAN`** : Utilisé pour stocker des valeurs booléennes (`true` ou `false`). Il représente la logique binaire et est souvent utilisé pour les expressions conditionnelles.

<br>

---

<br>

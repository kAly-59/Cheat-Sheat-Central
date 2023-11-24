# PG CLI Cheat Sheet

## Installation

**Assurez-vous que `pip` est installé :**
```bash
sudo apt update
sudo apt install python3-pip
```

**Installation `pgcli` :**
```bash
sudo pip3 install pgcli
```

**Connexion `pgcli` :**
```bash
pgcli -h <hôte> -U <utilisateur> -d <base_de_données>
```

**Version :**
```bash
pgcli --version
```

<br>

***

<br>

## Création d'une base de données :

**Création & Suppression base de données :**

```sql
CREATE DATABASE <nom_de_la_base_de_données>;
```
```sql
DROP DATABASE <nom_de_la_base_de_données>;
```

**Creation Table (Exemple) :**
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

**Importer Fichier SQL :**
```sql
\i <nom_fichier.sql>
```

<br>

***

<br>

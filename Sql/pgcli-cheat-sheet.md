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

**Version :**
```bash
pgcli --version
```

## Initialisation

**Connexion `pgcli` :**
```bash
pgcli -h <hôte> -U <utilisateur> -d <base_de_données>
```

## Exportation & Importation

**Exportation**
***CLI***
```sql
\! pg_dump -U nom_utilisateur -d nom_base_de_données > backup.sql
```
***SQL***
```bash
pg_dump -U nom_utilisateur -d nom_base_de_données > backup.sql
```

**Importation**
***CLI***
```sql
\! pg_restore -U nom_utilisateur -d nom_base_de_données < backup.sql
```

***SQL***
```bash
psql -U kaly -d au_bon_deal < backup.sql
```

## Extension

**uuid-ossp**
```sql
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
```
**Vérifiez la disponibilité de la fonction uuid_generate_v4()**
```sql
SELECT uuid_generate_v4();
```

<br>

***

<br>

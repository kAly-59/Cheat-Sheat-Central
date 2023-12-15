# PM2

## Installation

### Installer PM2
```bash
$ sudo npm install pm2@latest -g
```

### Build le projet
```bash
$ npm run build
```

### Exécuter le projet
```bash
$ pm2 start dist/main.js --name <nom_de_l'application>
```
## Commandes

### Contrôle PM2 :

- **Redémarrer une application**
  ```bash
  $ pm2 restart app_name
  ```

- **Recharger une application**
  ```bash
  $ pm2 reload app_name
  ```

- **Arrêter une application**
  ```bash
  $ pm2 stop app_name
  ```

- **Supprimer une application de PM2**
  ```bash
  $ pm2 delete app_name
  ```

### Gestion des journaux et surveillance

- **Afficher les serveurs lancer**
  ```bash
  $ pm2 list
  ```

- **Afficher les journaux d'une application**
  ```bash
  $ pm2 logs
  ```

- **Surveiller les applications actives**
  ```bash
  $ pm2 monit
  ```

### Mises à jour :

- **Mettre à jour PM2**
  ```bash
  $ pm2 update
  ```
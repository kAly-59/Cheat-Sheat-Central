## Node.js Installation (Version LTS 20.10.0)

### Utilisation de Node Version Manager (NVM)
- Installation de Node Version Manager (NVM) :
  ```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
  ```
- Rafraîchir le shell pour appliquer les modifications :
  ```bash
  source ~/.bashrc
  ```
- Installer Node.js version LTS 20.10.0 avec NVM :
  ```bash
  nvm install 20.10.0
  ```
- Utiliser Node.js version LTS 20.10.0 :
  ```bash
  nvm use 20.10.0
  ```
- Définir Node.js version LTS 20.10.0 par défaut :
  ```bash
  nvm alias default 20.10.0
  ```
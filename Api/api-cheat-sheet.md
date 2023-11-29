# API

## Requêtes HTTP (GET, POST, PUT, DELETE)

### GET 
- **Objectif** : Récupère des données à partir d'une ressource spécifiée.
- **Utilisation** : Utilisé pour obtenir des données sans modifier la ressource.
- **Transmission de données** : Les données sont envoyées via les paramètres d'URL.
- **Sécurité** : Les données sont visibles dans l'URL, moins sécurisé pour les informations sensibles.
- **Caching** : Peut être mis en cache et mis en signet.
- **Exemple d'utilisation** :
  ```
  GET /api/utilisateurs?id=123
  ```

### POST 
- **Objectif** : Soumet des données à une ressource spécifiée pour traitement.
- **Utilisation** : Souvent utilisé pour créer de nouvelles ressources.
- **Transmission de données** : Les données sont envoyées dans le corps de la requête et ne sont pas visibles dans l'URL.
- **Sécurité** : Plus sécurisé car les données ne sont pas exposées dans l'URL.
- **Caching** : Généralement non mis en cache et non mis en signet.
- **Exemple** :
  ```
  POST /api/utilisateurs
  {
    "nom": "Alice",
    "email": "alice@example.com"
  }
  ```

### PUT 
- **Objectif** : Met à jour une ressource spécifiée avec les données fournies.
- **Utilisation** : Utilisé pour modifier une ressource existante ou créer si elle n'existe pas.
- **Transmission de données** : Les données sont envoyées dans le corps de la requête.
- **Sécurité** : Les données ne sont pas exposées dans l'URL, similaire à POST.
- **Caching** : Généralement non mis en cache et non mis en signet.
- **Exemple** :
  ```
  PUT /api/utilisateurs/123
  {
    "nom": "Bob",
    "email": "bob@example.com"
  }
  ```

### DELETE 
- **Objectif** : Supprime la ressource spécifiée.
- **Utilisation** : Utilisé pour supprimer des données sur le serveur.
- **Transmission de données** : Peut parfois nécessiter l'identification de la ressource dans l'URL, mais n'envoie généralement pas de données dans le corps de la requête.
- **Sécurité** : Les informations peuvent être exposées dans l'URL, par conséquent, les identifiants de ressources sensibles peuvent être visibles.
- **Caching** : Ne devrait normalement pas être mis en cache.
- **Exemple** :
  ```
  DELETE /api/utilisateurs/123
  ```

### PATCH 
- **Objectif** : Applique des modifications partielles à une ressource existante.
- **Utilisation** : Utilisé pour mettre à jour spécifiquement certains champs d'une ressource sans remplacer la ressource complète.
- **Transmission de données** : Les données sont envoyées dans le corps de la requête pour indiquer les modifications à apporter.
- **Sécurité** : Les données ne sont pas exposées dans l'URL, similaire à POST et PUT.
- **Caching** : Généralement non mis en cache et non mis en signet.
- **Exemple** :
  ```
  PATCH /api/utilisateurs/123
  {
    "email": "nouveauemail@example.com"
  }
  ```

### Comparaison 

| Méthode HTTP | Objectif                 | Utilisation                  | Sécurité               | Transmission de données | Caching            |
|--------------|--------------------------|------------------------------|------------------------|-------------------------|--------------------|
| GET          | Récupération de données  | Récupérer des données        | Moins sécurisé (visible)| Via les paramètres d'URL | Peut être mis en cache |
| POST         | Soumission de données     | Créer de nouvelles données  | Plus sécurisé (non visible) | Dans le corps de la requête | Non mis en cache  |
| PUT          | Mise à jour de données   | Modifier ou créer des données| Plus sécurisé (non visible) | Dans le corps de la requête | Non mis en cache  |
| DELETE       | Suppression de données   | Supprimer des données        | Moins sécurisé (visible) | Peut nécessiter l'URL | Non mis en cache  |
| PATCH        | Modifications partielles  | Modifier spécifiquement     | Plus sécurisé (non visible) | Dans le corps de la requête | Non mis en cache  |

---

## Codes de Statut HTTP

| Catégorie  | Description                                  | Exemples de Codes de Statut                 |
|------------|----------------------------------------------|---------------------------------------------|
| 2xx (Success) | Indique que la requête a été traitée avec succès. | 200 (OK), 201 (Created), 204 (No Content) |
| 3xx (Redirection) | Indique que d'autres actions doivent être prises pour compléter la requête. | 301 (Moved Permanently), 302 (Found), 304 (Not Modified) |
| 4xx (Client Error) | Indique une erreur attribuable à la requête du client. | 400 (Bad Request), 404 (Not Found), 403 (Forbidden) |
| 5xx (Server Error) | Indique une erreur du côté du serveur lors du traitement de la requête. | 500 (Internal Server Error), 503 (Service Unavailable), 502 (Bad Gateway) |




  

# AFK News Frontend

Fichiers : `index.html`, `style.css`, `app.js`.

L'URL du backend se trouve au début de `app.js` :
`const API_BASE = "https://afk-news-backend.onrender.com";`

## Déploiement Render
1. Crée un dépôt GitHub et ajoute les trois fichiers à sa racine.
2. Sur Render : **New + → Static Site**.
3. Connecte le dépôt GitHub.
4. Build Command : laisse vide.
5. Publish Directory : `.`
6. Clique sur Deploy.

Le frontend utilise `GET /api/articles?page=1&limit=12` et la structure JSON confirmée. La météo utilise l'API publique Open-Meteo sans clé. Si le navigateur affiche une erreur CORS, il faudra autoriser le domaine du frontend dans la configuration CORS du backend.

# 🌦️ Weather API

**Weather API** est une application qui permet de faire des requêtes basiques pour obtenir des informations météorologiques basées sur la localisation.

## Fonctionnalités

- **Obtenir les Conditions Météorologiques Actuelles** : Faites une requête pour obtenir les conditions météorologiques actuelles pour une localisation donnée.
- **Gérer les Erreurs** : Traitez et renvoyez des erreurs personnalisées pour les requêtes incorrectes ou les problèmes de serveur.

## Installation

1. **Cloner le Dépôt** :

   ```bash
   git clone <url-du-dépôt>
   cd weather-api
   ```

2. **Installer les Dépendances** :

   ```bash
   npm install
   ```

3. **Configurer les Variables d'Environnement** :

   Créez un fichier `.env` dans le répertoire racine et ajoutez les variables d'environnement nécessaires, par exemple :

   ```plaintext
   WEATHER_API_KEY=<votre_clé_api_météo>
   PORT=3000
   ```

4. **Compiler le Projet** :

   ```bash
   npx tsc
   ```

5. **Démarrer le Serveur** :

   ```bash
   npm start
   ```

## Utilisation

### Obtenir les Conditions Météorologiques Actuelles

1. Faites une requête `GET` à l'endpoint `/weather` avec un paramètre de localisation. Par exemple :

   ```bash
   curl "http://localhost:3000/weather?location=Paris"
   ```

2. Le serveur renverra les informations météorologiques actuelles pour la localisation spécifiée.

## Structure du Projet

```plaintext
weather-api/
│
├── constantes/
│   ├── config.ts
│   ├── errorCodes.ts
│   └── errorMessages.ts
│
├── controller/
│   └── WeatherController.ts
│
├── errors/
│   ├── ApiError.ts
│   └── CustomError.ts
│
├── middleware/
│   └── errorHandler.ts
│
├── node_modules/
│
├── .env
├── README.md
├── package.json
└── tsconfig.json
```

## Technologies Utilisées

- **Node.js** : Runtime JavaScript pour l'exécution côté serveur.
- **TypeScript** : Pour le typage statique.
- **Express** : Framework web pour Node.js pour créer le serveur et les endpoints API.

---

Voilà **Weather API** ! Si vous avez des questions ou des suggestions, n'hésitez pas à les partager. 🌦️✨

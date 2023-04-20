# Étape 1 : Utiliser une image Node.js pour construire l'application
FROM node:14-alpine 

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./

# Installer les dépendances de l'application
RUN npm ci

# Copier le reste des fichiers de l'application dans le conteneur
COPY . .

# Construire l'application Angular en mode de production
CMD ["npm", "run", "prod"]

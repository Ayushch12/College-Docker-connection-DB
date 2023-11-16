# Utilisez une image Node.js officielle comme base
FROM node:14

# Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./

# Installez les dépendances
RUN npm install

# Copiez le code de l'application dans le conteneur
COPY . .

# Exposez le port 80 vers le monde extérieur
EXPOSE 80

# Définissez la commande pour exécuter votre application
CMD ["npm", "start"]

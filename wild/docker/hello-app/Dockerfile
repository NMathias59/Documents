# Utilisez une image de Node.js comme base
FROM node:lts-alpine

# Créez un répertoire de travail dans l'image
WORKDIR /hello-app

# Copiez les fichiers package.json et package-lock.json dans l'image
COPY package.json package-lock.json ./

# Installez les dépendances de l'application
RUN npm install

# Copiez le reste de l'application dans l'image
COPY . .

# Exposez le port sur lequel l'application s'exécute (si nécessaire)
EXPOSE 3000

# Commande pour exécuter l'application
CMD ["node", "index.js"]

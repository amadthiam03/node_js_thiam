# Utilize l'image officielle Node.js 

FROM node:14 

# Définit le répertoire de travail dans le conteneur 

WORKDIR /app 

# Copier les fichiers package.json et package-lock.json 

COPY package*.json ./ 

# Installer les dépendances du projet 

RUN npm install 

# Copier le reste des fichiers du projet 

COPY . . 

# Expose le port sur lequel l'application s'exécute 

EXPOSE 8080 

# Démarre l'application 

CMD [ "npm", "start" ]

FROM node:14.16.1-alpine3.13

WORKDIR /app

# copia os arquivos package para o diretório /app da imagem
COPY package*.json ./ 
#npm config set strict-ssl false
RUN npm install
COPY . . 

#expoe a porta do container
EXPOSE 8080

#Comando que será executado ao final ao inicializar o container
CMD ["node", "index.js"]
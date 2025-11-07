# frontend/Dockerfile (Modo Desenvolvimento)

FROM node:20-alpine

WORKDIR /app

# Instala as dependências primeiro para cache
COPY package.json package-lock.json ./
RUN npm install

# Copia o restante do código
COPY . .

# Expor a porta padrão do Angular
EXPOSE 4200

# Comando para rodar o servidor de desenvolvimento
CMD ["npm", "run", "start"] # Presume que 'start' no package.json roda 'ng serve'
FROM node
WORKDIR /app
# copiando as definições de dependências separadamente, fazem com que o container crie um cache e só atualize caso
# as definições tenham sido alteradas
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD [ "node", "server.js" ]
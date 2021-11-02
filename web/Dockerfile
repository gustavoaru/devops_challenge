FROM node:14-alpine3.14

# Diretorio da aplicacao
WORKDIR /usr/src/app

# Copiar as dependecias da aplicacao
# Caso depois altere apenas os arquivos da aplicacao sem suas
# dependencias serah aproveitado o cache do Docker
COPY package*.json ./

# Construindo as dependencias
RUN npm install

# Copiando os arquivos da aplicacao
# Observacao = Criado o .dockerignore para remover os arquivos desnecessários
COPY . .

# Executar a aplicacao
ENTRYPOINT [ "npm", "start"]

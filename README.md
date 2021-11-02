# DevOps Challenge

- This repo contains code for a multilayer application.

- The application overview is as follows: web <=> api <=> db

- There is an api directory and another web, you should dock the application in the best possible way.

- Write a recipe with the tool of your choice (ansible or terraform) to build the environment and run the application in an automated way.

# Running

- The idea to test locally is to just run 'docker-compose up'
- Access url localhost: 8080


# Evaluation

- It will count the quality of 'Dockerfile', 'docker-compose.yml'
- Extra points if you use terraform and are in good practice
- Extra points if you use ansible and are well structured

# Dock the application

- Ajustado a conexão com o banco de dados
- Criado o Dockerfile para cada aplicação (api, web)
- Criado um docker-compose.yaml para levantar todos os serviços
- Não foi exposta a porta do banco de dados
- Criando o arquivo .env com as variáveis da aplicação:

```
# DATABASE POSTGRES
POSTGRES_VERSION=14-alpine
POSTGRES_DB=db_name
POSTGRES_USER=db_user
POSTGRES_PASSWORD=db_password
POSTGRES_PORT=5432

# PORTA API
API_PORT=8081

# PORTA WEB
WEB_PORT=8080
```
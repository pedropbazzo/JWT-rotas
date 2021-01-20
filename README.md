# Autenticação JWT

## Descrição
Autenticação JWT e controle de segurança nas rotas

Rota: Express

ODM: Mongoose

Autenticação: JWT


#### Instalar pacotes mongo
`npm install`


##### docker:

baixe a imagem mongo:

`docker pull mongo`

Inicie um container:

`docker run --name mongodocker -p 27017:27017 -d mongo`

##### iniciar o projeto

`npm start`

## Testando
Use [postman](https://www.getpostman.com/apps) para realizar as chamadas a API

#### Criar usuário 
Método POST na rota /api/v1/usuarios/ sem verificação de token
passando os parâmetros: nome, login, senha e email no corpo da requisição

inserir usuários

#### Logando
Método POST na rota /api/v1/login/
passando os parâmetros: login e senha no corpo da requisição


#### Acessando rota com JWT
Método GET na rota /api/v1/usuarios com verificação de token
Informe token no cabeçalho da requisição com a chave: 'x-access-token' e valor informar o token recebido no login

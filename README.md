
 ▄▄▄       ██▓███   ██▓▒██   ██▒   ©2018
▒████▄    ▓██░  ██▒▓██▒▒▒ █ █ ▒░   
▒██  ▀█▄  ▓██░ ██▓▒▒██▒░░  █   ░   
░██▄▄▄▄██ ▒██▄█▓▒ ▒░██░ ░ █ █ ▒    
 ▓█   ▓██▒▒██▒ ░  ░░██░▒██▒ ▒██▒   
 ▒▒   ▓▒█░▒▓▒░ ░  ░░▓  ▒▒ ░ ░▓ ░   
  ▒   ▒▒ ░░▒ ░      ▒ ░░░   ░▒ ░   
  ░   ▒   ░░        ▒ ░ ░    ░     
      ░  ░          ░   ░    ░     

PWA APIX 2018 App

Manager: https://manager-apix.sensedia.com/api-manager/
Massa de dados: https://next.json-generator.com/Eyd8QJgpg

Install NVM:
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash

Install node:
nvm install stable

Inicializando um projeto (na pasta que você definiu):
npm init -y

Instalando o json-server:
npm install json-server --save

Criando arquivo da massa de dados:
vi db.json
{
 "cards" : []
}

Editando package.json
vi package.json

Substituir:

{
  "name": "be",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}

Por:
{
  "name": "be",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "start": "json-server --watch db.json"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "dependencies": {
    "json-server": "^0.14.0"
  }
}

Editar db.json e adicionar a massa de dados dentro do array.


Rodar aplicação:
npm start
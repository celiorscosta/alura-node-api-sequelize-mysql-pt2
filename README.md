# ORM com NodeJS: Avançando com Sequelize e MySQL

Continuação do curso anterior [ORM com NodeJS: API com Sequelize e MySQL](https://github.com/celiorscosta/alura-node-api-sequelize-mysql), onde implementaremos as rotinas trabalhar com BDs de forma extremamente produtiva utilizando mapeamento objeto-relacional (ou ORM, do inglês: Object-relational mapping) com o Sequelize ORM.

> Esta é a segunda parte do curso.

### EXTRAS
**Docker**

>Também criei todo o ambiente rodando no docker como forma de colocar em pratica o que tenho aprendido em meus estudos.

## Project setup

> Instale os pacotes usando o comando abaixo:
```
npm install
```
Feito isso a pasta ``node_modules`` devera ter sido criada.

### Docker Compose

> O ambiente foi todo criado utilizando o docker para montar a infraestrutura. Basta rodar o comando a seguir e toda a infraestrutura sera montada no docker e o sistema devera iniciar.

```
docker-compose up
```

### Migrate

> Altere o campo "host" no arquivo "config.json" dentro da pasta "src/config" de "mysqldb2" para "localhost", salve e execute os comandos a seguir para criar a tabela e preencher com alguns dados iniciais:

> Rode os comandos a seguir no terminal:

```
npx sequelize-cli db:migrate
```
```
npx sequelize-cli db:seed:all
```

> Após isso, volte o campo "host" no arquivo "config.json" para "mysqldb2" e salve o arquivo.

Pronto. Fazendo isso, é para funcionar.

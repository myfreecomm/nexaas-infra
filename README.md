# Nexaas Infra

O Nexaas Infra é um projeto criado com o objetivo de centralizar os containers responsáveis por receber e enviar dados, que necessitam transitar entre os microserviços da Nexaas.

Inicialmente será utilizado para conectar os serviços de messageria com Apache Kafka. A princípio o projeto funcionará a partir de um arquivo env.sample e docker-compose para subir os containers no ambiente de desenvolvimento.

Dependências:
* Linux / Mac OSX

* [Docker](https://www.docker.com/)

* [Docker Compose](https://docs.docker.com/compose/)

* [Docker Desktop](https://www.docker.com/products/docker-desktop/)

## Setup do projeto com Docker
Antes de subir o projeto, as variáveis de ambiente precisam estar presentes no projeto:

Abra o terminal, navegue para a raiz do projeto e crie os arquivos com base nos arquivos de exemplo:
```
cp .env.sample .env
```

Para subir os containers executando em background, execute o comando:
```
docker compose up -d
```

Ao subir os containers com sucesso, os containers do Kafka os demais serviços estarão disponíveis.

# Dart for backend - ROADMAP 2022

Roadmap dedicado aos devs que desejam iniciar com o Dart no backend.
Esse documento irá abordar as principais técnicas e assuntos a serem estudados pata
criar um backend saudável, manutenível e escalável.

# Linguagens

Iremos usar o Dart como linguagem principal, então é necessário um conhecimento intermediário sobre
as principais features da linguagem. Além disso, precisamos entender algumas outras linguagens de 
marcação para executar ferramentas essenciais para o trabalho.

## Dart

O SDK Do Dart vem junto com o Flutter, por tanto, se já estiver com o toolkit instalado, experimente digitar em um console:
```
dart --version
```

## SQL

Para base de dados como MySQL e Postgres.

- [O que é SQL?](https://www.youtube.com/watch?v=kMznyI7r2Tc)
- [Curso completo de SQL](https://www.youtube.com/watch?v=rX2I7OjLqWE)



## YAML

A mesma linguagem de marcação utilizada no pubspec.yaml do Dart/Flutter também ajuda a configurar outros serviços como docker-compose, CI/CD como Github Actions dentre outros.

- [Descomplicando o YAML](https://www.youtube.com/watch?v=JOtIVGy1SgE)

## JSON

Provavelmente a linguagem de marcação mais popular nos dias atuais. Javascript Object Notation é utilizado para transporte de informações entre cliente e servidor. *Obrigatório.

- [O que é JSON?](https://www.youtube.com/watch?v=P81dE-tkaaA)
- [Aprenda JSON](https://www.youtube.com/watch?v=BWPUSXzSWA8)


# Docker

É extremamente necessário trabalhar com containers nos dias atuais tanto para publicação de uma aplicação quanto para iniciar um ambiente de desenvolvimento, pois basta levantar um container de um postgres ou mysql para ter esse banco rodando na sua máquina com apenas um comando.

Dito isso, sua vida profissional no backend dependerá bastante do conhecimento sobre docker.

- [O que é um container?](https://www.youtube.com/watch?v=-pUZBovqRcU)
- [Getting Starting (Oficial)](https://docs.docker.com/get-started/)
- [Docker, Docker-compose](https://www.youtube.com/watch?v=yb2udL9GG2U)

# Protocolo HTTP

Como que é feita a comunicação de um computador(server) com outro(client)? A resposta está nos Sockets.
A transmissão de dados via socket é muito comum na internet, ou melhor, ESSA É A INTERNET.
Porém, enviar apenas dados de computador para computador apenas com sockets se mostra uma tarefa complexa no sentido de organização, o que nos leva ao protocolo HTTP, que simplesmente padroniza as requisições(Request) e respostas(Response) para que qualquer um possa criar servidores e clientes compartilhando essa tecnologia de forma fácil. Por exemplo, sem o protocolo http, todo site deveria criar seu próprio navegador, oque inviabilizaria a web. 

- [O que é HTTP](https://www.youtube.com/watch?v=hwttZtWkXTk)
- [Conceitos essenciais](https://www.youtube.com/watch?v=hwttZtWkXTk)
- [Overview](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Overview)

# API

Iremos construir uma API em Dart, então é importante entender o que é API.

- [O que é API?](https://www.youtube.com/watch?v=vGuqKIRWosk)
- [API na prática](https://www.youtube.com/watch?v=3LHSyha0xN0)
- [Tirando dúvidas sobre API Rest/Restful](https://www.youtube.com/watch?v=P92SBaN42mQ)
- [API Restful ilustrada](https://www.youtube.com/watch?v=Abo_GiaunlU)
- [API Rest e Restful](https://www.youtube.com/watch?v=ghTrp1x_1As)



# Shelf

Toda ferramenta contém um framework dedicado para construir uma API Web, no caso do Dart nós temos o **Shelf**.

Framework baseado em Middleware muito semelhante ao Express.js.
Essa ferramenta é totalmente escalável por outros packages, ou seja, uma nova funcionalidade pode ser adicionada ao Shelf como um plugin.

O Shelf sozinho apenas "escuta" as conexões, precisaremos de outros packages para a construção de nossa api.

## Rotas

Existem 2 packages principais que trabalham com rotas.

- [shelf_modular (Flutterando)](https://modular.flutterando.com.br/docs/shelf_modular/start/).

Mesma estrutura do flutter_modular para rotas e injeção de dependências para o Shelf.


- [shelf_router (Google)](https://modular.flutterando.com.br/docs/shelf_modular/start/).


Sistema de rotas simples mais eficiência extremamente semelhante ao sistema de rotas do Express.js.

## Documentação de API

- [shelf_swagger_ui (Flutterando)](https://pub.dev/packages/shelf_swagger_ui)

## Injeção de dependências


- [shelf_modular (Flutterando)](https://modular.flutterando.com.br/docs/shelf_modular/start/).
- [get_it](https://pub.dev/packages/get_it).


## Json Web Token (JWT)

- [jose](https://pub.dev/packages/jose)
- [dart_jsonwebtoken](https://pub.dev/packages/dart_jsonwebtoken)


## Websocket

- [shelf_web_socket](https://pub.dev/packages/shelf_web_socket)


## Base de dados

- [postgres](https://pub.dev/packages/postgres)
- [mysql_client](https://pub.dev/packages/mysql_client)
- [mongo_dart](https://pub.dev/packages/mongo_dart)


Muitas coisas ainda estão por vir!
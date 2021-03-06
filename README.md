# Node.js - Desafio 1

[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/osvaldokalvaitir/nodejs-desafio1/blob/master/LICENSE)
![](https://img.shields.io/github/package-json/v/osvaldokalvaitir/nodejs-desafio1.svg)
![](https://img.shields.io/github/last-commit/osvaldokalvaitir/nodejs-desafio1.svg?color=red)
![](https://img.shields.io/github/languages/top/osvaldokalvaitir/nodejs-desafio1.svg?color=yellow)
![](https://img.shields.io/github/languages/count/osvaldokalvaitir/nodejs-desafio1.svg?color=lightgrey)
![](https://img.shields.io/github/languages/code-size/osvaldokalvaitir/nodejs-desafio1.svg)
![](https://img.shields.io/github/repo-size/osvaldokalvaitir/nodejs-desafio1.svg?color=blueviolet)
[![made-for-VSCode](https://img.shields.io/badge/Made%20for-VSCode-1f425f.svg)](https://code.visualstudio.com/)
![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)

Aplicação usando Node.js, Express, Nunjucks, EditorConfig e ESLint.

## Desafio

Nesse desafio vamos construir uma aplicação que aceita a entrada de um campo do usuário por um formulário e o redireciona para a página correta baseado em sua idade.

Configure uma aplicação utilizando **ExpressJS, Nunjucks, EditorConfig e ESLint**.

### Rotas (Desafio)

- `/`: Rota inicial que renderiza uma página com um formulário com um único campo `age` que representa a idade do usuário;
- `/check`: Rota chamada pelo formulário da página inicial via método POST que checa se a idade do usuário é maior que 18 e o redireciona para a rota `/major`, caso contrário o redireciona para a rota `/minor` (Lembre de enviar a idade como Query Param no redirecionamento);
- `/major`: Rota que renderiza uma página com o texto: `Você é maior de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;
- `/minor`: Rota que renderiza uma página com o texto: `Você é menor de idade e possui x anos`, onde `x` deve ser o valor informado no input do formulário;

### Middlewares

Deve haver um middleware que é chamado nas rotas `/major` e `/minor` e checa se a informação de idade não está presente nos Query Params. Se essa informação não existir deve redirecionar o usuário para a página inicial com o formulário, caso contrário o middleware deve apenas continuar com o fluxo normal.

## Índice

- [Capturas de Tela](#capturas-de-tela)

  - [Principal](#main)

  - [Maior](#major)

  - [Minor](#minor)

- [Desenvolvimento](#desenvolvimento)

  - [Configuração do Ambiente](#configuração-do-ambiente)

  - [Instalação do Projeto](#instalação-do-projeto)

  - [Execução do Projeto](#execução-do-projeto)

- [Utilizados no Projeto](#utilizados-no-projeto)

  - [Bibliotecas](#bibliotecas)

## Capturas de Tela

### Principal

![Main](/.github/assets/main.png)
Esta é a tela principal onde o usuário informa a idade para a checagem.

### Maior

![Major](/.github/assets/major.png)
Esta tela aparecerá se a idade informada for maior que 18 anos.

### Menor

![Minor](/.github/assets/minor.png)
Esta tela aparecerá se a idade informada for menor ou igual à 18 anos.

## Desenvolvimento

### Configuração do Ambiente

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/README.md) e siga `Configuração de Ambiente`.

### Instalação do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Instalação de Projeto`.

### Execução do Projeto

Clique [aqui](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/nodejs.md) e siga `Execução de Projeto para Desenvolvimento` ou `Execução de Projeto para Produção`.

## Utilizados no Projeto

### Bibliotecas

- [ESLint](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/eslint.md)

- [Express](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/express.md)

- [Nodemon](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nodemon.md)

- [Nunjucks](https://github.com/osvaldokalvaitir/projects-settings/blob/master/nodejs/libs/nunjucks.md)

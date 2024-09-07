**Projeto de Servidor em Node.js**
=====================================

**Descrição**
---------------

Este é um projeto de servidor em Node.js que utiliza o módulo `http` para criar um servidor que escuta requisições HTTP. O servidor é configurado para lidar com requisições POST para as rotas `/user` e `/login`.

**Funcionalidades**
-------------------

*   Criação de usuários: o servidor permite a criação de novos usuários enviando uma requisição POST para a rota `/user` com os dados do usuário no corpo da requisição.
*   Login de usuários: o servidor permite o login de usuários enviando uma requisição POST para a rota `/login` com os dados de login no corpo da requisição.

**Requisitos**
--------------

*   Node.js (versão 14 ou superior)
*   Módulo `http` (incluído no Node.js)
*   Módulo `fs` (incluído no Node.js)
*   Módulo `formidable` (instalado via npm)

**Instalação**
--------------

1.  Clone o repositório
2.  Instale as dependências: `npm install`
3.  Inicie o servidor: `node server.js`

**Uso**
-----

*   Para criar um novo usuário, envie uma requisição POST para a rota `/user` com os dados do usuário no corpo da requisição. Exemplo:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"nome": "João", "email": "joao@example.com", "senha": "123456"}' http://localhost:3333/user
```

*   Para fazer login, envie uma requisição POST para a rota `/login` com os dados de login no corpo da requisição. Exemplo:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"email": "joao@example.com", "senha": "123456"}' http://localhost:3333/login
```

**Licença**
------------

Este projeto é licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
# Bootcamp - GoStack

**Iniciando aplicação - Meetapp**

### Rotas

`POST /sessions`

- Autenticação de usuários utilizando JWT;

  Exemplo:

  `{ "email": "email@dominio.com.br", "password": "123456" }`

`POST /users`

- Adiciona novos usuários com validação dos dados de entrada;
- Criptografa a senha do usuário para segurança.

  Exemplo:

  `{ "name": "Nome do usuário", "email": "email@dominio.com.br", "password": "123456" }`

`PUT /users`

- Edita as informações do usuário;

  Exemplo de alteração de usuário sem senha:

  `{ "name": "Nome do usuário", "email": "email@dominio.com.br", "password": "123456" }`

  Exemplo de alteração de usuário com senha:

  `{ "name": "Nome do usuário", "email": "email@dominio.com.br", "oldPassword": "123456", "password": "12345678", "confirmPassword": "12345678" }`

No arquivo `src/config/database.js` encontra-se as configurações de acesso ao postgres, alterar conforme suas informações.

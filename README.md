# 📌NoteHub API
![NoteHub Logo](./assets/img/notehub-logo.png)

## Introdução
**Desafio Proposto:** A startup "NoteHub" está desenvolvendo um aplicativo simples de anotações digitais para estudantes. O aplicativo precisa de uma API backend para armazenar e gerenciar as anotações dos usuários. Como o projeto está em fase inicial, a versão 1.0 trabalhará apenas com anotações, sem sistema de usuários ou categorias complexas.

## API Endpoints
| Método HTTP | Endpoint         | Descrição                          |
|-------------|------------------|------------------------------------|
| GET         | /notas           | Retorna todas as anotações        |
| GET         | /notas/{id}      | Retorna uma anotação específica   |
| POST        | /notas           | Cria uma nova anotação            |
| PUT         | /notas/{id}      | Atualiza uma anotação existente   |
| DELETE      | /notas/{id}      | Remove uma anotação específica    |

## Tecnologias Utilizadas
[<img src="https://nodejs.org/static/images/logo.svg" alt="Node.js Logo" width="60px">](https://nodejs.org/) | [<img src="https://cdn.worldvectorlogo.com/logos/express-109.svg" alt="Express Logo" width="50px">](https://expressjs.com/) | [<img src="https://www.prisma.io/images/favicon-32x32.png" alt="Prisma Logo" width="30px">](https://www.prisma.io/)  |  [<img src="https://upload.wikimedia.org/wikipedia/commons/3/38/SQLite370.svg" alt="SQLite Logo" width="50px">](https://www.sqlite.org/)

## Como Executar
1. Instale as dependências do projeto:

```bash
npm install
```

2. Crie o arquivo `.env` com a variável `DATABASE_URL` apontando para o banco de dados desejado.

```
DATABASE_URL="file:./dev.db"
```

3. Execute as migrações:

```bash
npx prisma migrate dev
```

4. Inicie o servidor:

```bash
npm run dev
```

## Licença
Este projeto está licenciado sob a Licença MIT - consulte o arquivo [LICENSE](./LICENSE) para obter detalhes.
```
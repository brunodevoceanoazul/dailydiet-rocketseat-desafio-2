# Daily Diet · React and Fastify

Personal full-stack implementation of a Rocketseat training challenge. The app records meals and calculates metrics, including the longest streak of meals marked as on-diet.

**Stack** · TypeScript, React, Vite, Node.js, Fastify, Zod, Knex and SQLite.

| Start here | What it demonstrates |
| --- | --- |
| [Meals API](src/routes/meals.ts) | Request validation, CRUD, per-session record scoping and metrics. |
| [Database migrations](db/migrations/) | SQLite data model managed through Knex migrations. |
| [React screens](web/src/pages/) | Meal list, forms, details and metrics wired to the API. |

**Original contributions** · [API implementation](https://github.com/BrunoBDevOceanoAzul/dailydiet-rocketseat-desafio-2/commit/ea4b7fe18b4f555406a4e3d3279d1440b491120a) · [React frontend](https://github.com/BrunoBDevOceanoAzul/dailydiet-rocketseat-desafio-2/commit/d32397a1dd8fd536fdb499a1a1877f99b9aa9997).

## Run locally

Use Node.js 22. Start with a fresh local database and fictitious records.

```sh
npm ci
npm --prefix web ci
cp .env.example .env
npm run knex -- migrate:latest
npm run dev
```

The API defaults to port 3333. Open the URL printed by Vite, normally `http://localhost:5173`. To compile both components, use `npm run build` and `npm --prefix web run build`.

## Em português

Exercício pessoal full stack da Rocketseat. Os links acima destacam o código original da API e da interface, a modelagem do banco e a implementação das métricas.

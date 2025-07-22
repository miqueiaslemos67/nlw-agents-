# NLW Agents - Backend (Server)

Este é o projeto **backend** do NLW Agents, desenvolvido durante o evento da **Rocketseat**. Ele utiliza **Fastify**, **TypeScript**, **Drizzle ORM** e **PostgreSQL** para fornecer uma API performática e escalável.

## 🛠 Tecnologias Utilizadas

- **Fastify** - Framework web leve e performático para Node.js.
- **TypeScript** - Superset do JavaScript com tipagem estática.
- **Drizzle ORM** - ORM moderno, focado em SQL type-safe.
- **PostgreSQL** - Banco de dados relacional.
- **Zod** - Validação de esquemas de dados.
- **Dotenv** - Gerenciamento de variáveis de ambiente.
- **Fastify CORS** - Middleware para configuração de CORS.
- **fastify-type-provider-zod** - Integração entre Zod e Fastify.

## 🗂 Estrutura do Projeto

```bash
server
├── src
│   ├── db               # Configuração do Drizzle ORM e seeds
│   ├── env.ts           # Variáveis de ambiente tipadas
│   ├── http
│   │   └── routes       # Rotas da aplicação
│   └── server.ts        # Arquivo principal do servidor
├── .env                 # Arquivo com variáveis de ambiente
├── drizzle.config.ts    # Configuração do Drizzle
└── package.json
```

## ⚙️ Setup e Configuração

### 1. Clone o repositório e acesse a pasta `server`:

```bash
git clone <url-do-repo>
cd server
```

### 2. Instale as dependências:

```bash
npm install
```

### 3. Configure o banco de dados:

Altere o arquivo `.env` com sua URL de conexão PostgreSQL:

```
DATABASE_URL=postgres://user:password@localhost:5432/nlw_agents
PORT=3333
```

### 4. Execute as migrations e seeds:

```bash
npx drizzle-kit push
npm run db:seed
```

### 5. Inicie o servidor:

```bash
npm run dev
```

## 🔗 Endpoints disponíveis

- `GET /rooms` → Lista todas as salas disponíveis.
- `GET /health` → Verifica se o servidor está online.

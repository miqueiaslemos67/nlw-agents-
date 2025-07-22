# NLW Agents - Frontend (Web)

Este é o projeto **frontend** do NLW Agents, desenvolvido com **React**, **TypeScript**, **Tailwind CSS** e **Vite**, durante o evento da Rocketseat.

## 🧪 Tecnologias Utilizadas

- **React 18+** - Biblioteca JavaScript para construção de interfaces.
- **TypeScript** - Superset do JavaScript com tipagem.
- **Vite** - Bundler moderno e rápido.
- **React Router DOM** - Roteamento de páginas SPA.
- **Tailwind CSS** - Framework de utilitários CSS.
- **Phosphor Icons** - Ícones SVG otimizados.
- **Zod + React Hook Form** - Validação e controle de formulários.

## 🗂 Estrutura do Projeto

```bash
web
├── src
│   ├── components       # Componentes reutilizáveis
│   ├── pages            # Páginas da aplicação
│   ├── lib              # Utils, serviços, API etc.
│   ├── main.tsx         # Entrada da aplicação
│   └── vite-env.d.ts
├── index.html
├── tailwind.config.js
├── vite.config.ts
└── package.json
```

## ⚙️ Setup e Configuração

### 1. Clone o repositório e acesse a pasta `web`:

```bash
git clone <url-do-repo>
cd web
```

### 2. Instale as dependências:

```bash
npm install
```

### 3. Inicie o servidor de desenvolvimento:

```bash
npm run dev
```

### 4. Acesse no navegador:

```
http://localhost:5173
```

> Certifique-se que o backend (`server`) esteja rodando em `http://localhost:3333` com CORS liberado.

## 📋 Funcionalidades

- Listagem de salas.
- Navegação SPA.
- Comunicação com API via `fetch` utilizando `react-query`.

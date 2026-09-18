# Svelte / SvelteKit

Breve descrição
----------------
Este projeto usa SvelteKit — um framework moderno para construir aplicações web reativas com componentes Svelte. Fornece roteamento, renderização no servidor (opcional), e integração com Vite para desenvolvimento rápido.

Pré-requisitos
--------------
- Node.js (recomendado recente; ver `engines` quando aplicável).
- pnpm (recomendado): instale com `npm i -g pnpm`.

Como rodar (rápido)
-------------------
1. Instale dependências:

```bash
pnpm install
```

2. Inicie o servidor de desenvolvimento:

```bash
pnpm dev
```

Comandos úteis
--------------
- `pnpm dev` — inicia o Vite dev server (SvelteKit).
- `pnpm build` — gera o build de produção.
- `pnpm preview` — pré-visualiza o build produzido.
- `pnpm run test` — roda os testes (unit + e2e, conforme configurado).

Notas sobre o framework
-----------------------
Svelte diferencia-se por compilar componentes para JavaScript altamente eficiente em tempo de build, evitando runtime virtual DOM; SvelteKit adiciona camada de roteamento e opções de rendering (SSR/SSG).

--

# sv

Everything you need to build a Svelte project, powered by [`sv`](https://github.com/sveltejs/cli).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```sh
# create a new project
npx sv create my-app
```

To recreate this project with the same configuration:

```sh
# recreate this project
pnpm dlx sv@0.17.0 create --template demo --types ts --add prettier eslint vitest="usages:unit,component" playwright tailwindcss="plugins:forms,typography" --install pnpm myapp
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

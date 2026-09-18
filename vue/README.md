# Vue (Vite)

Breve descrição
----------------
Projeto baseado em Vue 3 e Vite. Usa `vue-router` e `pinia` para roteamento e estado, respectivamente. Vite é usado como bundler/dev server para desenvolvimento rápido.

Pré-requisitos
--------------
- Node.js (compatível com as engines definidas).
- pnpm (recomendado): `npm i -g pnpm`.

Como rodar (rápido)
-------------------
```bash
pnpm install
pnpm dev
```

Build e preview
----------------
```bash
pnpm build
pnpm preview
```

Comandos úteis
--------------
- `pnpm dev` — inicia o servidor de desenvolvimento (Vite).
- `pnpm run build` — gera o build de produção.
- `pnpm run test:unit` — executa testes unitários (Vitest).
- `pnpm run test:e2e` — executa testes e2e (Playwright), se configurado.

Notas sobre o framework
-----------------------
Vue 3 oferece API Composition e melhorias de performance; use `pinia` para gerenciamento de estado e `vue-router` para rotas. Consulte `vite.config.ts` para plugins e integrações.

# vue

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
pnpm install
```

### Compile and Hot-Reload for Development

```sh
pnpm dev
```

### Type-Check, Compile and Minify for Production

```sh
pnpm build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
pnpm test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
pnpm build

# Runs the end-to-end tests
pnpm test:e2e
# Runs the tests only on Chromium
pnpm test:e2e --project=chromium
# Runs the tests of a specific file
pnpm test:e2e tests/example.spec.ts
# Runs the tests in debug mode
pnpm test:e2e --debug
```

### Lint with [ESLint](https://eslint.org/)

```sh
pnpm lint
```
